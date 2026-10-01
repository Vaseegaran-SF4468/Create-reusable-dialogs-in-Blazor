# Create Reusable Dialogs

## Overview

This sample demonstrates how to create reusable dialog functionality in a Blazor Server application using the Syncfusion [Blazor Dialog](https://www.syncfusion.com/blazor-components/blazor-modal-dialog) component. Instead of creating and maintaining separate dialog implementations for individual pages, the sample centralizes dialog rendering and interaction logic into reusable components and services. This approach simplifies maintenance, reduces duplicated code, and provides a consistent modal experience across the application. The project serves as a practical reference for implementing reusable confirmation dialogs, notifications, and modal workflows in Blazor applications.

## Key Features

- Uses Syncfusion [Blazor Dialog](https://www.syncfusion.com/blazor-components/blazor-modal-dialog) services to display alogs in a Blazor Server application.
- Injects `SfDialogService` using dependency injection to provide dialog functionality within Razor components.
- Triggers dialog display through the `AlertAsync(string message, string title)` method.
- Displays a predefined alert message (`"10% of battery remaining"`) with a custom dialog title (`"Low Battery"`).
- Uses a Syncfusion `SfButton` component to initiate dialog interactions.
- Demonstrates asynchronous dialog handling using `async` and `await` patterns.
- Updates component state after the dialog is closed by the user.
- Shows how to provide user feedback by displaying a status message after dialog completion.
- Illustrates integration between Syncfusion Blazor Buttons and Dialog services within a Razor component.
- Provides a simple reference implementation for confirmation, notification, and alert dialog scenarios using `SfDialogService`.

## Prerequisites

- [Visual Studio 2022](https://visualstudio.microsoft.com/vs/) or [Visual Studio Code](https://code.visualstudio.com/)
- [.NET SDK](https://dotnet.microsoft.com/en-us/download/dotnet) compatible with the project's target framework

## How to Run the Project

**Visual Studio 2022**

1. Clone or download this repository.
2. Open `CreateReusableDialog.sln`.
3. Restore all NuGet packages.
4. Ensure `CreateReusableDialog` is selected as the startup project.
5. Build the solution.
6. Run the application using `Ctrl+F5`.

**Visual Studio Code**

1. Open the repository folder in Visual Studio Code.
2. Open a terminal and navigate to the project directory.

```bash
dotnet restore
dotnet run
```

3. Open the local URL displayed in the terminal after the application starts.

## Project Structure

`Pages/Index.razor` - Primary sample page demonstrating dialog service usage. Injects `SfDialogService`, renders an `SfButton`, calls `DialogService.AlertAsync("10% of battery remaining", "Low Battery")`, and updates a status message after the alert dialog is closed.

## Support and Feedback

- For general product questions, visit the [Syncfusion Community Forum](https://www.syncfusion.com/forums) or [Syncfusion Support](https://www.syncfusion.com/support).
- To report an issue specific to this sample, open a GitHub issue in this repository.
- Refer to the official Syncfusion Dialog documentation: https://blazor.syncfusion.com/documentation/dialog/getting-started

## License

This is a Syncfusion sample project provided to demonstrate product usage. Review the [Syncfusion license terms](https://www.syncfusion.com/sales/pricing?category=ui-components) before using Syncfusion components in your own applications.