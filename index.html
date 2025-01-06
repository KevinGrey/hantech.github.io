<!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>AI Chatbot</title>
        <script src="https://cdn.tailwindcss.com"></script>
        <style>
            /* Custom scrollbar styling */
            #chat-container::-webkit-scrollbar {
                width: 8px;
            }
            #chat-container::-webkit-scrollbar-thumb {
                background-color: #4f46e5; /* Indigo color */
                border-radius: 4px;
            }
            #chat-container::-webkit-scrollbar-track {
                background-color: #e5e7eb; /* Gray-200 */
            }
        </style>
    </head>
    <body class="bg-gradient-to-br from-indigo-500 via-purple-500 to-pink-500 min-h-screen flex items-center justify-center text-gray-800">
        <div class="max-w-3xl w-full bg-white shadow-lg rounded-lg overflow-hidden">
            <!-- Header -->
            <div class="bg-gradient-to-r from-indigo-500 to-purple-500 text-white p-6 text-center">
                <h1 class="text-3xl font-bold">AI Chatbot</h1>
                <p class="text-sm mt-2">Powered by GPT-4</p>
            </div>

            <!-- Chat Container -->
            <div id="chat-container" class="p-6 space-y-4 max-h-[400px] overflow-y-auto bg-gray-50">
                <!-- Chat messages will appear here -->
                <div class="text-center text-gray-400">Start the conversation!</div>
            </div>

            <!-- Input Section -->
            <div class="p-4 bg-gray-100 border-t">
                <div class="flex items-center">
                    <input id="user-input" type="text" placeholder="Type your message..." class="flex-1 border rounded-lg p-3 focus:outline-none focus:ring-2 focus:ring-indigo-500">
                    <button id="send-btn" class="ml-3 bg-indigo-500 text-white px-6 py-3 rounded-lg hover:bg-indigo-600 transition-all">Send</button>
                </div>
            </div>
        </div>

        <script>
            const chatContainer = document.getElementById('chat-container');
            const userInput = document.getElementById('user-input');
            const sendBtn = document.getElementById('send-btn');

            // Function to add a message to the chat
            function addMessage(sender, text) {
                const messageDiv = document.createElement('div');
                messageDiv.className = sender === 'user' ? 'text-right' : 'text-left';
                messageDiv.innerHTML = `
                    <div class="inline-block p-3 rounded-lg ${sender === 'user' ? 'bg-indigo-500 text-white' : 'bg-gray-200 text-gray-800'} shadow-md">
                        ${text}
                    </div>
                `;
                chatContainer.appendChild(messageDiv);
                chatContainer.scrollTop = chatContainer.scrollHeight; // Auto-scroll to the bottom
            }

            // Function to send a message
            async function sendMessage() {
                const userMessage = userInput.value.trim();
                if (!userMessage) return;

                // Add user message to chat
                addMessage('user', userMessage);
                userInput.value = '';

                // Call the backend API
                try {
                    const response = await fetch('/api/chat', {
                        method: 'POST',
                        headers: { 'Content-Type': 'application/json' },
                        body: JSON.stringify({ message: userMessage })
                    });
                    const data = await response.json();
                    addMessage('ai', data.reply);
                } catch (error) {
                    addMessage('ai', 'Error: Unable to connect to the server.');
                }
            }

            // Event listener for the send button
            sendBtn.addEventListener('click', sendMessage);

            // Allow pressing Enter to send a message
            userInput.addEventListener('keypress', (e) => {
                if (e.key === 'Enter') sendMessage();
            });
        </script>
    </body>
    </html>
