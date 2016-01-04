# Working with Issue Labels

Labels are appended using the method `NewIssue.Labels.Add(x)`, where `x` is a `string` from the list below.

Example:

    var myNewIssue = new NewIssue("Issue with dropdown menu");
    myNewIssue.Labels.Add("bug");
    
The default labels that come with every repository are:
- bug
- duplicate
- enhancement
- help wanted
- invalid
- question
- wontfix

You can add new labels within the `Issues` section of your own repository, clicking on the "Labels" button.

However, using the `Add(x)` function where `x` is a non-existent label will **still work perfectly fine**, creating the label which you specified. For example, using `myNewIssue.Labels.Add("my-new-label")` will not crash, but will instead add the tag **my-new-label** to the newly created issue.
