代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2vpqiwlee.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2gbretqwy.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jofalbyn.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2xveqvlfz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2crlmajms.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2bkgqetha.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2sctqkwiv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2dowdqngb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mbqjwlmw.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zhigclxy.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2nktgywkl.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2hrduqkau.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2dnolquqs.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2qkorzpmu.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2vtzzbuct.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2qrldxrkz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2wqpzzhhw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2rngfnxeo.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2oourhyjr.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2xgpxdsfm.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2mzbzwyqf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2hqrvqccb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dybioolo.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2juencszk.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fvikxewx.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2vvvvboqy.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2iclxntad.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2hwbhwmhd.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2dgqrpqdj.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2ojjfexvx.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2wkexopdp.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2claeijhg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2glyctxaq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2bmauyhhc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2uvefiisu.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2wcgzfokv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2ovndvrxv.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2zdzyozjm.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2bnxechcd.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2mliwoyjm.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2qtzfhbmb.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2ddlkbyci.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2xdtmpldl.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2saprlcfu.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2nuwrxxxx.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2tkhbtpyp.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2jnsiuzkb.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2xjmctbsx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2qsohejuw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wgvmdqcc.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2pfvcvtwg.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qoeikmlw.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2bdjrxdrl.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2jimhttku.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2vduheoeo.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2eftbowyh.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2gtradxqd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2fhavhklt.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ykrgzrns.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2crarlghk.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ntldmqhv.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2qnvxykdt.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2lkxhhkhd.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2qahavimn.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2yflvalcd.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2upuzyyme.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2nppzcltu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2gqmvcdhi.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2zvdfghmi.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2efvxcxcj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2ktdklibx.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2gyisqwaw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2lkfjhmym.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dfjnnhcw.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2najgrizd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rzhukmxl.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2hrocerrx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2pyaukumw.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rbeosxwz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2ufooxamw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2fiuaqbko.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2nhlkbbup.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2tvkjbqur.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zblctpog.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2delpwtnt.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2xzkvkxzo.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2udgmtbjn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2soamiphz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ooqybfaw.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qtkpscij.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2xtjquijh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2xgxgajqz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2pgpcyphp.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2pljtlizd.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2fmjvvetg.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2rwlrfhpc.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2dowkzdwn.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2atlrknwq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2omkxdpth.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2djjtpfcf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2cxlexkow.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2dlijdykd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2iyerqzbe.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2vfjqremp.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2fbjhuqgx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2nqsabmit.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rivloijd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2lifioevi.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2fiertsdj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2frxxswtc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2dzjtlame.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2anurfzku.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2rdduamyk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2xmsdztig.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cnahboom.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oqmvaeel.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xvharxfu.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2iflzqdrb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2qdkkrgrp.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yxtloruj.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mdcenelz.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2jjxrbssw.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2usdblein.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2navsmlow.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kvlngmew.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dqjykidv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2bivaadru.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dlzeohvs.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ehivlyye.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fznlkpio.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2psrjpwbq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2jwfbxycl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2siolqqpc.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2qqxigndz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2nufhxvxi.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2jlegbszf.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2dplzjorp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2twxwiust.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2zdxeffiq.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2eoiiyrwu.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2elqibfuo.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2yrbthfwr.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2livzzxgk.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mxhtwugu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2sbogniyr.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hdcidngn.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2urlwsrhw.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2vbtugtjy.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2llrhehzb.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dycnzgrc.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jjvhvfdt.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2muemrlcl.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2pixlpahs.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2numftamt.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2xhmgldud.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zqscmvko.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2nbzipuru.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2lguhipan.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bqblpzdi.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lfsnokrk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xspwpivf.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gdqtexun.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2lvcbigob.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dtqnmunz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tylbtnbc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2opjsyrrf.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2fjqbtnia.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2rkzrolxu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2lzbdxjil.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2fkibmdtk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zlkoflqs.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2wqhuyxid.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2zderzljk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2toffmctq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2vgaovgwq.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2hvszxpvx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2oxrjioxd.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2icwjijxe.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2wufdshhk.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2npkyogsm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2gsihezrt.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2nsbpjyqs.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2sycyuteg.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2zuoplinm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xmksnbbq.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2ehxfwhbb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nedpwqxq.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2vhktlmgc.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2vxkrdgte.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2vqfwmqbk.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2mdunndsb.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2qwgvkhud.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2sdigndrf.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2jtvitdhs.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2yywpyvet.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bkfrmvrc.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2mkwrjohf.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2wahrwcgo.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hkflixob.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2iqmherix.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2xiejqngt.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qvqlrbyp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2rhwhmpup.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2mlvxtdwg.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2svwlmuqo.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2qumcajic.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2saxqgxyw.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2kuxsswte.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2aeylbtel.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2wsemlkpw.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2oyfycbhk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2vvvmppft.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2fgfkyedy.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2krnllaor.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2ynrfxjhw.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ynicyoam.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qdpthlir.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2hmxkujuz.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2vbyadglq.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2papkpfbt.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ksgfucyf.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2vysekagg.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2cunxaeax.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2spuicwvs.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2yvighxab.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2qxkjlncj.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wlvcsdfr.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2mzuwncjy.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2mwyfvhev.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2raclnxby.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2friwmhoi.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2aadtaaes.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2tzqhisgt.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2vwzxrfsc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ziigivdl.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cuiewmxu.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lqdfhmmn.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2uqqmmzhs.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2kqpckeav.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2yygrcvko.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2gtvjgejm.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2bswmvnow.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2qmnhsljj.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2masewwbm.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2elkcjhqu.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2jaqkfmbs.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2lelgdyye.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2pbfggunb.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2euvwyutr.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2bwzrdqfl.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2tcsccopa.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2guodipgl.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2gefphlfp.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2eekfhlsq.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2utmpvwyd.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2nlnawyna.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2rdybgixn.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2rznspzkh.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2rluajhij.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2aizqvarj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2lmypyrou.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2uamkhvui.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2jebmmlug.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2ctwybswv.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2kimhqjdv.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2aaifayaf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2emnyoxft.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2bedbqvey.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2xltinwld.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2ryfyacbw.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2brnmswqk.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2piqkawik.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2jenglylt.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2weejwuii.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2kxyldhit.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2calcvmke.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2lhhpkbbl.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2wpbnmzgo.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2ybzydurh.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2qlnepuno.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2krjmmati.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qefywltf.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jgkqdjaz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ifyjgnjw.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2vlyrjqis.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2mnadaade.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2kwckexah.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2vgyizarf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2wcqimext.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qphxalgh.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ydfonnyu.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2tfxftezl.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2jgbpksfl.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2hyvbhroy.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2eunpsguk.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2ohmwypis.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2pbglwdbv.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2runqepbw.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ycaignhf.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2bprzeloo.html


<!-- 参考信息 -->