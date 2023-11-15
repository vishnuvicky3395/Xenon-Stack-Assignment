# Xenon-Stack-Assignment
Assignment-1 Manual
.TH INTERNCTL 1 "November 2023" "v0.1.0" "internsctl manual"

.SH NAME
internsctl \- Custom Linux command for managing intern operations

.SH SYNOPSIS
.B internsctl
[\fIOPTIONS\fR]
[\fICOMMAND\fR]

.SH DESCRIPTION
This manual page documents the \fBinternsctl\fR command.

.PP
\fBinternsctl\fR is a custom command-line tool for various intern-related operations.

.SH OPTIONS
The following options are supported:

.TP
.B \-\-help
Display help information.

.TP
.B \-\-version
Display version information.

.SH COMMANDS
The following commands are supported:

.TP
.BR cpu getinfo
Get CPU information.

.TP
.BR user create " <username>"
Create a new user.

.TP
.BR user list
List all regular users.

.TP
.BR user list " \-\-sudo-only"
List users with sudo permissions.

.TP
.BR file getinfo " <file-name>"
Get information about a file.

.SH EXAMPLES
.PP
To create a new user:
.nf
.B internsctl user create new_user
.fi

.PP
To list all regular users:
.nf
.B internsctl user list
.fi

.PP
To list users with sudo permissions:
.nf
.B internsctl user list \-\-sudo-only
.fi

.PP
To get information about a file:
.nf
.B internsctl file getinfo file.txt
.fi

.SH SEE ALSO
.BR lscpu (1)

