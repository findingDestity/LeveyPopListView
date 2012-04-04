### Differences from the original version

Levey did an amazing work, but I needed the ability to show this controller in a modal behavior, so now there's an option isModal that is set to YES by default. Clicking anywhere outside the tableview does nothing, only selecting a row will do.

### What's it?

When your app have so many options to choose, LeveyPopListView is an alternative of UIActionSheet, hope it can help someone :)

### How to

**Create and show the View**

	LeveyPopListView *lplv = [[LeveyPopListView alloc] initWithTitle:@"Share Photo to..." options:_options];
    lplv.delegate = self;
    [lplv showInView:self.window animated:YES];
    [lplv release];

**Get the delegate methods**

	#pragma mark - LeveyPopListView delegates
	- (void)leveyPopListView:(LeveyPopListView *)popListView didSelectedIndex:(NSInteger)anIndex;
	- (void)leveyPopListViewDidCancel;



### Screenshot ⤵

![Screen](http://i.minus.com/iDQo9wuPCB1Gr.png)    
