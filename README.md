# CBT836
Converted to GitHub via [cbt2git](https://github.com/wizardofzos/cbt2git)

This is still a work in progress. GitHub repos will be deleted and created during this period...

```
//***FILE 836 is from Sam Golob and contains programs from CBT      *   FILE 836
//*           File 830 (Xephon MVS Update issues from July 1987     *   FILE 836
//*           thru December 1996) that have been fixed to run on    *   FILE 836
//*           z/OS (currently at 2.5).  Original versions of the    *   FILE 836
//*           programs have been modified so they work at whatever  *   FILE 836
//*           z/OS level is the highest available.                  *   FILE 836
//*                                                                 *   FILE 836
//*           Since the support rights for these Xephon materials   *   FILE 836
//*           were given to www.cbttape.org by Bob Thomas in 2008,  *   FILE 836
//*           we are now taking advantage, by trying to get some    *   FILE 836
//*           of these programs to run in a current environment.    *   FILE 836
//*                                                                 *   FILE 836
//*           We try to give credit to the original author, if      *   FILE 836
//*           that person's name is available in the original file. *   FILE 836
//*                                                                 *   FILE 836
//*           email:  sbgolob@cbttape.org                           *   FILE 836
//*                                                                 *   FILE 836
//*       Description of programs or articles.                      *   FILE 836
//*       In parentheses is the original member name in File 830.   *   FILE 836
//*                                                                 *   FILE 836
//*       ZTDM      - Rexx exec to restore the "Bottom of Data"     *   FILE 836
//*       (S.Golob)   line to your member lists.  This is changed   *   FILE 836
//*                   by some of the ISPF applications here.  But   *   FILE 836
//*                   you can use this little exec to put it back.  *   FILE 836
//*                   Or you can append it to the end of any exec   *   FILE 836
//*                   which alters the "bottom line" marker, and    *   FILE 836
//*                   set it back right.                            *   FILE 836
//*                                                                 *   FILE 836
//*       ASVTSCAN  - Program written by David Welch to summarize   *   FILE 836
//*       (AC7AF2B8)  the information about Address Space totals    *   FILE 836
//*                   that is found in the ASVT.                    *   FILE 836
//*       ASVTSCAT  - TSO command with the same output.             *   FILE 836
//*                                                                 *   FILE 836
//*       CHKASVT   - A companion program to ASVTSCAN, which        *   FILE 836
//*                   enumerates which address space numbers are    *   FILE 836
//*                   not reusable.  From CBT Tape File 473.        *   FILE 836
//*                   (from Scott Finlayson, thru Ron Robinson)     *   FILE 836
//*                                                                 *   FILE 836
//*       CLS       - Clear the screen and preserve terminal        *   FILE 836
//*       (A315B7EF)  type.                                         *   FILE 836
//*                                                                 *   FILE 836
//*       DFRMM     - An introduction to RMM, what it does, and     *   FILE 836
//*       (BEAEA3B9)  how it is set up.  This is not code, but      *   FILE 836
//*                   a how-to narrative from Rem Perretta.         *   FILE 836
//*                                                                 *   FILE 836
//*       EDTDSPLY  - Package to display devices under Esoteric     *   FILE 836
//*       (Q9802A5F)  Unit Names in ISPF.  (from Rem Perretta)      *   FILE 836
//*                   Members:  EDTINF (Assembler program)          *   FILE 836
//*                             EDTDSPLY (Rexx exec)                *   FILE 836
//*                             EDTPAN01, EDTPAN02  (ISPF Panels)   *   FILE 836
//*                                                                 *   FILE 836
//*       ESVCSCAN  - Package from Rem Perretta to display          *   FILE 836
//*       (YE55C023)  extended SVC tables under ISPF.               *   FILE 836
//*                                                                 *   FILE 836
//*       FINDSYSI  - Article by Roger Bowler about how to find     *   FILE 836
//*       (C8B469E7)  Job-related info in MVS control blocks.       *   FILE 836
//*                   (From Roger Bowler)                           *   FILE 836
//*                                                                 *   FILE 836
//*       GETDSN    - Look in TIOT to see if a dsname is allocated  *   FILE 836
//*       (A08A5369)  to a ddname.  Uses QSAM and is callable.      *   FILE 836
//*                   (Enhanced and IVP supplied by Willy Jensen.)  *   FILE 836
//*                   (Original article anonymous)                  *   FILE 836
//*                   GETDSNM - macro library in IEBUPDTE format    *   FILE 836
//*                                                                 *   FILE 836
//*       GETDEVNM  - Get Device Number....                         *   FILE 836
//*       (S254E5EF)  Rexx exec with backup assembler program       *   FILE 836
//*                   and panels.  You give it a disk volser, and   *   FILE 836
//*                   it returns the device unit address and other  *   FILE 836
//*                   nice information about the pack.              *   FILE 836
//*                   (From Rem Perretta)                           *   FILE 836
//*                   Members:  GETDEVNM (Rexx exec)                *   FILE 836
//*                             GETUADDR (Assembler program)        *   FILE 836
//*                             GETDEVP1 thru GETDEVP4 (panels)     *   FILE 836
//*                                                                 *   FILE 836
//*       GETOSLVL  - Display the current system level, but also    *   FILE 836
//*                   derive a hash as a unique return code, so     *   FILE 836
//*                   that the job steps following this one, can    *   FILE 836
//*                   depend on the operating system level.         *   FILE 836
//*                                                                 *   FILE 836
//*       LLASTATS  - From Mike Pekic via Bill Smith & Lionel Dyck  *   FILE 836
//*                   Xephon MVS Update 186 - March 2002            *   FILE 836
//*                   Produces LLA statistics via a REXX which      *   FILE 836
//*                   scrapes the output of the undocumented        *   FILE 836
//*                   operator command:  D LLA,STATISTICS           *   FILE 836
//*                   Produces beautiful ISPF formatted output.     *   FILE 836
//*                                                                 *   FILE 836
//*       LISTAPF   - Lists all APF-authorized datasets.            *   FILE 836
//*                   (from October 2002 MVS Update-fixed by SG)    *   FILE 836
//*                                                                 *   FILE 836
//*       MORESYSI  - Article with more information about how to    *   FILE 836
//*       (FEDEBB0D)  find information in MVS control blocks.       *   FILE 836
//*                   (From Lynn Grant)                             *   FILE 836
//*                                                                 *   FILE 836
//*       PRSMINFO  - Package to display LPAR, processor, and       *   FILE 836
//*       (D2F6A419)  IODF information.  From R.F.Perretta.         *   FILE 836
//*                   Packaged and fixed to run on z/OS 2.3.        *   FILE 836
//*                   (member is in TSO XMIT format)                *   FILE 836
//*                                                                 *   FILE 836
//*       RACFAUTH  - A program to give SPECIAL and/or OPERATIONS   *   FILE 836
//*                   authority to a userid.                        *   FILE 836
//*                                                                 *   FILE 836
//*       RACROUTE  - An assembler program to show how much RACF    *   FILE 836
//*       (David      authority that this userid has, to a dataset. *   FILE 836
//*         Spiegel)  Accompanied by a REXX exec to use the program *   FILE 836
//*                   to do a display.                              *   FILE 836
//*                                                                 *   FILE 836
//*       RGENR     - REXX to decompile RACF profiles and convert   *   FILE 836
//*       (A6B797AC)  them to "source" TSO RACF commands.           *   FILE 836
//*                                                                 *   FILE 836
//*       SEND@     - TSO command to send a non-deletable message   *   FILE 836
//*       (BC5C26EB)  to the operator console. (from Walter         *   FILE 836
//*                   Wiedemann)                                    *   FILE 836
//*                                                                 *   FILE 836
//*       SHOWALOC  - TSO CLIST to display TSO dataset allocations  *   FILE 836
//*       (F64BA4D1)  for a DDname.  (from Andrew Cahillane)        *   FILE 836
//*                                                                 *   FILE 836
//*       SMPEMOVE  - Instructions to move SMP/E zone entries from  *   FILE 836
//*       (A162FCC4)  one VSAM file (zone) to another, and to       *   FILE 836
//*                   combine two zones into one.                   *   FILE 836
//*                   (From John Bradley)                           *   FILE 836
//*                                                                 *   FILE 836
//*       STRPATRN  - An assembler macro to test a string against   *   FILE 836
//*                   a pattern.  (from Willy Jensen)               *   FILE 836
//*                                                                 *   FILE 836
//*       SUBCOMS   - REXX function to list all the names of        *   FILE 836
//*       (ABA7F5DD)  environments available to REXX.               *   FILE 836
//*                   (from Willy Jensen - Xephon contributor       *   FILE 836
//*                    was anonymous)                               *   FILE 836
//*                                                                 *   FILE 836
//*       SUBSYSxx  - REXX and PANELS to display subsystem          *   FILE 836
//*       (WAB4EB8B)  information under ISPF. (from R.F.Perretta)   *   FILE 836
//*                                                                 *   FILE 836
//*       SVCR****  - SVC Update Recording Table display (from      *   FILE 836
//*       (XABB8414)  R.F.Perretta). Displays all SVCs that have    *   FILE 836
//*                   been updated.                                 *   FILE 836
//*                                                                 *   FILE 836
//*       SWRID     - A more advanced version of USEID.  Assembles  *   FILE 836
//*                   differently for z/OS 2.2 and lower, and for   *   FILE 836
//*                   z/OS 2.3 and higher, with the 8-character     *   FILE 836
//*                   TSO userid support.  Also includes a lot of   *   FILE 836
//*                   WTO's to tell everybody what you did.         *   FILE 836
//*                                                                 *   FILE 836
//*       USEID     - (Xephon issue 33 August 2003)                 *   FILE 836
//*                   TSO command to change your userid in two      *   FILE 836
//*                   places, the ASXB and the ACEE (importantly)   *   FILE 836
//*                   so that you can run jobs with someone else's  *   FILE 836
//*                   authority.  You have to know the other id's   *   FILE 836
//*                   password, however, to effect the change.      *   FILE 836
//*                   (Fixed for 8-character TSO userid support.)   *   FILE 836
//*                                                                 *   FILE 836
//*       USEID22   - Pre-z/OS 2.3 version of USEID.                *   FILE 836
//*                   (No 8-character TSO userid support.)          *   FILE 836
//*                                                                 *   FILE 836
//*       WHEREIS   - Program to determine where a module was       *   FILE 836
//*       (AC7C7897)  loaded from.  This program does the job       *   FILE 836
//*                   particularly well. (Fixed by Willy Jensen.)   *   FILE 836
//*                   (Original contributor - Paul Poolsaar)        *   FILE 836
//*                                                                 *   FILE 836
//*       WTOPROG   - A multi-function WTO program.  Can be ysed    *   FILE 836
//*       (BB2BDE14)  to force a job to wait, if other jobs are     *   FILE 836
//*                   (or are not) present.  Or it may be used to   *   FILE 836
//*                   stop a job until the operator answers "Y"     *   FILE 836
//*                   to a WTOR message of your choice.             *   FILE 836
//*                   (from R.F.Perretta)  (Works fine on z/OS 2.3) *   FILE 836
//*                                                                 *   FILE 836
```
