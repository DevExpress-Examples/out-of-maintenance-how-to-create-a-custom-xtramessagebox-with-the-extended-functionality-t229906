# How to create a custom XtraMessageBox with the extended functionality

## This example is obsolete and starting with version 18.1 this task can be accomplished out of the box by handling the **XtraMessageBoxArgs.Showing** event and adjusting the **XtraMessageBoxArgs** settings.

**Details:**
Starting with version *15.2*, we implemented the <a href="https://docs.devexpress.com/WindowsForms/DevExpress.XtraEditors.XtraBaseArgs.Showing">XtraMessageBoxArgs.Showing event</a> that is designed to customize the dialog form before it is shown. This allows you to disable/enable buttons, specify the form's start position etc.
Also, in version *18.1*, we introduced the **Auto Close** feature for the **XtraMessageBox** dialog. Use the **XtraMessageBoxArgs.AutoCloseOptions** to customize it. For more information, see <a href="https://docs.devexpress.com/WindowsForms/114566/controls-and-libraries/messages-notifications-and-dialogs/xtramessagebox">XtraMessageBox</a>.

## ***If the built-in functionality does not suit you, we will be happy to find the most appropriate solution for you if you describe your real-life scenario. Just click <a href="https://www.devexpress.com/Support/Center/Question/Create">here</a> to submit a ticket to our Support Center.***
