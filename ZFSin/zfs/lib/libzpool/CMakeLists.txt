set(MODULE_DIR "../../module")

add_library(libzpool
	"${MODULE_DIR}/lua/lapi.c"
    "${MODULE_DIR}/lua/lauxlib.c"
    "${MODULE_DIR}/lua/lbaselib.c"
    "${MODULE_DIR}/lua/lbitlib.c"
    "${MODULE_DIR}/lua/lcode.c"
    "${MODULE_DIR}/lua/lcompat.c"
    "${MODULE_DIR}/lua/lcorolib.c"
    "${MODULE_DIR}/lua/lctype.c"
    "${MODULE_DIR}/lua/ldebug.c"
    "${MODULE_DIR}/lua/ldo.c"
    "${MODULE_DIR}/lua/ldump.c"
    "${MODULE_DIR}/lua/lfunc.c"
    "${MODULE_DIR}/lua/lgc.c"
    "${MODULE_DIR}/lua/llex.c"
    "${MODULE_DIR}/lua/lmem.c"
    "${MODULE_DIR}/lua/lobject.c"
    "${MODULE_DIR}/lua/lopcodes.c"
    "${MODULE_DIR}/lua/lparser.c"
    "${MODULE_DIR}/lua/lstate.c"
    "${MODULE_DIR}/lua/lstring.c"
    "${MODULE_DIR}/lua/lstrlib.c"
    "${MODULE_DIR}/lua/ltable.c"
    "${MODULE_DIR}/lua/ltablib.c"
    "${MODULE_DIR}/lua/ltm.c"
    "${MODULE_DIR}/lua/lundump.c"
    "${MODULE_DIR}/lua/lvm.c"
    "${MODULE_DIR}/lua/lzio.c"
    "${MODULE_DIR}/zcommon/zfs_comutil.c"
    "${MODULE_DIR}/zcommon/zfs_deleg.c"
    "${MODULE_DIR}/zcommon/zfs_fletcher.c"
    "${MODULE_DIR}/zcommon/zfs_namecheck.c"
    "${MODULE_DIR}/zcommon/zfs_prop.c"
    "${MODULE_DIR}/zcommon/zfs_uio.c"
    "${MODULE_DIR}/zcommon/zpool_prop.c"
    "${MODULE_DIR}/zcommon/zprop_common.c"
    "${MODULE_DIR}/zfs/abd.c"
    "${MODULE_DIR}/zfs/aggsum.c"
    "${MODULE_DIR}/zfs/arc.c"
    "${MODULE_DIR}/zfs/blkptr.c"
    "${MODULE_DIR}/zfs/bplist.c"
    "${MODULE_DIR}/zfs/bpobj.c"
    "${MODULE_DIR}/zfs/bptree.c"
    "${MODULE_DIR}/zfs/bqueue.c"
    "${MODULE_DIR}/zfs/cityhash.c"
    "${MODULE_DIR}/zfs/dbuf.c"
    "${MODULE_DIR}/zfs/dbuf_stats.c"
    "${MODULE_DIR}/zfs/ddt.c"
    "${MODULE_DIR}/zfs/ddt_zap.c"
    "${MODULE_DIR}/zfs/dmu.c"
    "${MODULE_DIR}/zfs/dmu_diff.c"
    "${MODULE_DIR}/zfs/dmu_object.c"
    "${MODULE_DIR}/zfs/dmu_objset.c"
    "${MODULE_DIR}/zfs/dmu_recv.c"
    "${MODULE_DIR}/zfs/dmu_send.c"
    "${MODULE_DIR}/zfs/dmu_traverse.c"
    "${MODULE_DIR}/zfs/dmu_tx.c"
    "${MODULE_DIR}/zfs/dmu_zfetch.c"
    "${MODULE_DIR}/zfs/dnode.c"
    "${MODULE_DIR}/zfs/dnode_sync.c"
    "${MODULE_DIR}/zfs/dsl_bookmark.c"
    "${MODULE_DIR}/zfs/dsl_crypt.c"
    "${MODULE_DIR}/zfs/dsl_dataset.c"
    "${MODULE_DIR}/zfs/dsl_deadlist.c"
    "${MODULE_DIR}/zfs/dsl_deleg.c"
    "${MODULE_DIR}/zfs/dsl_destroy.c"
    "${MODULE_DIR}/zfs/dsl_dir.c"
    "${MODULE_DIR}/zfs/dsl_pool.c"
    "${MODULE_DIR}/zfs/dsl_proc.c"
    "${MODULE_DIR}/zfs/dsl_prop.c"
    "${MODULE_DIR}/zfs/dsl_scan.c"
    "${MODULE_DIR}/zfs/dsl_synctask.c"
    "${MODULE_DIR}/zfs/dsl_userhold.c"
    "${MODULE_DIR}/zfs/edonr_zfs.c"
    "${MODULE_DIR}/zfs/fm.c"
    "${MODULE_DIR}/zfs/gzip.c"
    "${MODULE_DIR}/zfs/hkdf.c"
    "${MODULE_DIR}/zfs/lz4.c"
    "${MODULE_DIR}/zfs/lzjb.c"
    "${MODULE_DIR}/zfs/metaslab.c"
    "${MODULE_DIR}/zfs/mmp.c"
    "${MODULE_DIR}/zfs/multilist.c"
    "${MODULE_DIR}/zfs/range_tree.c"
    "${MODULE_DIR}/zfs/refcount.c"
    "${MODULE_DIR}/zfs/rrwlock.c"
    "${MODULE_DIR}/zfs/sa.c"
    "${MODULE_DIR}/zfs/sha256.c"
    "${MODULE_DIR}/zfs/skein_zfs.c"
    "${MODULE_DIR}/zfs/spa.c"
    "${MODULE_DIR}/zfs/space_map.c"
    "${MODULE_DIR}/zfs/space_reftree.c"
    "${MODULE_DIR}/zfs/spa_boot.c"
    "${MODULE_DIR}/zfs/spa_checkpoint.c"
    "${MODULE_DIR}/zfs/spa_config.c"
    "${MODULE_DIR}/zfs/spa_errlog.c"
    "${MODULE_DIR}/zfs/spa_history.c"
    "${MODULE_DIR}/zfs/spa_misc.c"
    "${MODULE_DIR}/zfs/spa_stats.c"
    "${MODULE_DIR}/zfs/txg.c"
    "${MODULE_DIR}/zfs/uberblock.c"
    "${MODULE_DIR}/zfs/unique.c"
    "${MODULE_DIR}/zfs/vdev.c"
    "${MODULE_DIR}/zfs/vdev_cache.c"
    "${MODULE_DIR}/zfs/vdev_file.c"
    "${MODULE_DIR}/zfs/vdev_indirect.c"
    "${MODULE_DIR}/zfs/vdev_indirect_births.c"
    "${MODULE_DIR}/zfs/vdev_indirect_mapping.c"
    "${MODULE_DIR}/zfs/vdev_initialize.c"
    "${MODULE_DIR}/zfs/vdev_label.c"
    "${MODULE_DIR}/zfs/vdev_mirror.c"
    "${MODULE_DIR}/zfs/vdev_missing.c"
    "${MODULE_DIR}/zfs/vdev_queue.c"
    "${MODULE_DIR}/zfs/vdev_raidz.c"
    "${MODULE_DIR}/zfs/vdev_removal.c"
    "${MODULE_DIR}/zfs/vdev_root.c"
    "${MODULE_DIR}/zfs/vdev_trim.c"
    "${MODULE_DIR}/zfs/zap.c"
    "${MODULE_DIR}/zfs/zap_leaf.c"
    "${MODULE_DIR}/zfs/zap_micro.c"
    "${MODULE_DIR}/zfs/zcp.c"
    "${MODULE_DIR}/zfs/zcp_get.c"
    "${MODULE_DIR}/zfs/zcp_global.c"
    "${MODULE_DIR}/zfs/zcp_iter.c"
    "${MODULE_DIR}/zfs/zcp_synctask.c"
    "${MODULE_DIR}/zfs/zfeature.c"
    "${MODULE_DIR}/zfs/zfeature_common.c"
    "${MODULE_DIR}/zfs/zfs_byteswap.c"
    "${MODULE_DIR}/zfs/zfs_debug.c"
    "${MODULE_DIR}/zfs/zfs_fm.c"
    "${MODULE_DIR}/zfs/zfs_fuid.c"
    "${MODULE_DIR}/zfs/zfs_sa.c"
    "${MODULE_DIR}/zfs/zfs_znode.c"
    "${MODULE_DIR}/zfs/zil.c"
    "${MODULE_DIR}/zfs/zio.c"
    "${MODULE_DIR}/zfs/zio_checksum.c"
    "${MODULE_DIR}/zfs/zio_compress.c"
    "${MODULE_DIR}/zfs/zio_crypt.c"
    "${MODULE_DIR}/zfs/zio_inject.c"
    "${MODULE_DIR}/zfs/zle.c"
    "${MODULE_DIR}/zfs/zrlock.c"
    "${MODULE_DIR}/zfs/zthr.c"
    "kernel.c"
    "taskq.c"
    "util.c"
)
target_link_libraries(libzpool PUBLIC
	libicp
	libnvpair
	libunicode
	libuutil
	libpthread
	libavl
	libefi
	libshare
	zlib
)