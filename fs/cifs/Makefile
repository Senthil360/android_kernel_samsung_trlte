#
# Makefile for Linux CIFS VFS client 
#
CFLAGS_asn1.o := -fno-strict-aliasing
CFLAGS_cifs.o := -fno-strict-aliasing
CFLAGS_cifsfs.o := -fno-strict-aliasing
CFLAGS_cifssmb.o := -fno-strict-aliasing
CFLAGS_cifs_debug.o := -fno-strict-aliasing
CFLAGS_connect.o := -fno-strict-aliasing
CFLAGS_dir.o := -fno-strict-aliasing
CFLAGS_file.o := -fno-strict-aliasing
CFLAGS_inode.o := -fno-strict-aliasing
CFLAGS_link.o := -fno-strict-aliasing
CFLAGS_transport.o := -fno-strict-aliasing
CFLAGS_cifs_unicode.o := -fno-strict-aliasing
CFLAGS_xattr.o := -fno-strict-aliasing
CFLAGS_cifsencrypt.o := -fno-strict-aliasing
CFLAGS_misc.o := -fno-strict-aliasing
CFLAGS_netmisc.o := -fno-strict-aliasing
CFLAGS_smbencrypt.o := -fno-strict-aliasing
CFLAGS_readdir.o := -fno-strict-aliasing
CFLAGS_ioctl.o := -fno-strict-aliasing
CFLAGS_sess.o := -fno-strict-aliasing
CFLAGS_export.o := -fno-strict-aliasing
CFLAGS_smb1ops.o := -fno-strict-aliasing
obj-$(CONFIG_CIFS) += cifs.o

cifs-y := cifsfs.o cifssmb.o cifs_debug.o connect.o dir.o file.o inode.o \
	  link.o misc.o netmisc.o smbencrypt.o transport.o asn1.o \
	  cifs_unicode.o nterr.o xattr.o cifsencrypt.o \
	  readdir.o ioctl.o sess.o export.o smb1ops.o

cifs-$(CONFIG_CIFS_ACL) += cifsacl.o

cifs-$(CONFIG_CIFS_UPCALL) += cifs_spnego.o

cifs-$(CONFIG_CIFS_DFS_UPCALL) += dns_resolve.o cifs_dfs_ref.o

cifs-$(CONFIG_CIFS_FSCACHE) += fscache.o cache.o

cifs-$(CONFIG_CIFS_SMB2) += smb2ops.o smb2maperror.o smb2transport.o \
			    smb2misc.o smb2pdu.o smb2inode.o smb2file.o
