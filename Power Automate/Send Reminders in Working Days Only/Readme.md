Sending Reminders through Power Automate is a very common task. This is usually achieved through a scheduled Flow where the Flow runs daily ,loops through all the tasks in a list and if the due date of any matches with today's date, sends the reminder.

  

However, there can be scenarios when the reminder date falls on a weekend or a holiday, or the recipient is Out-of-office, so there is high chance that they will overlook the reminder.

  

To overcome this issue, I have created this sample Flow with below logic -

*   The Flow will run only on weekdays and send reminder on a date which is 3 days before the due date.(you can change the no. of days based on your requirement)
*   If the actual reminder date falls on a holiday or weekend, it will send the reminder on the last working day before the weekend and holiday starts.
*   If the recipient is out of office, it will add the recipients manager in cc.

  

The unmanaged Solution HandlenonworkingDays_1_0_0_2.zip contains –

1.     Cloud Flow - Send Reminders on Working Days only - Scheduled Flow with weekly frequency that runs on Monday, Tuesday, Wednesday, Thursday and Friday (excluding Saturday and Sunday)

2.     Dataverse Table -Task Tracker – Sample table to store the tasks with the Due Date and Assigned To Fields

3.     Dataverse table – Holidays - Sample table to store the Holidays list
