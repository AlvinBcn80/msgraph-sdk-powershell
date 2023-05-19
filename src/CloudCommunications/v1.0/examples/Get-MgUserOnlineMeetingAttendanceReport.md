### Example 1: Code snippet

```powershellImport-Module Microsoft.Graph.CloudCommunications

# A UPN can also be used as -UserId.
Get-MgUserOnlineMeetingAttendanceReport -UserId $userId -OnlineMeetingId $onlineMeetingId -MeetingAttendanceReportId $meetingAttendanceReportId -ExpandProperty "attendanceRecords"
```
This example shows how to use the Get-MgUserOnlineMeetingAttendanceReport Cmdlet.
To learn about permissions for this resource, see the [permissions reference](/graph/permissions-reference).

