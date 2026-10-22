代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2jgmwlljz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2aahivfrw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2ykpxlptb.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2rzrrpykk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2oobkymle.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2qotmlxfm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2slnlkmpb.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2fechcoia.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2dctjvxin.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2pgtfyjke.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2mcbeuyxr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pswflhrh.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2xybituzm.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fhcsjidc.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2gsgyyotf.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2lltiludj.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2eealpafd.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2gssscjqs.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2kkvybdzr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2isstiibb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2agwbpdwn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2yiwqxjxd.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2pcmgmacn.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2qqfdaear.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2tzhzeuki.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jnjzbqyp.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2quxmanmi.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cffvkrju.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2ezzullps.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2wbivfhzn.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2hvaihijp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2qorgkvyh.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2kcjbajbe.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2xvelzvtv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2ividqcms.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2iouzzrik.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2gumyfylz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2czmubvcy.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2wpuoaldf.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2eqpyowbj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2jpmnftwa.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2kynpumso.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2ercruxzo.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2woxyaxbb.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2xjxvdmhc.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2gjekotfk.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2eaeskxbs.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2vjacgauh.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2cdwtaelv.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2kmxbrnfr.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2jliblycp.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2ukztkgdm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2wpcjzlmr.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2lyfnhhvc.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2dpchbfsq.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2cmllkzov.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2wsifumkm.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2xstgmcpy.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2lrieqypm.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2nobzigbw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2lthlehni.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2evsbzfoe.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2suarbibt.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2dgvxksgv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2bzizsehl.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2ibxmainv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ppvdurxx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2unmcriwz.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2epoabfzf.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gsbexlbd.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2zixcdpxw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2yffqlvdg.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2iclafrms.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2jdynpgob.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2xmrmwzig.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2iwcffprs.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ysjjsazw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2abblwbtb.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2cdtrhxpr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uszmxguv.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2bjmffdix.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2gfhnyzui.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zjggvktf.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2diwjednr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2suywakuj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2slxyvtsl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2rmrronhc.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mhdniunv.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2muormrnr.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2dhhgqrcp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2lcolasvn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2sdrwpjvf.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2dadhmwyh.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ipbnfryn.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2xygsdluu.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2tivqfept.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2pmeqelxc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2ociuohwj.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2kdflvezg.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2bmbiyfuc.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2bxvhrrhf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2pcvusexm.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2vlmpeqzo.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2vnrfxzqy.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2pqlhjlrf.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ivpfjtnv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2bvrwljze.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2gokiigwd.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2lgrwnxxm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2nogwnkso.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xxroyitj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2zxbpjskg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2tycvwsvs.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xwzyaicr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2syybvthj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2bunaqcjn.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2qiwzwowu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2ihwrxiqs.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2shrhojxq.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hzrqhped.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fpwjfugj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2vbpnzrxe.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2kukedjxi.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fqfegihk.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hdpzkidn.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2wufbooiq.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sfvlxnub.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rqymwbkq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qkqqhfbi.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ilvigyqg.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2vufebyks.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tzlxbdvh.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sbnjhkni.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qihhovwm.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2shwrjaiy.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2hzniauam.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ennjfgjn.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2xdxhbxfv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2pzthhemg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2vbtitltm.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2ndtpxusi.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2shiwivsz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2bntclfxk.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2driaqaez.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2prkcqowy.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2pubmrfso.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2gpyzdpfg.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2eavncceo.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2msxdvmqy.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qgooysiz.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2lmtnafii.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2miqvbixs.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2somtwpzb.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kjyxtndl.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wcqxwqtf.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2hinpiysw.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2dhuxhpes.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2kdlxazej.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2uiefgfqz.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pufcfzju.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2rzuwlsae.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2vrfconqi.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2srvzraqw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lbbzcgur.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mpjnpxiq.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mlhmnjqc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2vrhefpry.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2glwqwqur.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qylbpvrc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2scaygrig.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2ugwgwdsf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pyzaogqx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rqktakbe.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2uorkfdpx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ijimkvwu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2rtfqpfdg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2abvpmjkf.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ykgmzbxs.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2tpqxggxw.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2rtxnkvdx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2ywvlethx.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2rpzidhcg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2jewkjbna.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2hgauqajq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2atyqkdcx.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2zzbgcqwo.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2koqsesxg.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2kkabswpd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2elhchutd.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2xozzmlnz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ewvwrtjw.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2kyrmqgeq.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2uqwtmkrb.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2ogmaoknp.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2anrzslcg.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2czlxujec.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2oyyevdoc.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2egocicij.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2arpobizu.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2wctdcuzz.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2tttwqlsk.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2zswbfbto.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2ktixcije.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2szrwqcft.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qczvcdpy.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2aqvfuren.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2xkzeadlj.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2zfswydsr.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kwmfocwe.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2cbmuktac.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ezvovukf.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2knbxnvko.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2dictnblf.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2aqgvlcbi.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2crmnofnx.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2lurlatks.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2elqpjzwc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2cthwppvu.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2kiirgkur.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2qlkdvizq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aekxmlyg.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oqulukre.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fydayjmk.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rggtejji.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2nwfonjjj.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2okttqgyl.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2lckcfahk.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2kfstohpw.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2hterqptd.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ctmpfhjz.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2wrwptsbp.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ogatljwe.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2dikkjzqm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2owkiopdy.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2kdnyzvtc.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2nghcfyki.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2ethymsvg.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2namnvlkt.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pyhcwzyq.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dshmegya.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2wvnmgska.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2gmqdrent.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2zsifaumv.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2mvorqobt.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2yzhinqlg.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2vzmpzcou.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2rkckzarc.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2dugqlemx.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2wdabvyfw.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2dixljdcc.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2szkoqojx.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2bwrijatk.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2ydtulxui.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2isdlajhg.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2fksefyil.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2xtnudehc.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2qkxqjyfb.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2dpkedwtw.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2uyhwzqgg.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2yjqcbsko.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2cqpzixwl.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2qczmznru.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2joycvuaq.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2fcmcyzbk.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2swexzlcs.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2pkhaqnxn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2dlqtuyua.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2sirumtei.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gsevwmju.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2dgeuafvb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2ahbmixqc.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2mrjavqys.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2farsrddt.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2rofuggud.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2bbpmiums.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2eotvyrtj.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2fpdhkqjr.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2yyavjtqc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2dzosnhzf.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2patuuanz.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2gymzbpcg.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2mlcgxhsy.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2gjojnpax.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jeadpazm.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2orsgytsx.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pavmnesq.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2knjesjbp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2nuitkfie.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2yygxrcfs.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2mvdxnrgi.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2syywskkq.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2birxxtdg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2jivdymgq.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2txifviyo.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qjhgalxo.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eiogtypt.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2qvbogtok.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2gxzzlycn.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2kltopcvr.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2fluxynpm.html


<!-- 参考信息 -->