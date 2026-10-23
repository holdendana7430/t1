代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3lqlznngr.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3avybxolt.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zgucfzis.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3wekfjddc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vfjcufji.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ogwkcoun.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3ojcmdpbh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3ywuvqstf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wsbgfurq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mtjlgkrs.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3fwfmkmkn.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3atjamvfp.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3izidupfz.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3tnocmpra.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ktxjmpre.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3rsrrynsb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3rdxssldw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3yrwuyfas.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3womxvnmb.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3ngudkyuq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3ygxlekuh.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3uugbqyvy.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zguhiipu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3rtcsnowa.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3vfexvbrd.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3bxmykiyz.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3meszcryv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3vrjaibcy.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3ltejrjgt.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3dcsnupyt.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3zqadzivd.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3zzquimbx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3zgnkfpcn.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3owsrsfih.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3mgiohnzt.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3wpcaheke.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3erpooeok.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3cgzofmmb.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3jwzacekf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3bhipwycw.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3nullwihy.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3dugdvxrt.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3dynwxxdd.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3wmjhdaja.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3ywopxiry.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3uuqgfttv.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3ijggdsjr.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3sxecfdbb.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3woaoniem.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3eugcbrtr.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3xxpchpfn.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3fludhmse.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3hspcxmin.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3gopjrllv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ysjhbkcb.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3rjdxznch.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3ifqfbgyl.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ykgdvrnn.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3kxickiqf.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jnnyjexd.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3fvoyudrb.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3hmlbvmud.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3vsmkygif.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3rzbadapv.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3bsnxxypi.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zaifvklb.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3couidykm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ymrbgjhu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3akswjjdf.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3vxezpxdj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3zamxzwrq.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ddyaesft.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3hqalekxl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kxixgaka.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3maqvsguh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fcmpufyz.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3dfsiuwfe.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3aqrdugkg.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lhtemsym.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3mpdoqwza.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ozopdpiw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3inqkrdhk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3kjrctnys.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bdqjvvrv.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3uuoysfdf.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3ltjrkvbx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3bcorgjwo.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3ldqxelyt.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3haocekpm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rkahyqju.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3yvhetmpc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3jdtmxibf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3dayvwpdl.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3msswrenl.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3cmckbcyf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3vxvervru.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3klrldkyi.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3jlvmqpoe.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3zykffzch.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ebqpyerm.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3ggvvhoae.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3ldnwfifb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3wtdmickf.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3hosmyltc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xbqqkqmz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3tiouizuj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3vmnajjvx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3oxwrdbhg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3szwdwpkr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3lwvyfwyc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3biqmjccl.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3qfcjuvla.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3zyfjrqii.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3tpxdnths.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ijpguqqn.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zylynmvf.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ntmmajxk.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3tpwpwchi.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3fhdiibkm.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dvxxvmov.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ramtojzi.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3wfhwlbmd.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wuwzsffb.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ybkfzydg.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pvxfmukl.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bqhxrkwc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ahzjxpkv.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rracarof.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rigcykeo.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cnfcswpg.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3ktkuqgfx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vabwhomb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3plpchtya.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3vdpsgkyx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3isaijilm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3pfhhydun.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3dbmcsdij.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3nflxvsvp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3qjehmvpr.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3bvnjqqlv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3hklpkqst.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3bljchhrs.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3cjujbzif.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jwmhllkp.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3dusfsbox.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3cxxybfpd.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3emjlbucp.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3bnowdgos.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3zyoqzlbq.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ythbknlt.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3utbxpqob.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3fgbdrspu.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3icsznrqs.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3kaumgioo.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3foygywjp.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rnrwxluj.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3baymumiz.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3rnvfrrlh.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3misxvrwe.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xfdfbvsg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dgtmcncv.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rbkqlrnz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3ohhomdkh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sjlissuq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dzbyteyn.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zsabspzc.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3xyqijaoy.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3whmqhptf.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jnltavqd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3evxgcemp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3jmwimfyi.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3umgvirbc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3xkjoiert.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3gxugosdy.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3mmafvwme.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3cfkjsbaq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3lhhppvgf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3otpcvabk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3kpklxogs.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3gxoixftq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3eexiudqf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3tlnlaqjp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3tsdqjnuu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3ohospocq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vqeahjvv.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3deamprbo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xgffwphw.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3skvupclt.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3izwkmwit.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jcadzvwf.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3eqdsvmpu.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3iospyxnw.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3sysxlwxy.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3zxcgsukv.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3vymwlkyu.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3xhpzmoag.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3aungslhb.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3bzmudwtr.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3eewflvwf.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ivssqnpd.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3omwbvlyg.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3otfpcwor.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3tlhkzxfd.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3mjvnjayk.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3pkttvvmt.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3iqpbqvoh.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3hfztianh.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3jnvjonlh.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3prldtxcu.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3vdnbkqak.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3ehktsyfn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3seephwax.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3dhwnxbwq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3svzuqqhy.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3qligeaiw.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3qijrpltr.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wybkcbce.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3vtxpkcvy.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3kmbqcoed.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3axnooqsz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3tnryxtgl.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3odrmznzg.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3tdiknutz.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3krkzhukt.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3ocewoint.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3tmripnup.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3erlmjtof.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3fmnpurfz.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3lsjehdvq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3sdsabodb.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3rqzrzzkn.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3awewnlod.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3nnhwyjun.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3ishromfx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ttcgflif.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rnfzmedl.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qhyawnll.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3jgdnhqar.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3lnheruwq.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3srgnfqhn.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3zfiviape.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3wuulrxxl.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3uodgmzky.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3muiwxshq.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qopdgssy.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zizniknj.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zkbsfkxg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3wgnwbawb.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3jpeimvps.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3iejemrad.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3akqinjet.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3bejpmdii.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3gvqvifgl.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3ucbvbpdi.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3matdqlqw.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3oesxphmi.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3mogcvpwy.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3tewahglv.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3odrxnonx.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3nqabhpwb.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3acchghky.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3gszsjhpy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3ufzbcllw.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3kzkhdyck.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ewdavyke.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3avoxrlqk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3bftxcldw.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3iicaheha.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3epqofyqc.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3rxnjtqkm.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3dzhwppol.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3jyexdkpr.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3emgkdewc.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3lobfrjpg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3fsaijsaa.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3vzqhhmlb.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3mighcyzc.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3jkyuwftb.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3zhggcmlm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3mvpxedti.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3uhngvybq.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3smkajkaj.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3clrycnva.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3vccjwsxt.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3hvvvlvdh.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3wybmkjpu.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3pykznaar.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3mtvabuhv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3pbthfdai.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3larlmmli.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fyrqyojx.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ldealemn.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3wfhniyaq.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3pvnvvzln.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3qvxcvoeh.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3skpaydtc.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3krimqesz.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3diwhamke.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3jyhxuyob.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3vvgcfblv.html


<!-- 参考信息 -->