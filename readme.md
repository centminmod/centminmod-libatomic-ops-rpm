```
rpm -qa --changelog centmin-libatomic_ops
* Thu Dec 30 2021 George Liu <centminmod.com> 7.6.12
- libatomic_ops-7.6.12 for centminmod.com LEMP stack libatomic_ops-7.6.12
```
```
yum -q info centmin-libatomic_ops-7.6.12
Installed Packages
Name        : centmin-libatomic_ops
Arch        : x86_64
Version     : 7.6.12
Release     : 1.el7
Size        : 713 k
Repo        : installed
From repo   : /centmin-libatomic_ops-7.6.12-1.el7.x86_64
Summary     : libatomic_ops-7.6.12 for centminmod.com LEMP stack libatomic_ops-7.6.12
URL         : https://centminmod.com
License     : unknown
Description : libatomic_ops-7.6.12 for centminmod.com LEMP stacks
```

For PREFIX=/usr/local/nginx-dep version

```
PKG_CONFIG_PATH='/usr/local/nginx-dep/lib/pkgconfig/' pkg-config atomic_ops --libs
-L/usr/local/nginx-dep/lib -latomic_ops  

PKG_CONFIG_PATH='/usr/local/nginx-dep/lib/pkgconfig/' pkg-config atomic_ops --cflags
-I/usr/local/nginx-dep/include  

PKG_CONFIG_PATH='/usr/local/nginx-dep/lib/pkgconfig/' pkg-config --modversion  atomic_ops
7.6.12
```
```
rpm -ql centmin-libatomic_ops-7.6.12
/usr/local/nginx-dep/include/atomic_ops.h
/usr/local/nginx-dep/include/atomic_ops/ao_version.h
/usr/local/nginx-dep/include/atomic_ops/generalize-arithm.h
/usr/local/nginx-dep/include/atomic_ops/generalize-small.h
/usr/local/nginx-dep/include/atomic_ops/generalize.h
/usr/local/nginx-dep/include/atomic_ops/sysdeps/all_acquire_release_volatile.h
/usr/local/nginx-dep/include/atomic_ops/sysdeps/all_aligned_atomic_load_store.h
/usr/local/nginx-dep/include/atomic_ops/sysdeps/all_atomic_load_store.h
/usr/local/nginx-dep/include/atomic_ops/sysdeps/all_atomic_only_load.h
/usr/local/nginx-dep/include/atomic_ops/sysdeps/ao_t_is_int.h
/usr/local/nginx-dep/include/atomic_ops/sysdeps/armcc/arm_v6.h
/usr/local/nginx-dep/include/atomic_ops/sysdeps/emul_cas.h
/usr/local/nginx-dep/include/atomic_ops/sysdeps/gcc/aarch64.h
/usr/local/nginx-dep/include/atomic_ops/sysdeps/gcc/alpha.h
/usr/local/nginx-dep/include/atomic_ops/sysdeps/gcc/arm.h
/usr/local/nginx-dep/include/atomic_ops/sysdeps/gcc/avr32.h
/usr/local/nginx-dep/include/atomic_ops/sysdeps/gcc/cris.h
/usr/local/nginx-dep/include/atomic_ops/sysdeps/gcc/generic-arithm.h
/usr/local/nginx-dep/include/atomic_ops/sysdeps/gcc/generic-small.h
/usr/local/nginx-dep/include/atomic_ops/sysdeps/gcc/generic.h
/usr/local/nginx-dep/include/atomic_ops/sysdeps/gcc/hexagon.h
/usr/local/nginx-dep/include/atomic_ops/sysdeps/gcc/hppa.h
/usr/local/nginx-dep/include/atomic_ops/sysdeps/gcc/ia64.h
/usr/local/nginx-dep/include/atomic_ops/sysdeps/gcc/m68k.h
/usr/local/nginx-dep/include/atomic_ops/sysdeps/gcc/mips.h
/usr/local/nginx-dep/include/atomic_ops/sysdeps/gcc/powerpc.h
/usr/local/nginx-dep/include/atomic_ops/sysdeps/gcc/riscv.h
/usr/local/nginx-dep/include/atomic_ops/sysdeps/gcc/s390.h
/usr/local/nginx-dep/include/atomic_ops/sysdeps/gcc/sh.h
/usr/local/nginx-dep/include/atomic_ops/sysdeps/gcc/sparc.h
/usr/local/nginx-dep/include/atomic_ops/sysdeps/gcc/tile.h
/usr/local/nginx-dep/include/atomic_ops/sysdeps/gcc/x86.h
/usr/local/nginx-dep/include/atomic_ops/sysdeps/generic_pthread.h
/usr/local/nginx-dep/include/atomic_ops/sysdeps/hpc/hppa.h
/usr/local/nginx-dep/include/atomic_ops/sysdeps/hpc/ia64.h
/usr/local/nginx-dep/include/atomic_ops/sysdeps/ibmc/powerpc.h
/usr/local/nginx-dep/include/atomic_ops/sysdeps/icc/ia64.h
/usr/local/nginx-dep/include/atomic_ops/sysdeps/loadstore/acquire_release_volatile.h
/usr/local/nginx-dep/include/atomic_ops/sysdeps/loadstore/atomic_load.h
/usr/local/nginx-dep/include/atomic_ops/sysdeps/loadstore/atomic_store.h
/usr/local/nginx-dep/include/atomic_ops/sysdeps/loadstore/char_acquire_release_volatile.h
/usr/local/nginx-dep/include/atomic_ops/sysdeps/loadstore/char_atomic_load.h
/usr/local/nginx-dep/include/atomic_ops/sysdeps/loadstore/char_atomic_store.h
/usr/local/nginx-dep/include/atomic_ops/sysdeps/loadstore/double_atomic_load_store.h
/usr/local/nginx-dep/include/atomic_ops/sysdeps/loadstore/int_acquire_release_volatile.h
/usr/local/nginx-dep/include/atomic_ops/sysdeps/loadstore/int_atomic_load.h
/usr/local/nginx-dep/include/atomic_ops/sysdeps/loadstore/int_atomic_store.h
/usr/local/nginx-dep/include/atomic_ops/sysdeps/loadstore/ordered_loads_only.h
/usr/local/nginx-dep/include/atomic_ops/sysdeps/loadstore/ordered_stores_only.h
/usr/local/nginx-dep/include/atomic_ops/sysdeps/loadstore/short_acquire_release_volatile.h
/usr/local/nginx-dep/include/atomic_ops/sysdeps/loadstore/short_atomic_load.h
/usr/local/nginx-dep/include/atomic_ops/sysdeps/loadstore/short_atomic_store.h
/usr/local/nginx-dep/include/atomic_ops/sysdeps/msftc/arm.h
/usr/local/nginx-dep/include/atomic_ops/sysdeps/msftc/common32_defs.h
/usr/local/nginx-dep/include/atomic_ops/sysdeps/msftc/x86.h
/usr/local/nginx-dep/include/atomic_ops/sysdeps/msftc/x86_64.h
/usr/local/nginx-dep/include/atomic_ops/sysdeps/ordered.h
/usr/local/nginx-dep/include/atomic_ops/sysdeps/ordered_except_wr.h
/usr/local/nginx-dep/include/atomic_ops/sysdeps/read_ordered.h
/usr/local/nginx-dep/include/atomic_ops/sysdeps/standard_ao_double_t.h
/usr/local/nginx-dep/include/atomic_ops/sysdeps/sunc/sparc.h
/usr/local/nginx-dep/include/atomic_ops/sysdeps/sunc/x86.h
/usr/local/nginx-dep/include/atomic_ops/sysdeps/test_and_set_t_is_ao_t.h
/usr/local/nginx-dep/include/atomic_ops/sysdeps/test_and_set_t_is_char.h
/usr/local/nginx-dep/include/atomic_ops_malloc.h
/usr/local/nginx-dep/include/atomic_ops_stack.h
/usr/local/nginx-dep/lib/libatomic_ops.a
/usr/local/nginx-dep/lib/libatomic_ops.la
/usr/local/nginx-dep/lib/libatomic_ops.so
/usr/local/nginx-dep/lib/libatomic_ops.so.1
/usr/local/nginx-dep/lib/libatomic_ops.so.1.1.1
/usr/local/nginx-dep/lib/libatomic_ops_gpl.a
/usr/local/nginx-dep/lib/libatomic_ops_gpl.la
/usr/local/nginx-dep/lib/libatomic_ops_gpl.so
/usr/local/nginx-dep/lib/libatomic_ops_gpl.so.1
/usr/local/nginx-dep/lib/libatomic_ops_gpl.so.1.1.2
/usr/local/nginx-dep/lib/pkgconfig/atomic_ops.pc
```

For PREFIX=/usr/local version

```
PKG_CONFIG_PATH='/usr/local/lib/pkgconfig/' pkg-config atomic_ops --libs
-L/usr/local/lib -latomic_ops  

PKG_CONFIG_PATH='/usr/local/lib/pkgconfig/' pkg-config atomic_ops --cflags
-I/usr/local/include  

PKG_CONFIG_PATH='/usr/local/lib/pkgconfig/' pkg-config --modversion  atomic_ops
7.6.12
```
```
rpm -ql centmin-libatomic_ops-7.6.12
/usr/local/include/atomic_ops.h
/usr/local/include/atomic_ops/ao_version.h
/usr/local/include/atomic_ops/generalize-arithm.h
/usr/local/include/atomic_ops/generalize-small.h
/usr/local/include/atomic_ops/generalize.h
/usr/local/include/atomic_ops/sysdeps/all_acquire_release_volatile.h
/usr/local/include/atomic_ops/sysdeps/all_aligned_atomic_load_store.h
/usr/local/include/atomic_ops/sysdeps/all_atomic_load_store.h
/usr/local/include/atomic_ops/sysdeps/all_atomic_only_load.h
/usr/local/include/atomic_ops/sysdeps/ao_t_is_int.h
/usr/local/include/atomic_ops/sysdeps/armcc/arm_v6.h
/usr/local/include/atomic_ops/sysdeps/emul_cas.h
/usr/local/include/atomic_ops/sysdeps/gcc/aarch64.h
/usr/local/include/atomic_ops/sysdeps/gcc/alpha.h
/usr/local/include/atomic_ops/sysdeps/gcc/arm.h
/usr/local/include/atomic_ops/sysdeps/gcc/avr32.h
/usr/local/include/atomic_ops/sysdeps/gcc/cris.h
/usr/local/include/atomic_ops/sysdeps/gcc/generic-arithm.h
/usr/local/include/atomic_ops/sysdeps/gcc/generic-small.h
/usr/local/include/atomic_ops/sysdeps/gcc/generic.h
/usr/local/include/atomic_ops/sysdeps/gcc/hexagon.h
/usr/local/include/atomic_ops/sysdeps/gcc/hppa.h
/usr/local/include/atomic_ops/sysdeps/gcc/ia64.h
/usr/local/include/atomic_ops/sysdeps/gcc/m68k.h
/usr/local/include/atomic_ops/sysdeps/gcc/mips.h
/usr/local/include/atomic_ops/sysdeps/gcc/powerpc.h
/usr/local/include/atomic_ops/sysdeps/gcc/riscv.h
/usr/local/include/atomic_ops/sysdeps/gcc/s390.h
/usr/local/include/atomic_ops/sysdeps/gcc/sh.h
/usr/local/include/atomic_ops/sysdeps/gcc/sparc.h
/usr/local/include/atomic_ops/sysdeps/gcc/tile.h
/usr/local/include/atomic_ops/sysdeps/gcc/x86.h
/usr/local/include/atomic_ops/sysdeps/generic_pthread.h
/usr/local/include/atomic_ops/sysdeps/hpc/hppa.h
/usr/local/include/atomic_ops/sysdeps/hpc/ia64.h
/usr/local/include/atomic_ops/sysdeps/ibmc/powerpc.h
/usr/local/include/atomic_ops/sysdeps/icc/ia64.h
/usr/local/include/atomic_ops/sysdeps/loadstore/acquire_release_volatile.h
/usr/local/include/atomic_ops/sysdeps/loadstore/atomic_load.h
/usr/local/include/atomic_ops/sysdeps/loadstore/atomic_store.h
/usr/local/include/atomic_ops/sysdeps/loadstore/char_acquire_release_volatile.h
/usr/local/include/atomic_ops/sysdeps/loadstore/char_atomic_load.h
/usr/local/include/atomic_ops/sysdeps/loadstore/char_atomic_store.h
/usr/local/include/atomic_ops/sysdeps/loadstore/double_atomic_load_store.h
/usr/local/include/atomic_ops/sysdeps/loadstore/int_acquire_release_volatile.h
/usr/local/include/atomic_ops/sysdeps/loadstore/int_atomic_load.h
/usr/local/include/atomic_ops/sysdeps/loadstore/int_atomic_store.h
/usr/local/include/atomic_ops/sysdeps/loadstore/ordered_loads_only.h
/usr/local/include/atomic_ops/sysdeps/loadstore/ordered_stores_only.h
/usr/local/include/atomic_ops/sysdeps/loadstore/short_acquire_release_volatile.h
/usr/local/include/atomic_ops/sysdeps/loadstore/short_atomic_load.h
/usr/local/include/atomic_ops/sysdeps/loadstore/short_atomic_store.h
/usr/local/include/atomic_ops/sysdeps/msftc/arm.h
/usr/local/include/atomic_ops/sysdeps/msftc/common32_defs.h
/usr/local/include/atomic_ops/sysdeps/msftc/x86.h
/usr/local/include/atomic_ops/sysdeps/msftc/x86_64.h
/usr/local/include/atomic_ops/sysdeps/ordered.h
/usr/local/include/atomic_ops/sysdeps/ordered_except_wr.h
/usr/local/include/atomic_ops/sysdeps/read_ordered.h
/usr/local/include/atomic_ops/sysdeps/standard_ao_double_t.h
/usr/local/include/atomic_ops/sysdeps/sunc/sparc.h
/usr/local/include/atomic_ops/sysdeps/sunc/x86.h
/usr/local/include/atomic_ops/sysdeps/test_and_set_t_is_ao_t.h
/usr/local/include/atomic_ops/sysdeps/test_and_set_t_is_char.h
/usr/local/include/atomic_ops_malloc.h
/usr/local/include/atomic_ops_stack.h
/usr/local/lib/libatomic_ops.a
/usr/local/lib/libatomic_ops.la
/usr/local/lib/libatomic_ops.so
/usr/local/lib/libatomic_ops.so.1
/usr/local/lib/libatomic_ops.so.1.1.1
/usr/local/lib/libatomic_ops_gpl.a
/usr/local/lib/libatomic_ops_gpl.la
/usr/local/lib/libatomic_ops_gpl.so
/usr/local/lib/libatomic_ops_gpl.so.1
/usr/local/lib/libatomic_ops_gpl.so.1.1.2
/usr/local/lib/pkgconfig/atomic_ops.pc
```