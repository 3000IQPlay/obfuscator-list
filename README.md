# Java Obfuscator List

A comprehensive list of Java obfuscators, including both free/open-source and commercial options. Contributions welcome!

## Table of Contents
- [Transpilers/Native Obfuscation](#transpilersnative-obfuscation)
- [Bytecode Obfuscation](#bytecode-obfuscation)
- [Obfuscation Benchmarks](#obfuscation-benchmarks)

---

## Transpilers/Native Obfuscation

### Free/Open Source
| Name | Description |
|------|------------|
| [J2CC](https://github.com/0x3C50/j2cc) | Flexible transpiler with lots of cool features and high compatibility. |
| [MyJ2C](https://github.com/MyJ2c/Open-MyJ2c) | Obfuscator made by chinese people that managed to skid some of [Allatori's-V3](https://github.com/netindev/Allatori-v3.0) parts such as String Encryption and some other things into their project. Overall only recommend using it when u have nothing else to use. Can be partially deobfuscated using Allatori deobfuscator. Has a interesting feature called "Confusing CallSites". |
| [Native/Radioegor146](https://github.com/radioegor146/native-obfuscator) | Java .class to .cpp converter for use with JNI. |
| [Native+](https://github.com/Araykal/native-obfuscator-plus) | Modification of [Native/Radioegor146](https://github.com/radioegor146/native-obfuscator). |

### Commercial
| Name | Description |
|------|------------|
| [JNIC](https://jnic.dev) | One of not so many transpilers that offers String Encryption, Control Flow with Flattening and their famous Native compiler. This obfuscator is mainly used for the Native compiling and does a really good job doing so. You can see JNIC as an example in RusherHack Loader. Be aware that the Native obfuscation could cause lag or slow down the processes made in the application. If you would decide to use JNIC for obfuscation then make sure to not use it on it's own and instead use something with it. |
| [JNT](https://discord.gg/vjzmUJhARt) | A new upcoming transpiler that overthrows JNIC and other transpilers in every aspect. Performance, protection, compatiblity, price and more. Some of the components like renamer, call graph integrity, polymorphic string encryption, strong flow, traversing number encryption, integer table encoding, method inlining and most importantly, native virtualization which is something that JNIC does not have. One of the downsides might be the fact that they obfuscate your JAR on Cloud, essentially not obfuscating locally on your device which could create some trust issues. This might change over time. Althought if we ignore the cloud part, there is a chance that JNT will one day become the standart transpiler, replacing JNIC, given the fact that JNT has already managed to be FASTER than JVM. PS: This has been reported by the devs, there have been few samples out there but I can not 100% confirm all of this, it is in development and not released yet. Also has raw bytecode obfuscation, not just native. |
| [Skidfuscator Enterprises](https://skidfuscator.dev/pricing/) | Commercial. Skidfuscator Enterprises is a paid, cloud based, better version of [Skidfusctor Community](https://github.com/skidfuscatordev/skidfuscator-java-obfuscator), which offers more and better features and in the future will possibly even have Native obfuscation. One of the downsides might be the fact that they obfuscate your JAR on Cloud, essentially not obfuscating locally on your device which could create some trust issues. |
| [Virbox Protector](https://lm.virbox.com/product/8.html) | A native obfuscator, has a code virtualization made by chinese people. It's very different from native obfuscators from github and it's very expensive, almost 10k CNY per year. |

---

## Bytecode Obfuscation

### Free/Open Source
| Name | Description |
|------|------------|
| [Abonasera](https://github.com/abonasera/obfuscator) | Pretty lightweight because it only encrypts strings. Should not be used on its own, as it wont stop any reverse-engineer. |
| [AckerRun](https://github.com/leaks-YCgsasxGZY/AckerObfuscator) | Lightweight/Heavy obfuscator depanding on your config. Has some interesting features that not every other obfuscator has. Looks like XenonGuard skid but I can't confirm that. |
| [Alpheratzteam](https://github.com/alpheratzteam/obfuscator) | Older obfuscator using older tricks—Very outdated. Not adequate for use in any layer. |
| [Ambien](https://github.com/iiiiiiiris/Ambien) | Obfuscator that is not getting actively developed anymore. Has some cool packaging features mainly targeting Recaf 2.x with a great succeed since their RedHerring feature adds a fake jar before the real one. Most RE tools don't read backwards like the JVM, so they will read the fake jar. Also has a decent Crasher transformer that confuses various decompilers & other reverse engineering tools. Still contain some bugs/issue to this day. |
| [Avaj](https://github.com/cg-dot/avaj) | Has a nice way of generating decryption subroutines on string constants. Also has some CFG flattening which is always nice to see. |
| [Black](https://github.com/CodingGay/BlackObfuscator) | Android APK DexFile, it can help developer to protect source code by control flow flattening, and make it difficult to analyze the actual program control flow. |
| [Bozar](https://github.com/vimasig/Bozar) | Has some cheap tricks along with GUI that I have seen being used in the Minecraft Community. Definitely a look worth. Can be deobfuscated using [Narumii](https://github.com/narumii/Deobfuscator). |
| [Bruhfuscator](https://github.com/erxson/Bruhfuscator) | Based on [Ambien](https://github.com/iiiiiiiris/Ambien), is a skid of multiple FOSS obfuscators, therefore nothing in it is selfmade or special, it's horribly broken and has "experiemental" features on the most basic of transformers. Skidded transformers from GOTO, MyJ2C, Colonial and Souvenir. |
| [Caesium](https://github.com/sim0n/Caesium) | Has a transformer that implements a well-known HTML injection into any Java reverse-engineering tool that parses HTML tags. Shows alot in Minecraft Community. Can be deobfuscated using [Narumii](https://github.com/narumii/Deobfuscator). |
| [CafeVault](https://github.com/Taptzuz/CafeVault) | Basic Jar-File Crypter, therefore has a lot of room for improvements. Could be used as lightweight top-layer. |
| [CheatBreaker](https://github.com/CheatBreaker/Obf) | Decent obfuscation that looks similar to Caesium's, but not as strong. Obfuscation is overall decent. Shows in Minecraft Community. Can be deobfuscated using [JavaDeobfuscator](https://github.com/java-deobfuscator/deobfuscator). |
| [ClassCloak](https://github.com/SohamGovande/ClassCloak) | Basic obfuscator with string encryption. |
| [CodeEncryptor+](https://github.com/4ra1n/code-encryptor-plus) | Uses JNI to encrypt bytecode and JVMTI to decrypt bytecode in order to protect code. The encrypted Class files becomes malformed and cannot be parsed. |
| [Colonial](https://github.com/ColonialBuilders/ColonialObfuscator) | Rename of [Simple Obfuscator](https://gitlab.com/nickfreeman/SimpleObfuscator), with some additions of [JObf/SB27](https://github.com/superblaubeere27/obfuscator). The string decryption with its hard-coded switch-case slightly reminds of [ZKM (Zelix Klass Master)](https://zelix.com/klassmaster/index.html), tho not nearly as strong. Is beloved by kids who develop their "own" Minecraft HvH clients, mainly russians. Can be deobfuscated using [Colonial-Deobfuscator](https://github.com/Loremas1er/Colonial-Deobfuscator). |
| [Crater](https://github.com/CraterTeam/Crater) | Basic java obfuscator. |
| [dProtect](https://github.com/open-obfuscator/dProtect) | Build on [ProGuard](https://github.com/Guardsquare/proguard) with additional flow-obfuscation, mixed-boolean-arithmetics-transformations and string-encryption. Definitely worth a try. |
| [GOTO](https://github.com/Dimples1337/goto-java-obfuscator) / [GOTO](https://github.com/KgDW/GOTOObfuscator) | An obfuscator made by chinese people written in Kotlin. Has interesting features but are kind of broken. |
| [Grunt](https://github.com/SpartanB312/Grunt) | Another ofuscator written in Kotlin. Should be used as a lightweight layer of obfuscation. Overall has very based features that are compatible with each other. Mainly known in Minecraft Comunity for it's mixin support renamer and compatibilty with obfuscating Forge mods/Plugins. |
| [Herbst](https://github.com/levzzz5154/herbst-obf/) | Light obfuscator made for some mc client. Only good for its flow and *maybe* its String encryption. |
| [HsGuard](https://github.com/3000IQPlay/HsGuard-Obfuscator) | An obfuscator developed by chinese people. Bad skid of Scuti with minimal additions. Can be deobfuscated using [Narumii](https://github.com/narumii/Deobfuscator). |
| [InDy](https://github.com/ventolotl/IndyObfuscator) | A simple project that provides an implementation to obfuscate method calls in Java Bytecode by replacing them with invokedynamic instructions. |
| [JarObfucator](https://github.com/jar-analyzer/jar-obfuscator) | A obfuscator with simple Bytecode transformers such as XOR encryption. Has a Class Encryptor which encrypts the contents of classes and allows you to decrypt them at runtime by using a Java Agent with their decryptor. |
| [Javari](https://github.com/3000IQPlay/Javari) | A simple obfuscator with a nice GUI and not so nice obfuscation-techniques. |
| [JBCO](http://www.sable.mcgill.ca/JBCO/) | Some interesting flow obfuscation techniques that still work in modern Java. Based on the [Soot](https://github.com/soot-oss/soot) library which is also something worthwhile checking out. |
| [JObf/SB27](https://github.com/superblaubeere27/obfuscator) | Pretty outdated. Due to the generic name is more commonly referred to by the author's name superblaubeere27 / sb27. Has some basic features along with a GUI. Still shows allot in the Minecraft Community (Mainly in Japanese/Chinese Anarchy Clients). Can be easily deobfuscated with no effort using [Narumii](https://github.com/narumii/Deobfuscator)/[JavaDeobfuscator](https://github.com/java-deobfuscator/deobfuscator). |
| [Masxinlingvonta](https://github.com/superblaubeere27/masxinlingvonta) | Compiles Java ByteCode to LLVM IR (for obfuscation purposes). |
| [Mosey](https://github.com/Hippo/Mosey) | Outdated obfuscator mainly coded in Scala. Overall is no recommended for use since the obfuscation is very light and is easy to deobfuscate. Mainly used for 2+. layer obfuscation. Can be deobfuscated using [Narumii](https://github.com/narumii/Deobfuscator). |
| [NeonObf](https://github.com/MoofMonkey/NeonObf) | Made up of the easier to defeat obfuscation techniques. NeonObf is also the name inspiration for Radon. |
| [Ob](https://github.com/ShivamMistry/Ob/) | Older obfuscator from 2011 with string encryption, branching, and a renamer. |
| [Obsidian](https://github.com/obsidian-java/obsidian) | Control flow obfuscator that looks like it's being worked on. Looks interesting and definitely unique compared to what you might see normally. |
| [ObzucureVM](https://github.com/HoverCatz/ObzcureVirtualMachine) | Java Virtual Machine made in Java. |
| [Popuskator](https://github.com/erxson/Popuskator) | Obfuscator based of Ambien. 100% Skidded, nothing custom. |
| [Radon](https://github.com/ItzSomebody/radon) | Abandoned experimental obfuscator by ItsSomebody (The person that made some of the parts of this Obfuscator list). Radon is an open-source free obfuscator. It has a UI that's visually similar to Skidfuscator/ProGuard and it is very intuitive to use. Easy to deobfuscate using [JavaDeobfuscator](https://github.com/java-deobfuscator/deobfuscator). |
| [Reflow](https://github.com/PolyRocketMatt/Reflow) | A Java Bytecode Obfuscator. |
| [Retype](https://github.com/JTrixEx/Retype) | A Java Bytecode Obfuscator. |
| [Sandmark](http://sandmark.cs.arizona.edu) | Really old obfuscator research project led by Christian Collberg at the University of Arizona. Has some interesting ideas in static and dynamic watermarking (Embeder & Recognizer) are some of the flow obfuscation ideas are good. |
| [Scuti](https://github.com/netindev/scuti) | Outdated obfuscator. Has an option to pack classes into binary blobs, and load them via a classloader. The binary blob names are just the original class names with simple XOR encryption, and the blob contents are the original class file with simple XOR encryption. Can be deobfuscated using [Narumii](https://github.com/narumii/Deobfuscator). |
| [Sentinel](https://cdn.discordapp.com/attachments/972906162641076317/972942077669310556/SentinelObf-1.0-SNAPSHOT-all-obf.jar) | Dead, Obfuscator mainly known in Minecraft community. Has some basic features. Currently there are no public transformers for it and still can be used. If you decide to use it, make sure to use key "sentinelisback" once you run it in cmd. |
| [Skidfuscator Community](https://github.com/skidfuscatordev/skidfuscator-java-obfuscator) | Skidfuscator is known obfuscator for its simplicity, ease of use, and effectiveness in protecting Java applications from reverse engineering and tampering. You can get free (community) version having overall strong obfuscation. Paid (Enterprises) version has (Unfinished) Native obfuscation with some other features that aren't included in the Community version. Has its own [documentary website](https://skidfuscator.dev/docs/). Requires libraries (Doesn't have max depth). Free version has slightly broken Matcher. Uses [Maple IR](https://github.com/LLVM-but-worse/maple-ir) framework which is something worth checking out. Shows a lot in Minecraft community. |
| [Souvenir](https://github.com/Body-Alhoha/Souvenir) | Lightweight obfuscation that doesn't have anything special. Has only 3 transformers (Light Flow, String, Number). |
| [StarLock](https://github.com/JavaVirtualMachine-source/Java-Obfuscator) OR [StarLock Original](https://github.com/DevPaimonSoft/StarLock) | Pretty solid obfuscation techniques; it is a good canidate for a layer. It has an interesting flow technique called reverseJump which inverts jumps with antonyms to create "else" blocks. |
| [W-Tap Fuscator](https://github.com/Librry1337/w-tapFuscator) | Relatively new java obfuscator with ≈1/2 of transformers skidded. Interestingly, there is a joker watermark and text prayers against RE. Might defend your code, who knows... |
| [XenonGuard](https://github.com/darklol9/Some-Java-Obfuscator) | Decent obfuscator based off CheatBreaker. Kind of looks like free version of ZKM. Has a very good and useful features that not every obfuscator has these days. Even tho there are no public deobfuscation transformers, I still recommend layering it since it's based off CheatBreaker and I am unsure if some transformer are still from CheatBreaker. Overall I really like this one. |
| [XiaoShadiao](https://github.com/SuperShadiao/XiaoShadiao-Obfuscator) | N/A |
| [yGuard](https://www.yworks.com/products/yguard) | Functionally equivalent to ProGuard as far as I can tell. |

### Commercial
| Name | Description |
|------|------------|
| [Allatori](http://www.allatori.com/) | Was a somewhat popular choice in industry. The v3 has been leaked a long time ago [Allatori-V3](https://github.com/netindev/Allatori-v3.0), tho not nothing special. Can be mainly found on Java based Malware. |
| [Binscure](https://github.com/4wl/binscure-license-removed) | Binscure was a commercial Java obfuscator that had a running spat with Recaf. Its primary advertised features were its crasher and zipping abilities and intense flow/indy obfuscation. However as with most cat-and-mouse games, one side would give up. Since we're using past tense here, its Binscure if you haven't caught on. The ASM/RE tool crashers are now fully patched in Recaf with current versions. The flow and indy obfuscation still is fair for the current market. Can be deobfuscated using [Narumii](https://github.com/narumii/Deobfuscator)/[JavaDeobfuscator](https://github.com/java-deobfuscator/deobfuscator). |
| [BranchLock](https://branchlock.net/) | An online, web-based obfuscator primarily known for its AntiDebugging features. It advertises itself as 'modern, lightweight, but powerful,' which is now untrue, considering that it can't compete with modern obfuscators anymore. It appears somewhat in the Minecraft Community. Due to it being web-based, it had some DDoS attacks lately, which caused the site to be down. Also is known to be easy to read though. Minecraft clients like Monsoon v2 or Prestige used this and got cracked many times. |
| [ClassGuard](https://zenofx.com/classguard/) | Relies mostly on class encryption with hardcoded AES keys in native libs. Pretty easy IDA/Binary Ninja/Ghidra exercise if you want to flex on your blog on something. Can be deobfuscated using [JavaDeobfuscator](https://github.com/java-deobfuscator/deobfuscator). |
| [DashO](https://www.preemptive.com/products/dasho/overview) | Shows up a bit in industry and has some interesting ideas (albeit probably outdated) in flow obfuscation. Can be deobfuscated using [JavaDeobfuscator](https://github.com/java-deobfuscator/deobfuscator). |
| [DexGuard](https://www.guardsquare.com/dexguard) | Mainly used for obfuscating Android apps. Never saw any samples. Can be deobfuscated using [JavaDeobfuscator](https://github.com/java-deobfuscator/deobfuscator). |
| [Eskid](https://github.com/PlutoSolutions/EskidRewrite) | Decent obfuscator based on [HsGuard](https://github.com/3000IQPlay/HsGuard-Obfuscator) and [Scuti](https://github.com/netindev/scuti/tree/master). Shows alot in Minecraft Community. Could be possibly deobfuscated using [AckeRun's](https://github.com/AckerRun1337) Eskid deobfuscator trasnformer. Got cracked by [PlutoSolution](https://github.com/PlutoSolutions). |
| [JObfuscator](https://www.pelock.com/products/jobfuscator) | Most of the obfuscated code are just int/double arrays with some light flow obfuscation (Based off sample). Uses polymorphic algorithm for strings encryption. Has only few features. Last update was made on 09.08.2022 which is a version 1.10. |
| [Obzcure](https://obzcu.re/) | Web-based obfuscation service with some inspiration taken from Radon and [SkidSuite2](https://github.com/GenericException/SkidSuite/tree/master/archive/skidsuite-2). Used to go by the name "SpigotProtect" so you might see some Spigot plugins using the obfuscation from this product if you look around hard enough. Can be deobfuscated using [JavaDeobfuscator](https://github.com/java-deobfuscator/deobfuscator). |
| [Paramorphism](https://paramorphism.dev/) | Was one of the most unusual and unique obfuscators at the time it was an active project in that relied a lot more on the JVM's unusual way of loading JAR archives including zip entries with duplicated names and the [fake directory trick](https://github.com/x4e/fakedirectory). Used to be more commonly used before people started ripping ideas from Paramorphism. Can be deobfuscated using [JavaDeobfuscator](https://github.com/java-deobfuscator/deobfuscator). |
| [Phantom Shield X](https://skidonion.tech/#/) | N/A |
| [Protector4J](https://protector4j.com/) | This "crypter" uses a JDK to It's advantage by removing as much critical features useful for reverse engineering while keeping the JDK functionable. It also encrypts your Jar so the JDK just simply can't be replaced. |
| [qProtect](https://qtechnologies.dev/) | Got [cracked](https://masterof13fps.com/forum/index.php?threads/qprotect-cracked-by-hcu.8886/#post-71519) millions of times, Devs and Admin only care about money, promotion and like to d0x people that don't like qProtect and possibly harass them or try to scare them. Their transformers are 1 big pattern and can be easily deobfuscated, not even mentioning the pain people have to go through to even make a working obfuscated jar. String obfuscation sometimes breaks actual strings, failing to correctly encrypt/decrypt them or chunks of code simply getting removed. Horrible scam for $70 (Skidfuscator FOSS is better than this). |
| [Stringer](https://jfxstore.com/stringer/) | Pretty infamous for its complicated AES-based encryption/decryption routines and price. Does not really offer a whole lot of protection, but sometimes does show up in industry. Older versions can be deobfuscated using [JavaDeobfuscator](https://github.com/java-deobfuscator/deobfuscator) and got cracked few times. |
| [ZKM (Zelix Klass Master)](https://zelix.com/klassmaster/index.html) | Zelix KlassMaster Obfuscator is known for its robust obfuscation techniques and strong obfuscation capabilities and is used by many companies to protect their Java applications from reverse engineering and tampering. Currently the best obfuscator for Java right now and always updates their compatiblities for newer or even older Java versions with bug fixes or patches whenever there are public deobfuscation transformers. |
| [zProtect](https://github.com/PotatoSUS/zProtect) | Stupid Binscure skid. Not recomended for use. SRC of it has been leaked and their obfuscation could be possibly deobfuscated using [darklols](https://github.com/darklol9) zProtect deobfuscator or using Binscure deobfuscator to semi deobfuscate it. |
| Zortfuscator | Dead, not so known obfuscator. Can tell that it has good obfuscation techniques from the look at the samples they have on their discord server and some small sample in a video made by [akita](https://www.youtube.com/watch?v=0B9SPdt75JQ). |

---

## Obfuscation Benchmarks
For performance and effectiveness comparisons from external sources:
- [JavaObfuscatorTest](https://github.com/huzpsb/JavaObfuscatorTest)

---

## Contribution Guidelines
1. Fork the repository
2. Add new obfuscators with complete information
3. Keep descriptions factual and unbiased
4. Submit a pull request
