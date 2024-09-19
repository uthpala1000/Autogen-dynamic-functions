# AutoGen dynamic function execution example with UI 

This code demonstrates how AutoGen agents can be used to dynamically execute functions through a discussion and integrate with existing systems, specifically a database for inventory management.


## Key Components

- **AutoGen Agents**: 
  - `AssistantAgent`: Interprets user requests and manages the conversation flow
  - `UserProxyAgent`: Executes functions as directed by the AssistantAgent

- **Flask API**: Provides endpoints for starting chats, sending messages, and retrieving responses

- **Database Integration**: Uses pyodbc to connect to a SQL Server database for CRUD operations on inventory items


## How It Works

1. The user starts a chat session through the API.
2. The AssistantAgent interprets user messages and decides on actions.
3. When a database operation is needed, the AssistantAgent instructs the UserProxyAgent to execute the appropriate function.(Currently save and retireve)
4. Results are returned to the user in a conversational manner.


## Future Enhancements

This approach is very useful for implementing voice control over systems. By integrating speech-to-text and text-to-speech capabilities, this system could be extended to provide a fully voice-controlled interface for managing inventory or interacting with other business systems. This would make the system more accessible and efficient for users who prefer or require hands-free operation.


should I build a full voice-controlled inventory management system?

