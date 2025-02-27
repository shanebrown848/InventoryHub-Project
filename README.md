

# InventoryHub

InventoryHub is a full-stack inventory management application built using Blazor for the front-end and .NET Minimal APIs for the back-end. The application enables users to view product details in real time and demonstrates seamless communication between client and server.

## Project Structure

```
InventoryHub/
├── BlazorFrontEnd/
│   ├── wwwroot/
│   ├── Pages/
│   │   └── FetchProducts.razor
│   ├── Program.cs
│   └── _Imports.razor (and other Blazor files)
├── MinimalApiBackEnd/
│   ├── Program.cs
│   └── appsettings.json (if needed)
├── README.md
└── REFLECTION.md
```

## Features

- **Seamless Integration:**  
  The Blazor front-end communicates with the .NET Minimal API back-end using HttpClient to fetch product data.

- **Robust Error Handling:**  
  The code includes try-catch blocks to gracefully handle network issues and JSON deserialization errors.

- **Structured JSON Responses:**  
  The back-end returns well-structured JSON data including product details and a nested category object for each product.

- **CORS Configuration:**  
  The Minimal API is configured with CORS to allow cross-origin requests from the Blazor front-end.

## Setup Instructions

1. **Clone the Repository:**
   ```bash
   git clone <repository-url>
   ```
2. **Run the Minimal API Back-End:**
   - Navigate to the `MinimalApiBackEnd` folder.
   - Run `dotnet run` to start the API.

3. **Run the Blazor Front-End:**
   - Navigate to the `BlazorFrontEnd` folder.
   - Run `dotnet run` or use Visual Studio Code to launch the Blazor application.

4. **Access the Application:**
   - Open your browser and navigate to `https://localhost:5001/fetchproducts` (or the appropriate URL) to view the product list.
