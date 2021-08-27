<!-- default badges list -->
![](https://img.shields.io/endpoint?url=https://codecentral.devexpress.com/api/v1/VersionRange/128619679/14.2.3%2B)
[![](https://img.shields.io/badge/Open_in_DevExpress_Support_Center-FF7200?style=flat-square&logo=DevExpress&logoColor=white)](https://supportcenter.devexpress.com/ticket/details/T229906)
[![](https://img.shields.io/badge/📖_How_to_use_DevExpress_Examples-e9f6fc?style=flat-square)](https://docs.devexpress.com/GeneralInformation/403183)
<!-- default badges end -->
<!-- default file list -->
*Files to look at*:

* **[MainForm.cs](./CS/MessageBoxHelper/MainForm.cs) (VB: [MainForm.vb](./VB/MessageBoxHelper/MainForm.vb))**
* [MyXtraMessageArgs.cs](./CS/MessageBoxHelper/MyMessageBox/MyXtraMessageArgs.cs) (VB: [MyXtraMessageArgs.vb](./VB/MessageBoxHelper/MyMessageBox/MyXtraMessageArgs.vb))
* [MyXtraMessageBox.cs](./CS/MessageBoxHelper/MyMessageBox/MyXtraMessageBox.cs) (VB: [MyXtraMessageBoxForm.vb](./VB/MessageBoxHelper/MyMessageBox/MyXtraMessageBoxForm.vb))
* [MyXtraMessageBoxForm.cs](./CS/MessageBoxHelper/MyMessageBox/MyXtraMessageBoxForm.cs) (VB: [MyXtraMessageBoxForm.vb](./VB/MessageBoxHelper/MyMessageBox/MyXtraMessageBoxForm.vb))
<!-- default file list end -->
# How to create a custom XtraMessageBox with the extended functionality

<p><strong>Important note.</strong></p>

Starting with version _15.2_, we implemented the **XtraMessageBoxArgs.Showing** event that is designed to customize the dialog form before it is shown. This allows you to disable/enable buttons, specify the form's start position etc. Also, in version _18.1_, we introduced the **Auto Close** feature for the **XtraMessageBox** dialog. Use the **XtraMessageBoxArgs.AutoCloseOptions** to customize it.

## ***If you still prefer the custom approach described below, please clarify why the built-in solution is not suitable for you. Just click   [here](https://www.devexpress.com/Support/Center/Question/Create) to submit a ticket to our Support Center.***

For earlier versions:

<p>This example demonstrates how to create a MessageBox with an extended functionality. For this, create MyXtraMessageBox class descendant that is inherited from the XtraMessageBox class and uses the XtraMessageBoxArgs class - a MyXtraMessageArgs descendant which contains properties to customize the XtraMessageBox behavior. <br />- ShowCountDown. If this property is true, the message box title will show you how many seconds are left before the timeout. When the countdown is over, the title will show its usual value.<br />- ShowNextTime. This property allows you to show a CheckBox on your message form. When you close the form, the result will be saved in the ShowMessageNextTime property of MyXtraMessageArgs and you can use this value later.<br />- DisableButtons. If this property value is true, all buttons except for "Cancel" will be disabled on the form.<br />- DisableCancel. This property gives you an opportunity to disable the "Cancel" button on the form.<br />- AutoClose. If you want to close your form, after the countdown is over, set this property to true. Also, you need to define the value of the AutoCloseResult property. This property shows what value will be received from the MyXtraMessageBox.Show method if the form is automatically closed.<br />- Center. If this property value is true, the MessageBox will be center aligned against its parent form.<br />- Timeout. This property sets the timer for the AutoClose and ShowCountDown properties in seconds. Its value should be greater than 0, otherwise, these properties will be unavailable.<br />- Buttons. This property specifies what buttons will be available on the form.<br />- Icon. This property specifies the MessageBox icon.</p>
