# STACK
Algorithm/Stack

namespace stack
 public partial class Form1 : Form
 {
 public Form1()
 {
 InitializeComponent();
 }
 Stack s = new Stack();
 private void ekle_Click(object sender, EventArgs e)
 {
 s.Push(textBox1.Text);
 }
 private void listboxtaGoster_Click(object sender, EventArgs e)
 {
 listBox1.Items.Clear();
 foreach (object i in s)
 {
 listBox1.Items.Add(i);
 }
 }
 private void labeldeGosterSil_Click(object sender, EventArgs e)
 {
 label1.Text = s.Pop().ToString();
 private void labeldeGoster_Click(object sender, EventArgs e)
 {
 label1.Text = s.Peek().ToString();
 }
 }
 }
