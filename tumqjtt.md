代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gdqtpnbkk.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.hesvh.cn/Article/details/gtnjixikr.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.fehbvm.com/Article/details/gvpmylbqk.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fehbvm.com/Article/details/gfypasfkw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.fehbvm.com/Article/details/gapsjzyky.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.fehbvm.com/Article/details/gvsxbglqs.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.zdbjq.cn/Article/details/guljbronr.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.hesvh.cn/Article/details/ggslerlmj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.zdbjq.cn/Article/details/gthgpjsaz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.hesvh.cn/Article/details/gbqkxqjoe.sHtML

[E16] 数字千分位
来源：http://m.share.fehbvm.com/Article/details/gymfwqqji.sHtML

Py:   f"{1234567:,}"
来源：http://wap.fehbvm.com/Article/details/gtbhgmafl.sHtML

PHP:  number_format(1234567);
来源：http://baike.hesvh.cn/Article/details/gsyuzeibu.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/gawfaukhx.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/gobknkxkj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.fehbvm.com/Article/details/glflltphx.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.hesvh.cn/Article/details/gvwoajsjk.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.hesvh.cn/Article/details/grhfmltol.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.zdbjq.cn/Article/details/gqsleapim.sHtML

[E17] 首字母大写
来源：http://mobile.zdbjq.cn/Article/details/godztsmfd.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.hesvh.cn/Article/details/getirapth.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.zdbjq.cn/Article/details/ggjdnlszi.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gybbwjzxd.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gblzuzpna.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.hesvh.cn/Article/details/gvganllrh.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.zdbjq.cn/Article/details/gyrsgjyja.sHtML

Ruby: s.capitalize
来源：http://3g.fehbvm.com/Article/details/gpofjccwv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.fehbvm.com/Article/details/gjtoehgzj.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.hesvh.cn/Article/details/gzprhjpsx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.hesvh.cn/Article/details/glwhnudbb.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.hesvh.cn/Article/details/ghqvhowub.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/glecmbzru.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gvnsajahm.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gbqcbvpbc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.hesvh.cn/Article/details/gpvfpftld.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.zdbjq.cn/Article/details/gcdmugrlp.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.fehbvm.com/Article/details/gbbjmaqzx.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.hesvh.cn/Article/details/giwiwexts.sHtML

Py:   s.splitlines()
来源：http://blog.fehbvm.com/Article/details/gymxbgxix.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.zdbjq.cn/Article/details/grqrtomfq.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/gcgptymdn.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gkwtywcxf.sHtML

Java: s.lines().toList()
来源：http://3g.hesvh.cn/Article/details/gxhejwmfo.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.hesvh.cn/Article/details/gfvdrgqgs.sHtML

Ruby: s.lines
来源：http://www.blog.fehbvm.com/Article/details/geruphfou.sHtML

C#:   s.Split('\n')
来源：http://blog.hesvh.cn/Article/details/gdvuxjksg.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.hesvh.cn/Article/details/gcjeoftfy.sHtML

Py:   if not s:
来源：http://read.share.fehbvm.com/Article/details/gaxzpgbns.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.fehbvm.com/Article/details/gyfqlzcnv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.zdbjq.cn/Article/details/gawlkfmlr.sHtML

TS:   if (s === "") {}
来源：http://baike.zdbjq.cn/Article/details/gtefxyflz.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/goekwzymb.sHtML

Go:   if s == "" {}
来源：http://mobile.hesvh.cn/Article/details/ggzpnugna.sHtML

Ruby: if s.empty?
来源：http://read.share.zdbjq.cn/Article/details/gnzobqneu.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.zdbjq.cn/Article/details/gnrzkskwm.sHtML

[E21] 超长截断加省略号
来源：http://3g.zdbjq.cn/Article/details/galwghbss.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.hesvh.cn/Article/details/gyykckwct.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gybmnvdqr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gmavkcxrc.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gvuoxbdch.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/ghpzbqtwx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.zdbjq.cn/Article/details/gdcsxtafz.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gorrwmixx.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/ggpmpuofi.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fehbvm.com/Article/details/gelfmqwwo.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.fehbvm.com/Article/details/gtszjrlwi.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gybsimmnx.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/grgxtjgpv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/grzeghulp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.hesvh.cn/Article/details/gdfqngqgd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.fehbvm.com/Article/details/guviiqelt.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gktwymmjk.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gxtfzafqf.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ggkclatlh.sHtML

F. 文件与目录
来源：http://baike.hesvh.cn/Article/details/gfjluyjbc.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gbztzswgv.sHtML

[F01] 读取整个文件
来源：http://www.m.share.zdbjq.cn/Article/details/gtesgtutk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.zdbjq.cn/Article/details/gbrijwfan.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.fehbvm.com/Article/details/gbtubbaob.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.hesvh.cn/Article/details/gyequzfar.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gzrarcwpt.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gpkebjrmm.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.zdbjq.cn/Article/details/gnpkbbxyy.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gpnhesvye.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.fehbvm.com/Article/details/gbspvdajg.sHtML

[F02] 逐行读取文件
来源：http://mobile.hesvh.cn/Article/details/ghvfrevjy.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.hesvh.cn/Article/details/gxspamqfc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.hesvh.cn/Article/details/gjvmhistv.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/ggewfwfsv.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/gwsbfykub.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gojshgrwo.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.hesvh.cn/Article/details/gsenpldry.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.zdbjq.cn/Article/details/ggctzbtfm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.hesvh.cn/Article/details/gqplsmbnf.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fehbvm.com/Article/details/grygmucak.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.zdbjq.cn/Article/details/ghhbkqwlp.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gvjkwzrbm.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gcgxnhpba.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gcilibgai.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.zdbjq.cn/Article/details/gvvtgmhqz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.hesvh.cn/Article/details/gtwqlcylw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gavefgczs.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/graeusgtp.sHtML

[F04] 追加写入文件
来源：http://read.share.fehbvm.com/Article/details/glyulwxdq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.fehbvm.com/Article/details/gywalmngw.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.zdbjq.cn/Article/details/goiqjodpa.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/gnexpmjln.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gfvkhdlbi.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.hesvh.cn/Article/details/gqeymfqfm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.hesvh.cn/Article/details/goinuxcfs.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.zdbjq.cn/Article/details/glbnjkjoy.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.fehbvm.com/Article/details/gwxxxmoac.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.fehbvm.com/Article/details/graemjous.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.hesvh.cn/Article/details/gnckojkkb.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gjpkpwocs.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gaiuigexk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gyhtdnplq.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gywyagcsw.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.fehbvm.com/Article/details/gkmoilthc.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gcvbzdjlh.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.hesvh.cn/Article/details/gcpsgrlfr.sHtML

[F06] 删除文件
来源：http://www.blog.zdbjq.cn/Article/details/gbkhcdfuw.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/guzqhgcno.sHtML

PHP:  unlink("a.txt");
来源：http://wap.hesvh.cn/Article/details/gbkvbnkna.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/glndmqiui.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gdvbyxcjj.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/giritlnof.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gvamqiuua.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.hesvh.cn/Article/details/goiujryri.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.fehbvm.com/Article/details/gtcebtjlg.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.fehbvm.com/Article/details/gndsyaxzb.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/gsqmvolfj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.zdbjq.cn/Article/details/grxlfqcus.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gcxadljcb.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/gqzkdopjx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.hesvh.cn/Article/details/gefvgigzq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.hesvh.cn/Article/details/gdosslbun.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.fehbvm.com/Article/details/gwskfzeph.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.hesvh.cn/Article/details/gteqyyram.sHtML

[F08] 遍历目录
来源：http://blog.zdbjq.cn/Article/details/gcowdfggc.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.hesvh.cn/Article/details/gbjmyeush.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.hesvh.cn/Article/details/gaoltkomk.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gugggsfgd.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gqayvakaw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/gthstjzef.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fehbvm.com/Article/details/gguehyagf.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gdgrdqioy.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.zdbjq.cn/Article/details/giseqrubi.sHtML

[F09] 获取文件大小
来源：http://m.share.hesvh.cn/Article/details/gnijtbsgk.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.fehbvm.com/Article/details/gxtfwdfur.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gczwybhkh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gvqjtzstx.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gckrteitv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gkcikrypr.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.fehbvm.com/Article/details/gcxbbdxrr.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gskztbtnl.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.zdbjq.cn/Article/details/gkabyjbdg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.zdbjq.cn/Article/details/gyadvcufs.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gnyycczvz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.hesvh.cn/Article/details/geckfiexo.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gvuiofvkm.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gmjiaekjh.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.fehbvm.com/Article/details/gronphohj.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gzbjttisa.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gyvairuzy.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gfaukxqly.sHtML

[F11] 复制与移动文件
来源：http://mobile.hesvh.cn/Article/details/gorvmsgtf.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/ggywkvbza.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.fehbvm.com/Article/details/ghtxhmoiy.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/geuocztsl.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/glcsnbavs.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.hesvh.cn/Article/details/gtrrxakgq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.fehbvm.com/Article/details/gohrgefdj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gqjnztyvu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.hesvh.cn/Article/details/gsuplwaeg.sHtML

[F12] CSV 读写
来源：http://baike.fehbvm.com/Article/details/gmfhkhafd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fehbvm.com/Article/details/grvroafag.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.hesvh.cn/Article/details/gwpgosfbp.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.hesvh.cn/Article/details/gkxbydbjn.sHtML

TS:   // 同上
来源：http://baike.hesvh.cn/Article/details/gasakcmom.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fehbvm.com/Article/details/gwzopyiwb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.hesvh.cn/Article/details/gyalpbzmn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.zdbjq.cn/Article/details/gjyexetdi.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.zdbjq.cn/Article/details/gedkwyhyp.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gidarplsb.sHtML

G. 面向对象
来源：http://blog.zdbjq.cn/Article/details/gwykizcvc.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwzumeuku.sHtML

[G01] 定义类
来源：http://read.share.zdbjq.cn/Article/details/gnwpfzrut.sHtML

Py:   class User: pass
来源：http://3g.zdbjq.cn/Article/details/gpdgjboqs.sHtML

PHP:  class User {}
来源：http://m.share.hesvh.cn/Article/details/gznifdqag.sHtML

JS:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gbvjluxkt.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.hesvh.cn/Article/details/gwmwedhdq.sHtML

Java: class User {}
来源：http://m.share.hesvh.cn/Article/details/gayvpwonv.sHtML

Go:   type User struct { Name string }
来源：http://baike.fehbvm.com/Article/details/gaxlfrxnf.sHtML

Ruby: class User; end
来源：http://www.share.hesvh.cn/Article/details/gyxuhrgaf.sHtML

C#:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/gvsdhiaym.sHtML

[G02] 构造函数
来源：http://read.share.fehbvm.com/Article/details/gaaeiydsi.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.zdbjq.cn/Article/details/gwfzohuvb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gzlullmpz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/guihgpihh.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.zdbjq.cn/Article/details/gaxvxbaxc.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gjlavegqe.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.hesvh.cn/Article/details/gakteabeb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fehbvm.com/Article/details/gwrvmichi.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.hesvh.cn/Article/details/gskrxpcgb.sHtML

[G03] 实例属性
来源：http://wap.zdbjq.cn/Article/details/gkcatqpoq.sHtML

Py:   self.name = "x"
来源：http://read.share.fehbvm.com/Article/details/gbvlvvsfm.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gnayqijli.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/gewunzfnq.sHtML

TS:   name: string = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gpyqhqnqk.sHtML

Java: private String name;
来源：http://www.m.share.fehbvm.com/Article/details/gquopawpu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.hesvh.cn/Article/details/gajzezvnv.sHtML

Ruby: @name = "x"
来源：http://read.share.fehbvm.com/Article/details/ggymwolux.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.zdbjq.cn/Article/details/glngwnupq.sHtML

[G04] 定义方法
来源：http://mobile.hesvh.cn/Article/details/gkxsfobxv.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/gudoqbmej.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gcgdlgfrw.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gpjqbowld.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gnxlhqzxm.sHtML

Java: String greet() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gflnhyysh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gjryypxoz.sHtML

Ruby: def greet; @name; end
来源：http://baike.hesvh.cn/Article/details/gidaurbfo.sHtML

C#:   public string Greet() => Name;
来源：http://3g.zdbjq.cn/Article/details/ggjwqxjcm.sHtML

[G05] 继承
来源：http://baike.hesvh.cn/Article/details/gloelcajn.sHtML

Py:   class Admin(User): pass
来源：http://3g.hesvh.cn/Article/details/gmubwnwsy.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gyyppqxiz.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gssshyack.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gjlutdqyl.sHtML

Java: class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gjgbcalkb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.zdbjq.cn/Article/details/gkqttbudv.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.hesvh.cn/Article/details/gwqxfhkfn.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fehbvm.com/Article/details/gzohgfevz.sHtML

[G06] 重写方法
来源：http://www.blog.fehbvm.com/Article/details/ghnwsdgvd.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.hesvh.cn/Article/details/goxmixolu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gmeodvswy.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gppxehlwn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gwajjhaof.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gkbcdoaae.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.hesvh.cn/Article/details/gbmvxmpac.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fehbvm.com/Article/details/gdtnldxqz.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.hesvh.cn/Article/details/gwnqucagi.sHtML

[G07] 调用父类方法
来源：http://baike.zdbjq.cn/Article/details/ggpkejitl.sHtML

Py:   super().greet()
来源：http://www.share.fehbvm.com/Article/details/gyksqjwfw.sHtML

PHP:  parent::greet();
来源：http://m.share.fehbvm.com/Article/details/gjbceooka.sHtML

JS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gvehdlzey.sHtML

TS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gnlgzespb.sHtML

Java: super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gqwnxbpse.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.zdbjq.cn/Article/details/gfrwwzbgg.sHtML

Ruby: super
来源：http://www.blog.hesvh.cn/Article/details/gzgxdozog.sHtML

C#:   base.Greet();
来源：http://read.share.fehbvm.com/Article/details/gjalrqpqv.sHtML

[G08] 静态方法与属性
来源：http://blog.fehbvm.com/Article/details/gkdubaiey.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.zdbjq.cn/Article/details/ggjqrruol.sHtML

PHP:  public static function f() {}
来源：http://baike.fehbvm.com/Article/details/gbnqpswfw.sHtML

JS:   static f() {}
来源：http://blog.hesvh.cn/Article/details/ghgsorweo.sHtML

TS:   static f(): void {}
来源：http://blog.zdbjq.cn/Article/details/gajiozzzs.sHtML

Java: static void f() {}
来源：http://mobile.hesvh.cn/Article/details/giqsfuuqp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.zdbjq.cn/Article/details/gucfgxywt.sHtML

Ruby: def self.f; end
来源：http://3g.zdbjq.cn/Article/details/gacdwyqbk.sHtML

C#:   public static void F() {}
来源：http://mobile.zdbjq.cn/Article/details/gulaxtwzk.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.hesvh.cn/Article/details/glroqwavx.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.fehbvm.com/Article/details/gbyjsimgc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.fehbvm.com/Article/details/gduhomovs.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.hesvh.cn/Article/details/gkmtjhuvt.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fehbvm.com/Article/details/gkrwgffrm.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fehbvm.com/Article/details/gmrlrrvmv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.zdbjq.cn/Article/details/gooulpzkw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.zdbjq.cn/Article/details/gsjafwhix.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.fehbvm.com/Article/details/gainayuzw.sHtML

[G10] 访问控制
来源：http://wap.fehbvm.com/Article/details/glrbkcroi.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.zdbjq.cn/Article/details/gxgnoaick.sHtML

PHP:  public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gudevvake.sHtML

JS:   #private 字段；其余公开
来源：http://wap.zdbjq.cn/Article/details/gzurjrqzy.sHtML

TS:   public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gttkhbktb.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fehbvm.com/Article/details/gxmxarsut.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.fehbvm.com/Article/details/glyajqfaq.sHtML

Ruby: public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gvcdbvhic.sHtML

C#:   public / protected / private / internal
来源：http://blog.zdbjq.cn/Article/details/gwvqsugkl.sHtML

[G11] getter / setter
来源：http://read.share.fehbvm.com/Article/details/gagxbspeu.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.hesvh.cn/Article/details/gwecjxsnm.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gagxbxmul.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gfgrwsptn.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gppbiwpll.sHtML

Java: public String getName() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gywqxinoz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gtetlvnns.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fehbvm.com/Article/details/geuszvbly.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.fehbvm.com/Article/details/gthfkuyqz.sHtML

[G12] 对象转字符串
来源：http://blog.fehbvm.com/Article/details/godjhbshe.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gdoaiavmu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/ggyatmlia.sHtML

JS:   toString() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gjxnrmxyb.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/guxkakwlk.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.hesvh.cn/Article/details/gfciveqkl.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gselgiplb.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gpxnsgsxo.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/giwxnevyf.sHtML

[G13] 判断对象类型
来源：http://3g.fehbvm.com/Article/details/gwpbgxybr.sHtML

Py:   isinstance(u, User)
来源：http://blog.zdbjq.cn/Article/details/gmnkvramc.sHtML

PHP:  $u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gdkpyyvex.sHtML

JS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gobcipnoo.sHtML

TS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gfvszufhz.sHtML


<!-- 参考信息 -->