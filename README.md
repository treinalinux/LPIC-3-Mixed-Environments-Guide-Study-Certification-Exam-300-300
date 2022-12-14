# Linux Professional Institute LPIC-3 Mixed Environments

The LPIC-3 certification is the culmination of the multi-level professional certification program of the Linux Professional Institute (LPI). LPIC-3 is designed for the enterprise-level Linux professional and represents the highest level of professional, distribution-neutral Linux certification within the industry. Four separate LPIC-3 specialty certifications are available. Passing any one of the four exams will grant the LPIC-3 certification for that specialty.

The LPIC-3 Mixed Environments certification covers the administration of Linux systems enterprise-wide in mixed environments.

Current version: 3.0 (Exam code 300-300)

Previous version: 1.0 (Exam code 300-100)
Available until February 23rd, 2022

Objectives: 300-300

Prerequisites: The candidate must have an active LPIC-2 certification to receive the LPIC-3 certification.

Requirements: Passing the 300 exam. The 90-minute exam is 60 multiple-choice and fill-in-the-blank questions.

Validity period: 5 years

Cost: Click here for exam pricing in your country.

Languages for exam available in VUE test centers: English, Japanese

## LPIC-3 Mixed Environments major topics

- Samba Basics
- Samba and Active Directory Domains
- Samba Share Configuration
- Samba Client Configuration
- Linux Identity Management and File Sharing

---

For reader:

- [Identity](https://learn.microsoft.com/pt-br/windows-server/identity/identity-and-access)
- [Lightweight Directory Access Protocol](https://learn.microsoft.com/en-us/previous-versions/windows/desktop/ldap/lightweight-directory-access-protocol-ldap-api)
- [Kerberos](https://learn.microsoft.com/en-us/previous-versions/tn-archive/cc995228(v=technet.10)?redirectedfrom=MSDN#Anchor_0)

---

LPIC-3 Exam 300: Mixed Environments

 

Exam Objectives Version: Version 3.0

Exam Code: 300-300

About Objective Weights: Each objective is assigned a weighting value. The weights indicate the relative importance of each objective on the exam. Objectives with higher weights will be covered in the exam with more questions

---

## Topic 301: Samba Basics

### 301.1 Samba Concepts and Architecture (weight: 2)

**Weight 2**

**Description**

Candidates should understand the essential concepts of Samba, including the various Samba server processes and networking protocols used by Samba when acting in various roles. Samba version 4.8 or higher is covered.

**Key Knowledge Areas**:

- [ ] Understand the roles of the various Samba daemons and components
- [ ] Understand key issues regarding heterogeneous networks
- [ ] Understand the networking services used with SMB/[CIFS](https://www.samba.org/cifs/) and Active Directory, including their ports
- [ ] Understand the major features of SMB protocol versions 1.0, 2.0, 2.1 and 3.0
- [ ] Understand of Samba 3 and Samba 4 differences
- [ ] [Awareness of Samba VFS modules](https://wiki.samba.org/index.php/Virtual_File_System_Modules#Developing_VFS_Modules)
- [ ] Awareness of Samba Clustering and CTDB


Partial list of the used files, terms and utilities:

- [ ] **smbd** `Server to provide SMB/CIFS services to clients`
- [ ] **nmbd** `NetBIOS name server to provide NetBIOS over IP naming services to clients`
- [ ] **samba** `A Windows AD and SMB/CIFS fileserver for UNIX | Server to provide AD and SMB/CIFS services to clients`
- [ ] **winbindd** `Name Service Switch daemon for resolving names from NT servers`


### 301.2 Samba Configuration (weight: 4)

**Weight 4**

**Description**

Candidates should be able to configure the Samba daemons.

**Key Knowledge Areas**:

- [ ] Manage Samba server file-based configuration
- [ ] Manage of Samba server registry-based configuration
- [ ] Manage of Samba configuration parameters and variables
- [ ] Understand Samba server roles and security modes
- [ ] Configure Samba to use TLS
- [ ] Check the validity of a Samba configuration
- [ ] Troubleshoot and debug configuration problems with Samba
- [ ] Understand Windows tools used to configure a Samba Server


**The following is a partial list of the used files, terms and utilities**:

- [ ] smb.conf
 - [ ] security
 - [ ] server role
 - [ ] server string
 - [ ] server services
 - [ ] tls enabled
 - [ ] tls keyfile
 - [ ] tls certfile
 - [ ] tls dh params file
 - [ ] tls cafile
 - [ ] config backend
 - [ ] registry shares
 - [ ] include
 - [ ] vfs objects

- [ ] samba-regedit
- [ ] HKLM\Software\Samba\
- [ ] REG_SZ, REG_MULTI_SZ
- [ ] testparm
- [ ] net registry (including relevant subcommands)
- [ ] Microsoft RSAT Tools
- [ ] Microsoft MMC
- [ ] Microsoft ADSI Edit
- [ ] Microsoft LDP
- [ ] Microsoft Regedit
 

### 301.3 Regular Samba Maintenance (weight: 2)

**Weight 2**

**Description**

Candidates should know the various tools and utilities that are part of a Samba installation.

**Key Knowledge Areas**:

- [ ] Start and stop Samba services on domain controllers and file servers
- [ ] Monitor and interact with running Samba daemons
- [ ] Backup and restore TDB files
- [ ] Backup and restore an Active Directory domain controller
- [ ] Understand backup and recovery strategies for Active Directory domain controllers
- [ ] Understand the impact of virtualization on Active Directory domain controllers


**The following is a partial list of the used files, terms and utilities**:

- [ ] **systemctl**
- [ ] **smbcontrol** (including relevant message types)
    - smbcontrol - send messages to smbd, nmbd or winbindd processes

- [ ] **smbstatus** `report on current Samba connections`
- [ ] **tdbbackup** `tool for backing up and for validating the integrity of samba .tdb files`
- [ ] **tdbrestore** `tool for creating a TDB file out of a tdbdump output`
- [ ] **samba-tool domain backup** `(including subcommands)`
- [ ] Virtual Machine Generation Identifier
- [ ] Virtual Machine Snapshots
 

### 301.4 Troubleshooting Samba (weight: 3)

**Weight 3**

**Description**

Candidates should be able to analyze and troubleshoot Samba issues. This includes accessing and modifying the LDAP content of a Samba server hosting an Active directory as well as working with trivial database files. Furthermore, candidates should be able to create a renamed clone of an existing Active Directory for debugging.

**Key Knowledge Areas**:

- [ ] Configure Samba logging, including setting log levels for specific debug classes and client-specific logging
- [ ] Query and modify the Samba password database
- [ ] Understand the contents of important TDB files
- [ ] List and edit TDB file content
- [ ] Identify TDB file corruption
- [ ] Access and modify objects in a Samba LDAP directory
- [ ] Enable and use the LDAP recycle bin
- [ ] Confirm the integrity of a domain controller???s database
- [ ] Create a renamed clone of a domain controller
- [ ] Awareness of Samba eventlog shipping
- [ ] Use rpcclient to query information on a Samba server


**The following is a partial list of the used files, terms and utilities**:

- [ ] **smb.conf**:
    - [ ] **log level**
    - [ ] **debuglevel**

- [ ] /var/log/samba/
- [ ] **smbpasswd** `The Samba encrypted password file | change a user's SMB password`
- [ ] **pdbedit** `manage the SAM database (Database of Samba Users)`
- [ ] **registry.tdb**
- [ ] **secrets.tdb**
- [ ] **tdbdump** `tool for printing the contents of a TDB file`
- [ ] **tdbtool** `manipulate the contents TDB files`
- [ ] **ldbsearch** `Search for records in a LDB database`
- [ ] **ldbmodify** `Modify records in a LDB database`
- [ ] **ldbedit** `Edit LDB databases using your preferred editor`
- [ ] **ldbadd** `Command-line utility for adding records to an LDB`
- [ ] **ldbdel** ` Command-line program for deleting LDB records`
- [ ] **LDIF** `LDAP Data Interchange Format`
- [ ] **samba-tool dbcheck** `Check the local AD database for errors`
- [ ] **samba-tool domain backup** `(including relevant subcommands)`

    - **domain backup**
        Create or restore a backup of the domain.

    - **domain backup offline**
        Backup (with proper locking) local domain directories into a tar file.

    - **domain backup online**
        Copy a running DC's current DB into a backup tar file.

    - **domain backup rename**
        Copy a running DC's DB to backup file, renaming the domain in the process.

    - **domain backup restore**
        Restore the domain's DB from a backup-file.


- [ ] **rpcclient** `tool for executing client side MS-RPC functions`
 

## Topic 302: Samba and Active Directory Domains

### 302.1 Samba as Active Directory Domain Controller (weight: 5)

**Weight 5**

**Description**

Candidates should be able to configure Samba as an Active Directory domain controller. This includes managing an Active Directory domain.

**Key Knowledge Areas**:

- [ ] Understand the concepts of Active Directory
- [ ] Understand the principles of the network services used by Active Directory (i.e. DNS, Kerberos, NTP and LDAP and CIFS and MS-RPC)
- [ ] Set up a new Active Directory domain using Samba
- [ ] Add a Samba domain controller to an existing Active Directory domain
- [ ] Demote and remove online and offline domain controllers
- [ ] Verify AD replication
- [ ] Understand and query the global catalog and the partial attribute set
- [ ] Understand and configure domain functional levels
- [ ] Understand and configure Active Directory forest and domain trusts
- [ ] Understand and configure Active Directory sites, including subnet assignments
- [ ] Understand and manage FSMO roles, including their impact in case of an outage
- [ ] Configure authentication audit logging
- [ ] Configure SYSVOL replication using rsync or robocopy
- [ ] Integrate Samba with ntpd
- [ ] Awareness of Windows NT4 domains


**The following is a partial list of the used files, terms and utilities**:

- [ ] smb.conf:
    - [ ] server role
    - [ ] log level

- [ ] samba-tool domain (including relevant subcommands)

    - **domain**
        Manage Domain.

    - **domain backup**
        Create or restore a backup of the domain.

    - **domain backup offline**
        Backup (with proper locking) local domain directories into a tar file.

    - **domain backup online**
        Copy a running DC's current DB into a backup tar file.

    - **domain backup rename**
        Copy a running DC's DB to backup file, renaming the domain in the process.

    - **domain backup restore**
        Restore the domain's DB from a backup-file.

    - **domain classicupgrade [options] classic_smb_conf**
        Upgrade from Samba classic (NT4-like) database to Samba AD DC database.

    - **domain dcpromo dnsdomain [DC|RODC] [options]**
        Promote an existing domain member or NT4 PDC to an AD DC.

    - **domain demote**
        Demote ourselves from the role of domain controller.

    - **domain exportkeytab keytab [options]**
        Dumps Kerberos keys of the domain into a keytab.

    - **domain info ip_address [options]**
        Print basic info about a domain and the specified DC.

    - **domain join dnsdomain [DC|RODC|MEMBER|SUBDOMAIN] [options]**
        Join a domain as either member or backup domain controller.

    - **domain level show|raise options [options]**
        Show/raise domain and forest function levels.

    - **domain passwordsettings show|set options [options]**
        Show/set password settings.

    - **domain passwordsettings pso**
        Manage fine-grained Password Settings Objects (PSOs).

    - **domain passwordsettings pso apply pso-name user-or-group-name [options]**
        Applies a PSO's password policy to a user or group.

    - **domain passwordsettings pso create pso-name precedence [options]**
        Creates a new Password Settings Object (PSO).

    - **domain passwordsettings pso delete pso-name [options]**
        Deletes a Password Settings Object (PSO).

    - **domain passwordsettings pso list [options]**
        Lists all Password Settings Objects (PSOs).

    - **domain passwordsettings pso set pso-name [options]**
        Modifies a Password Settings Object (PSO).

    - **domain passwordsettings pso show user-name [options]**
        Displays a Password Settings Object (PSO).

    - **domain passwordsettings pso show-user pso-name [options]**
        Displays the Password Settings that apply to a user.

    - **domain passwordsettings pso unapply pso-name user-or-group-name [options]**
        Updates a PSO to no longer apply to a user or group.

    - **domain provision**
        Promote an existing domain member or NT4 PDC to an AD DC.

    - **domain trust**
        Domain and forest trust management.

    - **domain trust create DOMAIN options [options]**
        Create a domain or forest trust.

    - **domain trust delete DOMAIN options [options]**
        Delete a domain trust.

    - **domain trust list options [options]**
        List domain trusts.

    - **domain trust namespaces [DOMAIN] options [options]**
        Manage forest trust namespaces.

    - **domain trust show DOMAIN options [options]**
        Show trusted domain details.

    - **domain trust validate DOMAIN options [options]**
        Validate a domain trust.



- [ ] samba-tool fsmo (including relevant subcommands)

    - **fsmo**
        Manage Flexible Single Master Operations (FSMO).

    - **fsmo seize [options]**
        Seize the role.

    - **fsmo show**
        Show the roles.

    - **fsmo transfer [options]**
           Transfer the role.


- [ ] samba-tool drs (including relevant subcommands)

    - **drs**
        Manage Directory Replication Services (DRS).

    - **drs bind**
        Show DRS capabilities of a server.

    - **drs kcc**
        Trigger knowledge consistency center run.

    - **drs options**
        Query or change options for NTDS Settings object of a domain controller.

    - **drs replicate destination_DC source_DC NC [options]**
        Replicate a naming context between two DCs.

    - **drs showrepl**
           Show replication status. The [--json] option results in JSON output, and with the [--summary] option produces very
           little output when the replication status seems healthy.

- [ ] samba-tool sites (including relevant subcommands)

    - **sites**
        Manage sites.

    - **sites create site [options]**
        Create a new site.

    - **sites remove site [options]**
           Delete an existing site.

- [ ] rsync
- [ ] rsync.conf
- [ ] /var/lib/samba/sysvol
- [ ] robocopy
- [ ] ntpd.conf
- [ ] ntpsigndsocket
 

### 302.2 Active Directory Name Resolution (weight: 2)

**Weight 2**

**Description**

Candidates should be familiar with the internal DNS server of Samba.

**Key Knowledge Areas**:

- [ ] Understand and manage DNS for Samba as an AD domain controller
- [ ] Manage DNS records in Samba DNS
- [ ] DNS forwarding
- [ ] Standardized names in an Active Directory
- [ ] Multicast DNS
- [ ] Awareness of BIND9 DLZ DNS back end
- [ ] Awareness of NetBIOS name resolution and WINS


**The following is a partial list of the used files, terms and utilities**:

- [ ] smb.conf:
    - [ ] dns forwarder
    - [ ] allow dns updates
    - [ ] multicst dns register

- [ ] **samba-tool dns** `(with subcommands)`
- [ ] **samba_dnsupdate**
- [ ] **dig**
- [ ] **host**
- [ ] /etc/resolv.conf
 

### 302.3 Active Directory User Management (weight: 4)

**Weight 4**

**Description**

Candidates should be able to manage user and group accounts on a standalone server and in a Samba based Active Directory.

**Key Knowledge Areas**:

- [ ] Manage user accounts and user group for standalone servers and Samba AD
- [ ] Knowledge of user account management tools
- [ ] Delegate administrative permissions in AD to specific users / user groups
- [ ] Configure password expiration and change requirements
- [ ] Manage password policies and password setting objects
- [ ] Understand principals and their identification SID (DN, GUID)
    - [ ] [SID](https://learn.microsoft.com/pt-br/windows-server/identity/ad-ds/manage/understand-security-identifiers)
    - [ ] [DN](https://learn.microsoft.com/en-us/previous-versions/windows/desktop/ldap/distinguished-names)
    - [ ] [GUID](https://learn.microsoft.com/pt-br/windows-server/identity/ad-ds/manage/understand-security-identifiers)
- [ ] Understand User Principal Name (UPN) and User Principal Name Suffix (UPN Suffix)
- [ ] Understand and manage Security and Distribution Groups
- [ ] Understand and manage LDAP attributes of security principals
- [ ] Understand and manage RFC2307 attributes in a Samba AD
- [ ] Map Kerberos service principal names to user accounts
- [ ] Export Kerberos keytabs for a specific principal
- [ ] Awareness of LDAP Account Manager


**The following is a partial list of the used files, terms and utilities**:

- [ ] **samba-tool user** `(including relevant subcommands)`
- [ ] **samba-tool group** `(including relevant subcommands)`
- [ ] **samba-tool domain passwordsettings**
- [ ] **samba-tool domain exportkeytab**
- [ ] **samba-tool spn** `(including relevant subcommands)`
- [ ] **smbpasswd**
- [ ] **pdbedit**
- [ ] **kinit**
- [ ] **klist**
 

### 302.4 Samba Domain Membership (weight: 4)

**Weight 4**

**Description**

Candidates should be able to join a Samba server into an existing Active Directory domain and authorize domain users to use the server. This includes installing and configuring the Winbind service.

**Key Knowledge Areas**:

- [ ] Join Samba to an existing AD domain
- [ ] Configure Winbind service, including ID mapping
- [ ] Understand and configure Winbind ID mapping, including various mapping backends
- [ ] Configure PAM and NSS to use Winbind

**The following is a partial list of the used files, terms and utilities**:

- [ ] smb.conf:
    - [ ] security
    - [ ] server role
    - [ ] realm
    - [ ] workgroup
    - [ ] idmap config
    - [ ] winbind enumerate users
    - [ ] winbind enumerate groups
    - [ ] winbind offline logon
    - [ ] winbind separator
    - [ ] template shell
    - [ ] template homedir
    - [ ] allow trusted domains

- [ ] [idmap_ad](https://www.samba.org/samba/docs/current/man-html/idmap_ad.8.html)
- [ ] [idmap_autorid](https://www.samba.org/samba/docs/current/man-html/idmap_autorid.8.html)
- [ ] [idmap_ldap](https://www.samba.org/samba/docs/current/man-html/idmap_ldap.8.html)
- [ ] [idmap_rfc2307](https://www.samba.org/samba/docs/current/man-html/idmap_rfc2307.8.html)
- [ ] [idmap_rid](https://www.samba.org/samba/docs/current/man-html/idmap_rid.8.html)
- [ ] [idmap_tdb](https://www.samba.org/samba/docs/current/man-html/idmap_tdb.8.html)
- [ ] [idmap_tdb2](https://www.samba.org/samba/docs/current/man-html/idmap_tdb2.8.html)
- [ ] [net ads](https://www.samba.org/samba/docs/current/man-html/net.8.html) (including relevant subcommands)

    - **net ads info**            Display details on remote ADS server
    - **net ads join**            Join the local machine to ADS realm
    - **net ads testjoin**        Validate machine account
    - **net ads leave**           Remove the local machine from ADS
    - **net ads status**      Display machine account details
    - **net ads user**            List/modify users
    - **net ads group**           List/modify groups
    - **net ads dns**             Issue dynamic DNS update
    - **net ads password**        Change user passwords
    - **net ads changetrustpw**   Change trust account password
    - **net ads printer**         List/modify printer entries
    - **net ads search**          Issue LDAP search using filter
    - **net ads dn**              Issue LDAP search by DN
    - **net ads sid**             Issue LDAP search by SID
    - **net ads workgroup**       Display workgroup name
    - **net ads lookup**          Perform CLDAP query on DC
    - **net ads keytab**          Manage local keytab file
    - **net ads setspn**          Manage Service Principal Names (SPN)s
    - **net ads gpo**             Manage group policy objects
    - **net ads kerberos**        Manage kerberos keytab
    - **net ads enctypes**        List/modify supported encryption types


- [ ] /etc/[nsswitch.conf](https://manpages.ubuntu.com/manpages/focal/pt/man5/nsswitch.conf.5.html)
- [ ] /etc/[pam.conf](https://man7.org/linux/man-pages/man5/pam.d.5.html)
- [ ] /etc/[pam.d](https://linux.die.net/man/5/pam.d)/
- [ ] [libnss_winbind](https://wiki.samba.org/index.php/Configuring_Winbindd_on_a_Samba_AD_DC)
- [ ] [libpam_winbind](https://www.samba.org/samba/docs/current/man-html/pam_winbind.8.html)
- [ ] [getent](https://man7.org/linux/man-pages/man1/getent.1.html)
- [ ] [wbinfo](https://www.samba.org/samba/docs/current/man-html/wbinfo.1.html) `Query information from winbind daemon`
 

### 302.5 Samba Local User Management (weight: 2)

**Weight 2**

**Description**

Candidates should be able to create and manage local user accounts on a stand alone Samba server.

**Key Knowledge Areas**:

- [ ] Setup a local password database
- [ ] Perform password synchronization
- [ ] Knowledge of different passdb backends
- [ ] Convert between Samba passdb backends


**The following is a partial list of the used files, terms and utilities**:

- [ ] smb.conf:
    - [ ] passdb backend

- [ ] /etc/passwd
- [ ] /etc/group
- [ ] pam_smbpass.so
- [ ] smbpasswd `The Samba encrypted password file | change a user's SMB password`
- [ ] pdbedit `manage the SAM database (Database of Samba Users)`
 

## Topic 303: Samba Share Configuration

### 303.1 File Share Configuration (weight: 4)

**Weight 4**

**Description**

Candidates should be able to create and configure CIFS file shares in Samba.

**Key Knowledge Areas**:

- [ ] Create and configure CIFS file shares
- [ ] Manage Samba share access configuration parameters
- [ ] Use registry based share configuration
- [ ] Manage profile and user home shares
- [ ] Plan file service migration
- [ ] Limit access to IPC$
- [ ] Awareness of user shares
- [ ] Awareness of existing VFS modules and their general functionality, including modules to support audit logs and snapshots / shadow copies


**The following is a partial list of the used files, terms and utilities**:

- [ ] smb.conf:
    - [ ] path
    - [ ] browsable
    - [ ] writable / write ok / read only
    - [ ] valid users
    - [ ] invalid users
    - [ ] read list
    - [ ] write list
    - [ ] guest ok
    - [ ] hosts allow / allow hosts
    - [ ] hosts deny / deny hosts
    - [ ] copy
    - [ ] hide unreadable
    - [ ] hide unwritable files
    - [ ] hide dot files
    - [ ] hide special files
    - [ ] veto files
    - [ ] delete veto files

- [ ] [homes]
- [ ] [IPC$]
- [ ] smbcquotas `Set or get QUOTAs of NTFS 5 shares`
 

### 303.2 File Share Security (weight: 3)

**Weight 3**

**Description**

Candidates should understand file permissions on CIFS shares and on a Linux file system.

**Key Knowledge Areas**:

- [ ] Enforce ownership and permissions of files and directories
- [ ] Manage ACLs for shares and folders
- [ ] Understand POSIX, Extended POSIX and Windows ACLs
- [ ] Understand how Samba stores Windows ACLs in Linux ACLs and extended attributes
- [ ] Configure ACLs for profile and home folder shares
- [ ] Configure encryption of CIFS connections


**The following is a partial list of the used files, terms and utilities**:

- [ ] smb.conf
    - [ ] create mask / create mode
    - [ ] directory mask / directory mode
    - [ ] force create mode
    - [ ] force directory mode
    - [ ] force user
    - [ ] force group / group
    - [ ] profile acls
    - [ ] inherit acls
    - [ ] map acl inherit
    - [ ] store dos attributes
    - [ ] vfs objects
    - [ ] smb encrypt

- [ ] chown `change file owner and group`
- [ ] chmod `change file mode bits`
- [ ] getfacl `get file access control lists`
- [ ] setfacl `set file access control lists`
- [ ] getfattr `get extended attributes of filesystem objects`
- [ ] smbcacls `Set or get ACLs on an NT file or directory names`
- [ ] sharesec `Set or get share ACLs`
- [ ] SeDiskOperatorPrivilege ``
- [ ] vfs_acl_xattr ``
- [ ] vfs_acl_tdb ``
- [ ] samba-tool ntacl (including subcommands) ``

    - **ntacl**
        Manage NT ACLs.

    - **ntacl changedomsid original-domain-SID new-domain-SID file [options]**
        Change the domain SID for ACLs. Can be used to change all entries in acl_xattr when the machine's SID has
        accidentally changed or the data set has been copied to another machine either via backup/restore or rsync.

        --use-ntvfs
            Set the ACLs directly to the TDB or xattr. The POSIX permissions will NOT be changed, only the NT ACL will be
            stored.

        --service=SERVICE
            Specify the name of the smb.conf service to use. This option is required in combination with the --use-s3fs
            option.

        --use-s3fs
            Set the ACLs for use with the default s3fs file server via the VFS layer. This option requires a smb.conf
            service, specified by the --service=SERVICE option.

        --xattr-backend=[native|tdb]
            Specify the xattr backend type (native fs or tdb).

        --eadb-file=EADB_FILE
            Name of the tdb file where attributes are stored.

        --recursive
            Set the ACLs for directories and their contents recursively.

        --follow-symlinks
            Follow symlinks when --recursive is specified.

        --verbose
            Verbosely list files and ACLs which are being processed.

    - **ntacl get file [options]**
        Get ACLs on a file.

    - **ntacl set acl file [options]**
        Set ACLs on a file.

    - **ntacl sysvolcheck**
        Check sysvol ACLs match defaults (including correct ACLs on GPOs).

    - **ntacl sysvolreset**
        Reset sysvol ACLs to defaults (including correct ACLs on GPOs).


### 303.3 DFS Share Configuration (weight: 1)

**Weight 1**

**Description**

Candidates should be able to create and manage DFS shares in Samba.

**Key Knowledge Areas**:

- [ ] Understand DFS
- [ ] Configure DFS shares


**The following is a partial list of the used files, terms and utilities**:

- [ ] smb.conf:
    - [ ] host msdfs
    - [ ] msdfs root
    - [ ] msdfs proxy

- [ ] ln
 

### 303.4 Print Share Configuration (weight: 2)

**Weight 2**

**Description**

Candidates should be able to create and manage print shares in Samba.

**Key Knowledge Areas**:

- [ ] Understand Samba printing, including raw printing
- [ ] Create and configure print shares
- [ ] Configure integration between Samba and CUPS
- [ ] Manage Windows print drivers and configure downloading of print drivers
- [ ] Upload printer drivers using 'Add Print Driver Wizard' in Windows
- [ ] Preconfigure driver settings
- [ ] Configure paper sizes and forms
- [ ] Supported driver versions
- [ ] Manage GPO options for trusted print servers
- [ ] Awareness of spoolssd

**The following is a partial list of the used files, terms and utilities**:

- [ ] smb.conf:
    - [ ] printing
    - [ ] printable / print ok
    - [ ] printcap name / printcap
    - [ ] spoolss: architecture = Windows x64

- [ ] [printers]
- [ ] [print$]
- [ ] CUPS
- [ ] cupsd.conf
- [ ] /var/spool/samba/
- [ ] smbspool
- [ ] rpcclient (to execute topic-related commands (enumdrivers, enumprinters, setdriver)
- [ ] net (included topic-related subcommands)
- [ ] SePrintOperatorPrivilege
 

## Topic 304: Samba Client Configuration

### 304.1 Linux Authentication Clients (weight: 5)

**Weight 5**

**Description**

Candidates should be familiar with management and authentication of user accounts. This includes configuration and use of NSS, PAM, SSSD and Kerberos for both local and remote directories and authentication mechanisms as well as enforcing a password policy.

**Key Knowledge Areas**:

- [ ] Understand and configure NSS and PAM
- [ ] Enforce password complexity policies and periodic password changes
- [ ] Create home directories for new users
- [ ] Lock accounts automatically after failed login attempts
- [ ] Configure NSS and PAM to retrieve information from LDAP
- [ ] Configure SSSD authentication against Active Directory, IPA, LDAP and Kerberos domains and the local system???s authentication database
- [ ] Manage local accounts through SSSD
- [ ] Obtain and manage Kerberos tickets

**The following is a partial list of the used files, terms and utilities**:

- [ ] /etc/pam.conf
- [ ] /etc/pam.d/
- [ ] /etc/nsswitch.conf
- [ ] /etc/login.defs
- [ ] pam_ldap.so
- [ ] ldap.conf
- [ ] pam_krb5.so
- [ ] pam_cracklib.so
- [ ] pam_tally2.so
- [ ] pam_faillock.so `Module counting authentication failures during a specified interval`
- [ ] pam_mkhomedir.so `pam_mkhomedir - PAM module to create users home directory`
- [ ] chage `change user password expiry information`
- [ ] faillog
- [ ] sssd
- [ ] sssd.conf
- [ ] sss_override
- [ ] sss_cache
- [ ] sss_debuglevel
- [ ] sss_user* and sss_group*
- [ ] /var/lib/sss/db/
- [ ] krb5.conf `Kerberos configuration file`
- [ ] kinit
- [ ] klist
- [ ] kdestroy
 

### 304.2 Linux CIFS Clients (weight: 3)

**Weight 3**

**Description**

Candidates should be able to use remote CIFS shares from a Linux client. This includes client-side management of CIFS credentials and managing remote ACLs and quotas.

**Key Knowledge Areas**:

- [ ] Access remote CIFS shares from a Linux client
- [ ] Mount remote CIFS shares on a Linux client
- [ ] Automatically mount home directories
- [ ] Store and manage CIFS credentials securely
- [ ] Understand and manage permissions and file ownership of remote CIFS shares
- [ ] Understand and manage quotas on CIFS shares

**The following is a partial list of the used files, terms and utilities**:

- [ ] smb.conf `The configuration file for the Samba suite`
- [ ] smbclient (including relevant subcommands) `ftp-like client to access SMB/CIFS resources on servers`
- [ ] mount `mount a filesystem`
- [ ] mount.cifs `mount using the Common Internet File System (CIFS)`
- [ ] /etc/fstab `static information about the filesystems`
- [ ] pam_mount.so
- [ ] pam_mount.conf.xml
- [ ] cifscreds `manage NTLM credentials in kernel keyring`
- [ ] getcifsacl `Userspace helper to display an ACL in a security descriptor for Common Internet File System (CIFS)`
- [ ] setcifsacl `Userspace helper to alter an ACL in a security descriptor for Common Internet File System (CIFS)`
- [ ] smbcquotas `Set or get QUOTAs of NTFS 5 shares`
- [ ] cifsiostat `Report CIFS statistics`
- [ ] smbget `wget-like utility for download files over SMB`
- [ ] smbtar `shell script for backing up SMB/CIFS shares directly to UNIX tape drives`
 

### 304.3 Windows Clients (weight: 3)

**Weight 3**

**Description**

Candidates should be able to access CIFS and print shares from Windows hosts and join such hosts into an Active Directory domain. Furthermore, candidates should be able to manage Windows hosts using GPOs and access remote Windows hosts.

**Key Knowledge Areas**:

- [ ] Understand how to set up and use Windows hosts
- [ ] Join a Windows host to an Active Directory domain
- [ ] Access remote CIFS shares from a Windows client
- [ ] Configure printing to remote printers from a Windows client
- [ ] Configure file and print shares on a Windows host
- [ ] Understand the concept, structure and capabilities of GPOs
- [ ] Create and modify GPOs and apply GPOs to machines or users
- [ ] Access a remote Windows desktop
- [ ] Create and configure logon scripts
- [ ] Configure roaming profiles for Active Directory users
- [ ] Configure profile folder redirects

**The following is a partial list of the used files, terms and utilities**:

- [ ] smb.conf:
    - [ ] logon path
    - [ ] logon script

- [ ] net (Windows command; including all relevant subcommands)
- [ ] samba-tool gpo (including all relevant subcommands)

    - **gpo**
        Manage Group Policy Objects (GPO).

    - **gpo create displayname [options]**
        Create an empty GPO.

    - **gpo del gpo [options]**
        Delete GPO.

    - **gpo dellink container_dn gpo [options]**
        Delete GPO link from a container.

    - **gpo fetch gpo [options]**
        Download a GPO.

    - **gpo getinheritance container_dn [options]**
        Get inheritance flag for a container.

    - **gpo getlink container_dn [options]**
        List GPO Links for a container.

    - **gpo list username [options]**
        List GPOs for an account.

    - **gpo listall**
        List all GPOs.

    - **gpo listcontainers gpo [options]**
        List all linked containers for a GPO.

    - **gpo setinheritance container_dn block|inherit [options]**
        Set inheritance flag on a container.

    - **gpo setlink container_dn gpo [options]**
        Add or Update a GPO link to a container.

    - **gpo show gpo [options]**
        Show information for a GPO.

    - **gpo manage symlink list**
        List VGP Symbolic Link Group Policy from the sysvol

    - **gpo manage symlink add**
        Adds a VGP Symbolic Link Group Policy to the sysvol

    - **gpo manage symlink remove**
        Removes a VGP Symbolic Link Group Policy from the sysvol

    - **gpo manage files list**
        List VGP Files Group Policy from the sysvol

    - **gpo manage files add**
        Add VGP Files Group Policy to the sysvol

    - **gpo manage files remove**
        Remove VGP Files Group Policy from the sysvol

    - **gpo manage openssh list**
        List VGP OpenSSH Group Policy from the sysvol

    - **gpo manage openssh set**
        Sets a VGP OpenSSH Group Policy to the sysvol

    - **gpo manage sudoers add**
        Adds a Samba Sudoers Group Policy to the sysvol.

    - **gpo manage sudoers list**
        List Samba Sudoers Group Policy from the sysvol.

    - **gpo manage sudoers remove**
        Removes a Samba Sudoers Group Policy from the sysvol.

    - **gpo manage scripts startup list**
        List VGP Startup Script Group Policy from the sysvol

    - **gpo manage scripts startup add**
        Adds VGP Startup Script Group Policy to the sysvol

    - **gpo manage scripts startup remove**
        Removes VGP Startup Script Group Policy from the sysvol

    - **gpo manage motd list**
        List VGP MOTD Group Policy from the sysvol.

    - **gpo manage motd set**
        Sets a VGP MOTD Group Policy to the sysvol

    - **gpo manage issue list**
        List VGP Issue Group Policy from the sysvol.

    - **gpo manage issue set**
        Sets a VGP Issue Group Policy to the sysvol

    - **gpo manage access add**
        Adds a VGP Host Access Group Policy to the sysvol

    - **gpo manage access list**
        List VGP Host Access Group Policy from the sysvol

    - **gpo manage access remove**
        Remove a VGP Host Access Group Policy from the sysvol


- [ ] gpupdate (Windows command)
- [ ] rdesktop
 

## Topic 305: Linux Identity Management and File Sharing

### 305.1 FreeIPA Installation and Maintenance (weight: 2)

**Weight 2**

**Description**

Candidates should be able to set up and manage a FreeIPA domain using standard settings and default services. This includes setting up replication and joining clients to the domain.

**Key Knowledge Areas**:

- [ ] Understand the features, architecture as well as server-side and client-side components of FreeIPA
- [ ] Install a FreeIPA server
- [ ] Set up and manage a FreeIPA domain using standard settings and default services
- [ ] Understand replication topology and configure FreeIPA replication
- [ ] Join clients to an existing FreeIPA domain
- [ ] Awareness of ipa-backup

**The following is a partial list of the used files, terms and utilities**:

- [ ] ipa-server-install
- [ ] ipa-replica-prepare
- [ ] ipa-replica-install
- [ ] ipa-client-install
- [ ] ipactl
 

### 305.2 FreeIPA Entity Management (weight: 4)

**Weight 4**

**Description**

Candidates should be able manage users, hosts and services in a FreeIPA domain.

**Key Knowledge Areas**:

- [ ] Manage user accounts and groups
- [ ] Manage hosts, hostgroups and services
- [ ] Understand the principle of IPA access control permissions, privileges and roles
- [ ] Understand ID views
- [ ] Awareness of sudo, autofs, SSH, SELinux and NIS integration as well as host based access control in FreeIPA
- [ ] Awareness of the FreeIPA CA


**The following is a partial list of the used files, terms and utilities**:

- [ ] ipa (including relevant user-, stageuser- and group- and idview- subcommands)
- [ ] ipa (including relevant host-, hostgroup-, service- and getkeytab subcommands)
- [ ] ipa (including relevant permission-, privilege-, and role- subcommands)
- [ ] ipctl
- [ ] ipa-advice
 

### 305.3 FreeIPA Active Directory Integration (weight: 2)

**Weight 2**

**Description**

Candidates should be able to set up a cross-forest trust between a FreeIPA and an Active Directory domain.

**Key Knowledge Areas**:

- [ ] Understand and set up FreeIPA and Active Directory integration using Kerberos cross-realm trusts
- [ ] Configure ID ranges in FreeIPA
- [ ] Understand and manage external non-POSIX groups in FreeIPA
- [ ] Awareness of Microsoft Privilege Attribute Certificates and how they are handled by FreeIPA
- [ ] Awareness of replication based FreeIPA and Active Directory integration


**The following is a partial list of the used files, terms and utilities**:

- [ ] ipa-adtrust-install
- [ ] ipa (including relevant trust-*, idrange-* and group-* subcommands)
 

### 305.4 Network File System (weight: 3)

**Weight 3**

**Description**

Candidates should be able to use NFSv4. This includes understanding ID mapping, NFSv4 ACLs and Kerberos authentication for NFS.

**Key Knowledge Areas**:

- [ ] Understand major NFSv4 features
- [ ] Configure and manage an NFSv4 server and clients
- [ ] Understand and use the NFSv4 pseudo file system
- [ ] Understand and use NFSv4 ACLs
- [ ] Use Kerberos for for NFSv4 authentication  


**The following is a partial list of the used files, terms and utilities**:

- [ ] exportfs
- [ ] /etc/exports
- [ ] /etc/idmapd.conf
- [ ] nfs4_editfacl
- [ ] nfs4_getfacl
- [ ] nfs4_setfacl
- [ ] mount (including common NFS mount options)
- [ ] /etc/fstab
