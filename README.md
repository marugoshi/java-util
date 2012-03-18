# Units

## Ssh

### Authorized Key Decoder

This is sample for scala.

  import org.marugoshi.javaUtil.utilSsh.
  val sampleKey: String = "ssh-rsa AAAAxxx...."
  val decoder: AuthorizedKeysDecoder = new AuthorizedKeysDecoder()
  val publicKey: PublicKey = decoder.decodePublicKey(sampleKey)

This is sample for build.scala.

  resolvers ++= Seq(
    "Marugoshi Java Util Repository" at "http://marugoshi.github.com/java-util/maven2"
  ),
  libraryDependencies ++= Seq(
    "org.marugoshi.java-util" % "util-ssh" % "1.0.0"
  )
