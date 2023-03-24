# Copyright (c) 2023 Intel Corporation
# SPDX-License-Identifier: Apache-2.0

zephyr_library()
zephyr_library_sources_ifdef(CONFIG_DT_HAS_INTEL_AGILEX_SOCFPGA_SIP_SMC_ENABLED sip_smc_intel_socfpga.c)
