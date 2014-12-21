
心之所向，身之所往。
相由心生，推己及人。

Dec.10 2014
    Hello World

iOS-UI 一些方法及释义

```
-(BOOL)textFieldShouldReturn:(UITextField *)textField

{
//文本将要返回，调用此方法，配合
"- (IBAction)editingLbel:(UITextField *)sender" 方法可以使文本显示在标签上

    [self.textField resignFirstResponder];
    return YES;

}
```

```
-(BOOL)textView:(UITextView *)textView shouldChangeTextInRange:(NSRange)range replacementText:(NSString *)text

{
//如果你的textview里不用回车键，可以把回车键当做退出键盘的响应键。
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
```