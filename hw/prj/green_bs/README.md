## FPGA project for partial-reconfiguration default AFU design, depending on exported PR FIM design.

call stack:
>   ```bash
>    make build-bin -> run_proj.tcl -> export_role.tcl -> ../../src/ipi/afu_default.bd.tcl
>   ```

To generate a Green Bitstream based on imported dcp and wrapper files from [../blue_bs](../blue_bs) project
>
>   ```bash
>    make build-bin AFU_SRC_FILE=../../src/afu_customize/hls_ip/adder_axilite/afu_example.bd.tcl AFU_IP_FILE=../../src/afu_customize/hls_ip/adder_axilite/add_afu_ip_path.tcl
>   ```
