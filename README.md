# login
here is my log in page for my new project, employee log in system. I'm currently updating it now for more details.

Public Class login

    Private Sub Button1_Click(ByVal sender As System.Object, ByVal e As System.EventArgs) Handles Button1.Click
        If TextBox1.Text = "username" And TextBox2.Text = "password" Then form1.ShowDialog() Else 
        MsgBox("Sorry, mate but either your password or username is incorrect.", MsgBoxStyle.Critical)
        Information(")")
    End Sub

    Private Sub Information(ByVal p1 As String)
        Throw New NotImplementedException
    End Sub

End Class
