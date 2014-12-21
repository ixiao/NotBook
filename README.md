
心之所向，身之所往。
相由心生，推己及人。

Dec.10 2014
    Hello World

iOS-UI 一些方法及释义

<kbd>

-(BOOL)textFieldShouldReturn:(UITextField *)textField
{
    [self.textField resignFirstResponder];
    return YES;
}
-(BOOL)textView:(UITextView *)textView shouldChangeTextInRange:(NSRange)range replacementText:(NSString *)text
{
    if (self.segmentControl.selectedSegmentIndex == 1)
    {
        if ([@"\n" isEqualToString:text])
        {
            [self.TextView resignFirstResponder];
            return NO;
        }

    }
    return YES;
}  
  
</kbd>
分割

<samp>
-(BOOL)textFieldShouldReturn:(UITextField *)textField

{

    [self.textField resignFirstResponder];
    return YES;

}

-(BOOL)textView:(UITextView *)textView shouldChangeTextInRange:(NSRange)range replacementText:(NSString *)text

{

    if (self.segmentControl.selectedSegmentIndex == 1)
    {
        if ([@"\n" isEqualToString:text])
        {
            [self.TextView resignFirstResponder];
            return NO;
        }

    }
    return YES;
} 
</samp>