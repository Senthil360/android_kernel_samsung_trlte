CFLAGS_zcache-main.o := -fno-strict-aliasing
zcache-y	:=		zcache-main.o tmem.o zbud.o
zcache-$(CONFIG_ZCACHE_DEBUG) += debug.o
zcache-$(CONFIG_RAMSTER_DEBUG) += ramster/debug.o
zcache-$(CONFIG_RAMSTER)	+=	ramster/ramster.o ramster/r2net.o
zcache-$(CONFIG_RAMSTER)	+=	ramster/nodemanager.o ramster/tcp.o
zcache-$(CONFIG_RAMSTER)	+=	ramster/heartbeat.o ramster/masklog.o

obj-$(CONFIG_ZCACHE)	+=	zcache.o
