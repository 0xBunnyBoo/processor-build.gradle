apply plugin: "application"

mainClassName = "org.ethereum.lists.chains.MainKt"

dependencies {
    implementation "org.jetbrains.kotlin:kotlin-stdlib:${KOTLIN_VERSION}"

    implementation "com.github.komputing.kethereum:rpc:${KETHEREUM_VERSION}"
    implementation "com.github.komputing.kethereum:model:${KETHEREUM_VERSION}"
    implementation "com.github.komputing.kethereum:erc55:${KETHEREUM_VERSION}"
    implementation "com.github.komputing.kethereum:crypto_impl_bouncycastle:${KETHEREUM_VERSION}"

    implementation 'com.beust:klaxon:5.6'
    implementation 'com.squareup.moshi:moshi:1.15.0'
    implementation 'com.squareup.okhttp3:okhttp:4.11.0'

    implementation "com.twelvemonkeys.imageio:imageio-jpeg:3.9.4"
    implementation "com.twelvemonkeys.imageio:imageio-batik:3.9.4"

    implementation "org.apache.xmlgraphics:batik-rasterizer-ext:1.16"
    implementation project(":model")

    testImplementation "org.jetbrains.kotlin:kotlin-test:${KOTLIN_VERSION}"
    testImplementation "org.jetbrains.kotlin:kotlin-test-junit:${KOTLIN_VERSION}"

    implementation 'com.github.ligi:ipfs-api-kotlin:0.15'
}
