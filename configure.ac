m4_define(jw_boot_logo_triplet, m4_esyscmd_s([cat version.txt]))
m4_define(jw_boot_log_list, m4_split(jw_boot_log_triplet, [[.]]))
m4_define(jw_boot_log_major, m4_argn(1, jw_boot_log_list))
m4_define(jw_boot_log_minor, m4_argn(2, jw_boot_log_list))
m4_define(jw_boot_log_patch, m4_argn(3, jw_boot_log_list))

AC_INIT([JW Boot Logo], [jw_boot_log_triplet])

AC_PROG_CXX
AC_CONFIG_MACRO_DIRS([m4])
AM_INIT_AUTOMAKE([foreign])

AC_SUBST([JW_BOOT_LOG_VERSION], jw_boot_log_triplet)

AC_CONFIG_FILES([Makefile])
AM_SILENT_RULES([yes])
AC_OUTPUT
