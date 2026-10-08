mkdir -p .repo/local_manifests

  cat > .repo/local_manifests/roomservice.xml
  << 'EOF'
  <?xml version="1.0" encoding="UTF-8"?>
<manifest>

  <!-- Device + Vendor -->
  <project name="galaxy-m55xq/android_device_samsung_m55xq" path="device/samsung/m55xq" remote="github" revision="lineage-23.2" />
  <project name="galaxy-m55xq/android_vendor_samsung_m55xq" path="vendor/samsung/m55xq" remote="github" revision="M556BXXS5DZF2" />
  <project name="LineageOS/android_hardware_samsung" path="hardware/samsung" remote="github" revision="lineage-23.2" />

  <!-- ======================== -->
  <!-- QCOM CAF - Audio (Taro)  -->
  <!-- ======================== -->
  <project path="hardware/qcom-caf/sm8450/audio/agm"
           name="LineageOS/android_vendor_qcom_opensource_agm"
           remote="github"
           revision="lineage-23.2-caf-sm8450" />

  <project path="hardware/qcom-caf/sm8450/audio/pal"
           name="LineageOS/android_vendor_qcom_opensource_arpal-lx"
           remote="github"
           revision="lineage-23.2-caf-sm8450" />

  <project path="hardware/qcom-caf/sm8450/audio/primary-hal"
           name="LineageOS/android_hardware_qcom_audio-ar"
           remote="github"
           revision="lineage-23.2-caf-sm8450" />

  <project path="hardware/qcom-caf/sm8450/audio/graphservices"
           name="LineageOS/android_vendor_qcom_opensource_audioreach-graphservices"
           remote="github"
           revision="lineage-23.2-caf-sm8450" />

  <!-- ======================== -->
  <!-- QCOM CAF - Display       -->
  <!-- ======================== -->
  <project path="hardware/qcom-caf/sm8450/display"
           name="LineageOS/android_hardware_qcom_display"
           remote="github"
           revision="lineage-23.2-caf-sm8450" />

  <!-- ======================== -->
  <!-- QCOM CAF - Data / IPA    -->
  <!-- ======================== -->
  <project path="hardware/qcom-caf/sm8450/data-ipa-cfg-mgr"
           name="LineageOS/android_vendor_qcom_opensource_data-ipa-cfg-mgr"
           remote="github"
           revision="lineage-23.2-caf-sm8450" />

  <!-- ======================== -->
  <!-- QCOM Opensource HALs     -->
  <!-- ======================== -->
  <project path="vendor/qcom/opensource/power"
           name="LineageOS/android_vendor_qcom_opensource_power"
           remote="github"
           revision="lineage-23.2" />

  <project path="vendor/qcom/opensource/vibrator"
           name="LineageOS/android_vendor_qcom_opensource_vibrator"
           remote="github"
           revision="lineage-23.2" />

  <project path="vendor/qcom/opensource/usb"
           name="LineageOS/android_vendor_qcom_opensource_usb"
           remote="github"
           revision="lineage-23.2" />

  <project path="vendor/qcom/opensource/thermal-engine"
           name="LineageOS/android_vendor_qcom_opensource_thermal-engine"
           remote="github"
           revision="lineage-23.2" />

  <project path="vendor/qcom/opensource/interfaces"
           name="LineageOS/android_vendor_qcom_opensource_interfaces"
           remote="github"
           revision="lineage-23.2" />

  <!-- Sound Trigger (needed for PAL/AGM audio) -->
  <project path="vendor/qcom/opensource/audio-hal/st-hal-ar"
           name="LineageOS/android_vendor_qcom_opensource_audio-hal_st-hal-ar"
           remote="github"
           revision="lineage-23.2" />

  <!-- WLAN HAL -->
  <project path="hardware/qcom-caf/wlan"
           name="LineageOS/android_hardware_qcom_wlan"
           remote="github"
           revision="lineage-23.2-caf" />

  <!-- SEPolicy for sm8450 family -->
  <project path="device/qcom/sepolicy_vndr/sm8450"
           name="LineageOS/android_device_qcom_sepolicy_vndr"
           remote="github"
           revision="lineage-23.2-caf-sm8450" />

</manifest>
EOF
