# lakza9
acdtive
2019-07-20 15:29:25> Program: Starting Squirrel Updater: --install .
2019-07-20 15:29:25> Program: Starting install, writing to C:\Users\mosi\AppData\Local\SquirrelTemp
2019-07-20 15:29:25> Program: About to install to: C:\Users\mosi\AppData\Local\GitHubDesktop
2019-07-20 15:29:25> CheckForUpdateImpl: Couldn't write out staging user ID, this user probably shouldn't get beta anything: System.IO.DirectoryNotFoundException: Could not find a part of the path 'C:\Users\mosi\AppData\Local\GitHubDesktop\packages\.betaId'.
   at System.IO.__Error.WinIOError(Int32 errorCode, String maybeFullPath)
   at System.IO.FileStream.Init(String path, FileMode mode, FileAccess access, Int32 rights, Boolean useRights, FileShare share, Int32 bufferSize, FileOptions options, SECURITY_ATTRIBUTES secAttrs, String msgPath, Boolean bFromProxy, Boolean useLongPath, Boolean checkHost)
   at System.IO.FileStream..ctor(String path, FileMode mode, FileAccess access, FileShare share, Int32 bufferSize, FileOptions options, String msgPath, Boolean bFromProxy, Boolean useLongPath, Boolean checkHost)
   at System.IO.StreamWriter.CreateFile(String path, Boolean append, Boolean checkHost)
   at System.IO.StreamWriter..ctor(String path, Boolean append, Encoding encoding, Int32 bufferSize, Boolean checkHost)
   at System.IO.File.InternalWriteAllText(String path, String contents, Encoding encoding, Boolean checkHost)
   at System.IO.File.WriteAllText(String path, String contents, Encoding encoding)
   at Squirrel.UpdateManager.CheckForUpdateImpl.getOrCreateStagedUserId()
2019-07-20 15:29:25> CheckForUpdateImpl: Failed to load local releases, starting from scratch: System.IO.DirectoryNotFoundException: Could not find a part of the path 'C:\Users\mosi\AppData\Local\GitHubDesktop\packages\RELEASES'.
   at System.IO.__Error.WinIOError(Int32 errorCode, String maybeFullPath)
   at System.IO.FileStream.Init(String path, FileMode mode, FileAccess access, Int32 rights, Boolean useRights, FileShare share, Int32 bufferSize, FileOptions options, SECURITY_ATTRIBUTES secAttrs, String msgPath, Boolean bFromProxy, Boolean useLongPath, Boolean checkHost)
   at System.IO.FileStream..ctor(String path, FileMode mode, FileAccess access, FileShare share)
   at Squirrel.Utility.LoadLocalReleases(String localReleaseFile)
   at Squirrel.UpdateManager.CheckForUpdateImpl.<CheckForUpdate>d__2.MoveNext()
2019-07-20 15:29:25> CheckForUpdateImpl: Reading RELEASES file from C:\Users\mosi\AppData\Local\SquirrelTemp
2019-07-20 15:29:25> CheckForUpdateImpl: First run or local directory is corrupt, starting from scratch
2019-07-20 15:29:26> ApplyReleasesImpl: Writing files to app directory: C:\Users\mosi\AppData\Local\GitHubDesktop\app-2.1.0
2019-07-20 15:29:26> LogHost: Rigging execution stub for lib/net45/GitHubDesktop_ExecutionStub.exe to C:\Users\mosi\AppData\Local\GitHubDesktop\GitHubDesktop.exe
2019-07-20 15:29:34> ApplyReleasesImpl: Squirrel Enabled Apps: [C:\Users\mosi\AppData\Local\GitHubDesktop\app-2.1.0\GitHubDesktop.exe]
2019-07-20 15:29:35> ApplyReleasesImpl: Couldn't run Squirrel hook, continuing: C:\Users\mosi\AppData\Local\GitHubDesktop\app-2.1.0\GitHubDesktop.exe: System.ComponentModel.Win32Exception (0x80004005): The specified executable is not a valid application for this OS platform.
   at System.Diagnostics.Process.StartWithCreateProcess(ProcessStartInfo startInfo)
   at System.Diagnostics.Process.Start()
   at System.Diagnostics.Process.Start(ProcessStartInfo startInfo)
   at Squirrel.Utility.<InvokeProcessAsync>d__11.MoveNext()
--- End of stack trace from previous location where exception was thrown ---
   at System.Runtime.CompilerServices.TaskAwaiter.ThrowForNonSuccess(Task task)
   at System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   at Squirrel.UpdateManager.ApplyReleasesImpl.<>c__DisplayClass10_0.<<invokePostInstall>b__0>d.MoveNext()
2019-07-20 15:29:35> IEnableLogger: Failed to invoke post-install: System.ComponentModel.Win32Exception (0x80004005): The specified executable is not a valid application for this OS platform.
   at System.Diagnostics.Process.StartWithShellExecuteEx(ProcessStartInfo startInfo)
   at System.Diagnostics.Process.Start()
   at System.Diagnostics.Process.Start(ProcessStartInfo startInfo)
   at Squirrel.UpdateManager.ApplyReleasesImpl.<>c.<invokePostInstall>b__10_6(ProcessStartInfo info)
   at Squirrel.EnumerableExtensions.ForEach[TSource](IEnumerable`1 source, Action`1 onNext)
   at Squirrel.UpdateManager.ApplyReleasesImpl.<invokePostInstall>d__10.MoveNext()
--- End of stack trace from previous location where exception was thrown ---
   at System.Runtime.CompilerServices.TaskAwaiter.ThrowForNonSuccess(Task task)
   at System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   at Squirrel.Utility.<LogIfThrows>d__37.MoveNext()
2019-07-20 15:29:36> Unhandled exception: System.AggregateException: One or more errors occurred. ---> System.ComponentModel.Win32Exception: The specified executable is not a valid application for this OS platform.
   at System.Diagnostics.Process.StartWithShellExecuteEx(ProcessStartInfo startInfo)
   at System.Diagnostics.Process.Start()
   at System.Diagnostics.Process.Start(ProcessStartInfo startInfo)
   at Squirrel.UpdateManager.ApplyReleasesImpl.<>c.<invokePostInstall>b__10_6(ProcessStartInfo info)
   at Squirrel.EnumerableExtensions.ForEach[TSource](IEnumerable`1 source, Action`1 onNext)
   at Squirrel.UpdateManager.ApplyReleasesImpl.<invokePostInstall>d__10.MoveNext()
--- End of stack trace from previous location where exception was thrown ---
   at System.Runtime.CompilerServices.TaskAwaiter.ThrowForNonSuccess(Task task)
   at System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   at Squirrel.Utility.<LogIfThrows>d__37.MoveNext()
--- End of stack trace from previous location where exception was thrown ---
   at System.Runtime.CompilerServices.TaskAwaiter.ThrowForNonSuccess(Task task)
   at System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   at System.Runtime.CompilerServices.TaskAwaiter.ValidateEnd(Task task)
   at Squirrel.UpdateManager.ApplyReleasesImpl.<ApplyReleases>d__2.MoveNext()
--- End of stack trace from previous location where exception was thrown ---
   at System.Runtime.CompilerServices.TaskAwaiter.ThrowForNonSuccess(Task task)
   at System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   at Squirrel.UpdateManager.<FullInstall>d__10.MoveNext()
--- End of stack trace from previous location where exception was thrown ---
   at System.Runtime.CompilerServices.TaskAwaiter.ThrowForNonSuccess(Task task)
   at System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   at System.Runtime.CompilerServices.TaskAwaiter.ValidateEnd(Task task)
   at Squirrel.Update.Program.<Install>d__4.MoveNext()
   --- End of inner exception stack trace ---
   at System.Threading.Tasks.Task.ThrowIfExceptional(Boolean includeTaskCanceledExceptions)
   at System.Threading.Tasks.Task.Wait(Int32 millisecondsTimeout, CancellationToken cancellationToken)
   at System.Threading.Tasks.Task.Wait()
   at Squirrel.Update.Program.executeCommandLine(String[] args)
   at Squirrel.Update.Program.main(String[] args)
---> (Inner Exception #0) System.ComponentModel.Win32Exception (0x80004005): The specified executable is not a valid application for this OS platform.
   at System.Diagnostics.Process.StartWithShellExecuteEx(ProcessStartInfo startInfo)
   at System.Diagnostics.Process.Start()
   at System.Diagnostics.Process.Start(ProcessStartInfo startInfo)
   at Squirrel.UpdateManager.ApplyReleasesImpl.<>c.<invokePostInstall>b__10_6(ProcessStartInfo info)
   at Squirrel.EnumerableExtensions.ForEach[TSource](IEnumerable`1 source, Action`1 onNext)
   at Squirrel.UpdateManager.ApplyReleasesImpl.<invokePostInstall>d__10.MoveNext()
--- End of stack trace from previous location where exception was thrown ---
   at System.Runtime.CompilerServices.TaskAwaiter.ThrowForNonSuccess(Task task)
   at System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   at Squirrel.Utility.<LogIfThrows>d__37.MoveNext()
--- End of stack trace from previous location where exception was thrown ---
   at System.Runtime.CompilerServices.TaskAwaiter.ThrowForNonSuccess(Task task)
   at System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   at System.Runtime.CompilerServices.TaskAwaiter.ValidateEnd(Task task)
   at Squirrel.UpdateManager.ApplyReleasesImpl.<ApplyReleases>d__2.MoveNext()
--- End of stack trace from previous location where exception was thrown ---
   at System.Runtime.CompilerServices.TaskAwaiter.ThrowForNonSuccess(Task task)
   at System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   at Squirrel.UpdateManager.<FullInstall>d__10.MoveNext()
--- End of stack trace from previous location where exception was thrown ---
   at System.Runtime.CompilerServices.TaskAwaiter.ThrowForNonSuccess(Task task)
   at System.Runtime.CompilerServices.TaskAwaiter.HandleNonSuccessAndDebuggerNotification(Task task)
   at System.Runtime.CompilerServices.TaskAwaiter.ValidateEnd(Task task)
   at Squirrel.Update.Program.<Install>d__4.MoveNext()<---

