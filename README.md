#Log_in-attempt_UI

Public Class Form1
    Dim Attempt As Integer = "0"
    Private Sub Button1_Click(ByVal sender As System.Object, ByVal e As System.EventArgs) Handles Button1.Click
        Dim username, password As String
        username = TextBox1.Text
        password = TextBox2.Text

        If username = "user" And password = "password" Then
            MsgBox("Welcome")
            Form2.Show()
            Me.Hide()
        ElseIf username = "user2" And password = "password2" Then
            MsgBox("Welcome")
            Form2.Show()
            Me.Hide()
        ElseIf Attempt = 3 Then
            MsgBox("Maximum number of attempts (3), program will close")
            Close()
        Else

        End If
        Attempt = Attempt + 1
        TextBox1.Text = ""
        TextBox2.Text = ""
        TextBox1.Focus()
    End Sub
End Class
