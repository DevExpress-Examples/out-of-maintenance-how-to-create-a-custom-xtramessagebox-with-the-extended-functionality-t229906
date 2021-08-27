<!-- default badges list -->
![](https://img.shields.io/endpoint?url=https://codecentral.devexpress.com/api/v1/VersionRange/128619679/18.1.3%2B)
[![](https://img.shields.io/badge/Open_in_DevExpress_Support_Center-FF7200?style=flat-square&logo=DevExpress&logoColor=white)](https://supportcenter.devexpress.com/ticket/details/T229906)
[![](https://img.shields.io/badge/📖_How_to_use_DevExpress_Examples-e9f6fc?style=flat-square)](https://docs.devexpress.com/GeneralInformation/403183)
<!-- default badges end -->
# How to create a custom XtraMessageBox with the extended functionality

## This example is obsolete and starting with version 18.1 this task can be accomplished out of the box by handling the **XtraMessageBoxArgs.Showing** event and adjusting the **XtraMessageBoxArgs** settings.

**Details:**
Starting with version *15.2*, we implemented the <a href="https://docs.devexpress.com/WindowsForms/DevExpress.XtraEditors.XtraBaseArgs.Showing">XtraMessageBoxArgs.Showing event</a> that is designed to customize the dialog form before it is shown. This allows you to disable/enable buttons, specify the form's start position etc.
Also, in version *18.1*, we introduced the **Auto Close** feature for the **XtraMessageBox** dialog. Use the **XtraMessageBoxArgs.AutoCloseOptions** to customize it. For more information, see <a href="https://docs.devexpress.com/WindowsForms/114566/controls-and-libraries/messages-notifications-and-dialogs/xtramessagebox">XtraMessageBox</a>.

## ***If the built-in functionality does not suit you, we will be happy to find the most appropriate solution for you if you describe your real-life scenario. Just click <a href="https://www.devexpress.com/Support/Center/Question/Create">here</a> to submit a ticket to our Support Center.***
