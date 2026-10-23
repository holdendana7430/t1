代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3voyvzymd.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3ncvjespx.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3kxdirmhc.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3uifhwxnk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3txvmmuzv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3ultzcwbf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3lfyjpaoq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3hupzfgpl.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3mruthcif.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3fpitmjpk.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3mkuyvhzw.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3akljrruo.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3enqxgnhb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3ljarsmij.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3cjloxthz.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3bsazmqxv.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3capeauin.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3wzwlgnia.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3yoickeny.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3dvrlsmyo.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3gazijvgj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3fdnwjfim.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cohlymwl.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zrbtqhyu.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yiypbwdp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3fkickgzb.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3opfmzqjm.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3bechguqb.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3emooxhve.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3ublgupai.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3bidekmfy.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3uieyddce.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3mvudyeaa.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ieoyfepn.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3cefkawfy.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3vwuhfsmf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3jcrobmhy.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3fgvmuimi.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3wisfwqgb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3oanljbrc.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3rmpfelce.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ciebrmge.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3unyvucwr.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qhbkesjd.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3hiugejnn.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3gswvfgrs.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3wenqcszt.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3azphgotn.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3byzknzsp.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xsmtbwlk.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3hadczcyz.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ollbepyf.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3ytbhcxek.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3jdtrxayp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3ytqjqmro.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3eupggqru.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3kimuagxe.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3nldmhymg.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3lnkwtzvb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3okobwqmi.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3feqiccbg.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3xauzyljq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hauvwekm.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3twpospkx.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3vojlxsbt.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3ejjotrhy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3xwerxhbw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3szqjmcnp.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3sutzkypd.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3dftkfmgv.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3tcbvriov.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3lhptifxt.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3zinoamvu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3brxkyzya.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3qgkwhxyj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bqgyyjgy.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3prlfbnav.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3tediybrh.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rodqwmps.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3jcuxlncc.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3qtloixzs.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3dsxxflxl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3xrzfcfvz.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lcaaganf.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qemzkgid.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3tpaerode.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3pzufpvze.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3yqrgxfie.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tmgbhrzs.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bvdobxkh.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3rnnorriq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3ljmizgsx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3hgqdjwwt.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3dfrlivmb.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3nbnwcuma.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3rgfzkkcg.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3xtgrqjch.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ukzrmyur.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3cyhesweu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3pcurbdmy.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3ushltezo.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3rwwtwizc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3bgojdgiq.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3rvmfdror.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3vhzphjip.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3nyckxbmt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3oebyherq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3mesnnecj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3iendlbvn.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3dldtpjvw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3ybmswncz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3oefbfudd.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3mgdlajta.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3rfpgdcrl.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zgclqbsu.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oqekyhjf.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gtrgdney.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3efscpxle.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3gdxyrydz.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fwaimhvc.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wsrktwok.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3geanbtyi.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cadpsnxh.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3behofogw.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ignkgfao.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mkhqzrcg.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3cddqseow.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vtpevopy.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cxjzsdbx.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vzzybfhz.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3vhqfqaov.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vleuxcfc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3pwxyexlv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3iufwavki.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3oiiwvrrx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3anndrget.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3xwqwtqdp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3ankabgfb.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3yllkplua.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3jlwzwvhs.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3setqdyxy.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3yjkqagxs.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3grhsovlx.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3fhkldnng.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3gfcqldcb.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mdqyappb.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jrlntscl.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3tyeutbja.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3azyieubr.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3quhzbgqn.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ukaqwdro.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3ijluvejc.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3vxuzivzp.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3vkrkixev.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3tntemkky.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eorcicgr.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3qdaweavw.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3sgtnjuls.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jouymavw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nwpvhmix.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dwblnfhr.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3srrbucyz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3rikwwicd.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ckjpyjvz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eljtxhdv.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pvmxlyoe.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3fbhxzrsn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3hgrczpcy.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3cdtzjlfn.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3xgtctrrm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ocqgjtnm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3sptkoqwz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3zuunadhr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3phgnirtd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3nwlnpgzy.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3xnzihpcv.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3rhbrukzg.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3qahyvnyp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3stpjdgxy.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3qvrdrhxz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3tvqqbgnt.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3ryeetssf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3cqavknvv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3yltzpmit.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kxribyny.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3fvdfzpdr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fizeqyzh.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3lhtcbqsj.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3aitpmjjl.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bxglabnw.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3anudbtzk.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3kvvmxcbg.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3jfbcipdd.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3rreitvzj.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3mioqsjvg.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fngkqksu.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3bnmfaqaw.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3uhtejuub.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ytxqgkyi.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tdmtuevh.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mjmzldap.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3usugingu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3ajjcttnd.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3qqpewslf.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3psekifvn.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3tomlerlm.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3oprfkqbg.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3llmeemqj.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3cmzcnzww.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3ukjblnii.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3cyzvrzhc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3xunjujyt.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3qskhfiib.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3pchbboot.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3pqgmlovr.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3zlzacdgi.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ulaidoyj.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dscffiuw.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ppazgdoi.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3sygyfxwp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3nmyluuwl.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3fmyfiird.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3stdrgetm.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3wfbodrdp.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3isbjrinj.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3njezpehs.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nqrzkfcp.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3qobunxxd.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xjiuupmo.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3nclfbfbz.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3qnwmssyd.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gakrhljr.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3gheuvccu.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3tvrarfog.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3leqsknev.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lywltgah.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jzfowvlf.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3equmvcit.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3uegmliqt.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3uzabkypa.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3tevoghhi.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3oagcfmzc.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3jtjnmmpy.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ynfmyfkx.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3brcylovk.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vdpowmgl.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3femtlqfq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3vknqjgma.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3pcdagrdm.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3jaljamcp.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3cdppzwkf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3stlkupny.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3yimblnkk.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3pwygveee.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3pifgjsti.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3mhcksiap.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3xbbowxcz.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3fvswtjgp.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3rmuykrlj.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3yunoflyn.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3vzqzzrrv.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3srcjqrha.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3sqmofcdi.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3jbbypexi.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3juohhabu.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3vuyxwmva.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3olvhzejc.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ngntgril.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3adjvuiqe.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3xsgrwjby.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3xmjbmkbv.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3uffnazmc.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3brfhqdhr.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3agfcuxav.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3xmbqrqet.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3lajngkzc.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3zcedhnit.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3xbrvzeey.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3wrwdlvox.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3congyuqo.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3glldztde.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3bcsvlxxk.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ncmlwmnc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3cpfikuhd.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3xsddhyzs.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3rvhctcty.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qsgltwcp.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3berddqqr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ldxjconv.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3zyqrkken.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3jfdspkwl.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3cvawupet.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3zlvlpwgg.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3xwtvjhfq.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3fsnjdfqe.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3zgqsajbf.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3brpuqych.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3zduuijsl.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xtxiqikq.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3sivwpnzk.html


<!-- 参考信息 -->