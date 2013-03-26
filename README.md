XR.Mono.Cover (c) 2013 Ian Norton
----------------------------------

XR.Mono.Cover is a simple code coverage tool specifically for mono. 
It will record which lines of your source are actually executed and 
log some basic statistics like call counts and the number of times 
a line is actually run.

![screenshot](https://raw.github.com/inorton/XR.Baboon/master/screenshots/baboon-001.png "Baboon Screenshot!")

It built on top of Mono.Debugger.Soft and so requires the mono 
runtime rather than the .Net one.

Results are gathered by the covtool program and can be 
displayed/analysed by the cov-console or cov-gtk programs.

Coverage data generated by covtool ( via Mono.XR.Cover library ) is 
saved in a Sqlite database file for easy processing and quick 
generation.

covtool will run any mono/c# process you ask of it, such as 
nunit-console or even graphical apps. In time covtool may allow you 
to attach to existing processes after they have started.

XR.Mono.Cover will not check coverage of unmanaged code, perhaps 
one day of Mono.Debugger.Soft does, this will too.
