workflows:
  ios-release:
    name: Build iOS Release
    environment:
      groups:
        - pickupcoletador # esse é o grupo de variáveis que você criou
      ios_signing:
        distribution_type: app_store
        bundle_identifier: com.app.wra6351acda948515228f31e632
    scripts:
      - name: Build .ipa
        script: |
          flutter build ios --release --no-codesign
    artifacts:
      - build/ios/ipa/*.ipa
    publishing:
      app_store_connect:
        apple_id: "suporte.dev@aquariumtech.com.br"
        app_id: 6444013845
