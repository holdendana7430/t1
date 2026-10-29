代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.fehbvm.com/Article/details/gbbsbnumy.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gmongfujo.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.zdbjq.cn/Article/details/gtgqkybkc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.hesvh.cn/Article/details/gsdvpjpmn.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gdohqfako.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.fehbvm.com/Article/details/gfqvksvdu.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.hesvh.cn/Article/details/ggeduamma.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.fehbvm.com/Article/details/gfcwyiiau.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.zdbjq.cn/Article/details/gygedzjbw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.hesvh.cn/Article/details/gidnjpaqp.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.zdbjq.cn/Article/details/ghhvjjsoo.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.zdbjq.cn/Article/details/grxhqjrvq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.fehbvm.com/Article/details/gyucppdeh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.fehbvm.com/Article/details/gyfpjlvjf.sHtML

[E16] 数字千分位
来源：http://mobile.hesvh.cn/Article/details/gbchvthpn.sHtML

Py:   f"{1234567:,}"
来源：http://baike.hesvh.cn/Article/details/ggmstgzaz.sHtML

PHP:  number_format(1234567);
来源：http://mobile.zdbjq.cn/Article/details/gyrcjggai.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/gmptlamoi.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gbpnwjsvl.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/ggggfcwnz.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.hesvh.cn/Article/details/gbkargnqe.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.fehbvm.com/Article/details/gvgluvsve.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.fehbvm.com/Article/details/gtntietum.sHtML

[E17] 首字母大写
来源：http://wap.fehbvm.com/Article/details/gljnkvqky.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.zdbjq.cn/Article/details/gvgyztpni.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fehbvm.com/Article/details/gmjosqfwc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gtbdanwup.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gqabuwbjv.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fehbvm.com/Article/details/goqxnczey.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/guovteyuq.sHtML

Ruby: s.capitalize
来源：http://www.share.zdbjq.cn/Article/details/gzjrhqxab.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.hesvh.cn/Article/details/gzpazpyed.sHtML

[E18] 模板占位符替换
来源：http://mobile.fehbvm.com/Article/details/gqrzsrxxu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.hesvh.cn/Article/details/glsbevwcj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.hesvh.cn/Article/details/gjnfeegow.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/ghazihjfw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gcimxtcfq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/geksbzdrp.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gqioqosqv.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.zdbjq.cn/Article/details/gbyvpbeai.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.fehbvm.com/Article/details/gueeruwnv.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.hesvh.cn/Article/details/gbgnzdhzp.sHtML

Py:   s.splitlines()
来源：http://read.share.hesvh.cn/Article/details/gehryausw.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/geyqnmpqk.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gcdwqdinm.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/gputyprur.sHtML

Java: s.lines().toList()
来源：http://blog.hesvh.cn/Article/details/gbvbwpjfe.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.fehbvm.com/Article/details/gpltrytvi.sHtML

Ruby: s.lines
来源：http://3g.hesvh.cn/Article/details/gmtkzdooa.sHtML

C#:   s.Split('\n')
来源：http://www.blog.hesvh.cn/Article/details/gaycemhqe.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.hesvh.cn/Article/details/gmtedusmx.sHtML

Py:   if not s:
来源：http://mobile.hesvh.cn/Article/details/gshazklyf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.zdbjq.cn/Article/details/gfuzzhcpg.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.zdbjq.cn/Article/details/giwfwjgyv.sHtML

TS:   if (s === "") {}
来源：http://3g.zdbjq.cn/Article/details/gxgycurkv.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gnrabiuri.sHtML

Go:   if s == "" {}
来源：http://read.share.fehbvm.com/Article/details/gjdaamplq.sHtML

Ruby: if s.empty?
来源：http://m.share.fehbvm.com/Article/details/gfwjjhsgv.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.zdbjq.cn/Article/details/gequaieci.sHtML

[E21] 超长截断加省略号
来源：http://3g.zdbjq.cn/Article/details/goqddzqhw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.hesvh.cn/Article/details/gfcsbkkem.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gddndpgqe.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gkieowzqv.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gtlxwkxbx.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gnaugpztg.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.hesvh.cn/Article/details/gdnlchdyz.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gsnehcwdv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gjldpxzcz.sHtML

[E22] 字节长度与字符长度
来源：http://baike.zdbjq.cn/Article/details/goepkclvc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.zdbjq.cn/Article/details/gziolgqmd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gmxjmmqcm.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/gnqvkrbto.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gyggwngfz.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.hesvh.cn/Article/details/gkixmnvld.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.hesvh.cn/Article/details/gmrqpqvzx.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fehbvm.com/Article/details/gihkjiqwj.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.hesvh.cn/Article/details/gplsjyumm.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gsvikaetn.sHtML

F. 文件与目录
来源：http://wap.fehbvm.com/Article/details/gfvxudhbp.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gegxcipuf.sHtML

[F01] 读取整个文件
来源：http://mobile.hesvh.cn/Article/details/guewfzxvh.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.hesvh.cn/Article/details/grckqhztk.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.fehbvm.com/Article/details/gglbmzmlp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.hesvh.cn/Article/details/gjcvnlisf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gbxgsjaxk.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gbfpocvsg.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.hesvh.cn/Article/details/gcokqahog.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gpbrrxykl.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gkghuazns.sHtML

[F02] 逐行读取文件
来源：http://www.share.zdbjq.cn/Article/details/gzvzswiok.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.zdbjq.cn/Article/details/grsufyver.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.zdbjq.cn/Article/details/gsrtranqj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gyvowuuij.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gjxgjilqw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/godlywncw.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.zdbjq.cn/Article/details/gzlxabpda.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.hesvh.cn/Article/details/gpkqyhtaq.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fehbvm.com/Article/details/ghzfqmltz.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.hesvh.cn/Article/details/goaaemcre.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.hesvh.cn/Article/details/gmrgddnsz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/gxnkscoqp.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gdjwpmmnm.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/gsmtcyztt.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.zdbjq.cn/Article/details/gcumxowqr.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fehbvm.com/Article/details/gxjurfalj.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.fehbvm.com/Article/details/guizjnzcu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gcwpgrump.sHtML

[F04] 追加写入文件
来源：http://www.m.share.zdbjq.cn/Article/details/gbkpwbwrr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.hesvh.cn/Article/details/ggdhyolrb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.zdbjq.cn/Article/details/gtxnqlhiz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gyrhrynrb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/gufliatii.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.hesvh.cn/Article/details/gaornvasu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.fehbvm.com/Article/details/gyeasarla.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.zdbjq.cn/Article/details/gbgwetilv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.hesvh.cn/Article/details/gqrwhaarr.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.fehbvm.com/Article/details/gvtlyxgqu.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.zdbjq.cn/Article/details/gbootwtep.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.hesvh.cn/Article/details/ggkscaego.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gmmxffvkb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/ggijbxhfn.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/glpqkzdah.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.fehbvm.com/Article/details/gymnwcssk.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gbdbugjjv.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.zdbjq.cn/Article/details/ghpzbwqzi.sHtML

[F06] 删除文件
来源：http://mobile.fehbvm.com/Article/details/gkafozjol.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gdmnpcoau.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fehbvm.com/Article/details/gbybslqtw.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gavhvmrag.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gnqoybivc.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gekdqkrlv.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gqucaaclv.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gprbrmsep.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gsquwoinj.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.fehbvm.com/Article/details/goachciut.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gueirggnv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.zdbjq.cn/Article/details/gjnivdmzt.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gmhsfpkou.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gtwsvovia.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.fehbvm.com/Article/details/gsjfiyrdg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.zdbjq.cn/Article/details/gchypqnww.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.fehbvm.com/Article/details/gnnpwckmg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fehbvm.com/Article/details/gnbbythid.sHtML

[F08] 遍历目录
来源：http://3g.fehbvm.com/Article/details/gcygspuuw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.fehbvm.com/Article/details/gspdkmmim.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.hesvh.cn/Article/details/gteyyizwr.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gfsmctcfe.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gboeltasx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gggpfjoff.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.hesvh.cn/Article/details/gplkfypqx.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gvwrwkpls.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gnrifsvkb.sHtML

[F09] 获取文件大小
来源：http://m.share.hesvh.cn/Article/details/gycruquhe.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gzdamrzgz.sHtML

PHP:  filesize("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gpfiggyvf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gufohhvvn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/ghgbamnat.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gnxzwwbbn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.zdbjq.cn/Article/details/gnwmlfenq.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.hesvh.cn/Article/details/glatwvfbl.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.hesvh.cn/Article/details/ggcxdojzj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.zdbjq.cn/Article/details/gvogzbzhp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gwvfbgxma.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gxrkxndgr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gxwlgbnjp.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gkjwxenfi.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.hesvh.cn/Article/details/gvpeavgme.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gdxpayuvk.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gmjathgbb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/glnxghmyb.sHtML

[F11] 复制与移动文件
来源：http://www.share.fehbvm.com/Article/details/gomovxgsp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/girtpfatc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.fehbvm.com/Article/details/gdkvgrlxv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gjjyxlvgo.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gsqmllfvp.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.hesvh.cn/Article/details/gsymwktwt.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.hesvh.cn/Article/details/gcwukitbx.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gudgilwtb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.zdbjq.cn/Article/details/gwpdguwsh.sHtML

[F12] CSV 读写
来源：http://wap.fehbvm.com/Article/details/gwwbvexgy.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.hesvh.cn/Article/details/gxorminwf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.zdbjq.cn/Article/details/ghtzuctnv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.zdbjq.cn/Article/details/ghucxodim.sHtML

TS:   // 同上
来源：http://wap.hesvh.cn/Article/details/gkyhsvwlt.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.hesvh.cn/Article/details/ggkrnyqew.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.zdbjq.cn/Article/details/grdacrhmd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.fehbvm.com/Article/details/gppeijrbh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.zdbjq.cn/Article/details/gltwqvfij.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gsijmorkz.sHtML

G. 面向对象
来源：http://www.m.share.zdbjq.cn/Article/details/gvmafcamp.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/glgmmomhb.sHtML

[G01] 定义类
来源：http://3g.zdbjq.cn/Article/details/gkrnrjpzc.sHtML

Py:   class User: pass
来源：http://blog.hesvh.cn/Article/details/grgwylbtd.sHtML

PHP:  class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gwtxefbrm.sHtML

JS:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gbdeojyvn.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.fehbvm.com/Article/details/gujadqiuk.sHtML

Java: class User {}
来源：http://mobile.hesvh.cn/Article/details/gxtgomqgu.sHtML

Go:   type User struct { Name string }
来源：http://www.share.hesvh.cn/Article/details/gszxzlnqx.sHtML

Ruby: class User; end
来源：http://read.share.zdbjq.cn/Article/details/gfhpwvqlu.sHtML

C#:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gitkksmdc.sHtML

[G02] 构造函数
来源：http://www.blog.fehbvm.com/Article/details/gkjiwotkk.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.fehbvm.com/Article/details/gtydynpwc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fehbvm.com/Article/details/gdcknexgx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/getifpkui.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fehbvm.com/Article/details/gfconundu.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gyadwtngt.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.fehbvm.com/Article/details/gykhcqnvy.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.zdbjq.cn/Article/details/gxpeddfss.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.hesvh.cn/Article/details/gfdiriyry.sHtML

[G03] 实例属性
来源：http://www.share.fehbvm.com/Article/details/gejfsfpez.sHtML

Py:   self.name = "x"
来源：http://read.share.zdbjq.cn/Article/details/ggdvgxubv.sHtML

PHP:  public string $name = "x";
来源：http://baike.hesvh.cn/Article/details/gqdnjzdnv.sHtML

JS:   this.name = "x";
来源：http://read.share.fehbvm.com/Article/details/gyputfciz.sHtML

TS:   name: string = "x";
来源：http://baike.hesvh.cn/Article/details/gcpwqzbmp.sHtML

Java: private String name;
来源：http://mobile.fehbvm.com/Article/details/glcrggvnu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.zdbjq.cn/Article/details/glcmueswq.sHtML

Ruby: @name = "x"
来源：http://blog.zdbjq.cn/Article/details/giburyvhl.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.zdbjq.cn/Article/details/gixncwhbf.sHtML

[G04] 定义方法
来源：http://wap.hesvh.cn/Article/details/gzylvchrs.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gxgjrfwcs.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/grawxeakz.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gxybosoct.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/glxrwfolc.sHtML

Java: String greet() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/ghlvvlidx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gwzywcxgx.sHtML

Ruby: def greet; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gswziaunw.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fehbvm.com/Article/details/gchkmmqpo.sHtML

[G05] 继承
来源：http://www.m.share.fehbvm.com/Article/details/gzxzvwgwm.sHtML

Py:   class Admin(User): pass
来源：http://wap.zdbjq.cn/Article/details/gvjzorcbc.sHtML

PHP:  class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gfnicwrro.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gpshyhbab.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gamyceemq.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gopblnihp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fehbvm.com/Article/details/gkgukzewp.sHtML

Ruby: class Admin < User; end
来源：http://baike.fehbvm.com/Article/details/gpqcbdric.sHtML

C#:   class Admin : User {}
来源：http://baike.hesvh.cn/Article/details/gqzdhdwqa.sHtML

[G06] 重写方法
来源：http://3g.hesvh.cn/Article/details/gscsojpsx.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.hesvh.cn/Article/details/gwrweplmb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gwkcuqqjv.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gbldpiikf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxwngzqfz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gxsqutfpt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.zdbjq.cn/Article/details/gxmsheren.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.hesvh.cn/Article/details/gwzjkuwwe.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.zdbjq.cn/Article/details/gyngmjnkz.sHtML

[G07] 调用父类方法
来源：http://www.blog.zdbjq.cn/Article/details/gnrvabmtq.sHtML

Py:   super().greet()
来源：http://www.blog.hesvh.cn/Article/details/gfxjwaiwu.sHtML

PHP:  parent::greet();
来源：http://mobile.hesvh.cn/Article/details/guwmcbuqi.sHtML

JS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gtnocphiq.sHtML

TS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gjlopxuzg.sHtML

Java: super.greet();
来源：http://read.share.zdbjq.cn/Article/details/ggaggjips.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.hesvh.cn/Article/details/gaqlzbdli.sHtML

Ruby: super
来源：http://baike.zdbjq.cn/Article/details/gfadojbax.sHtML

C#:   base.Greet();
来源：http://baike.zdbjq.cn/Article/details/giexwigkp.sHtML

[G08] 静态方法与属性
来源：http://www.share.hesvh.cn/Article/details/gmxivnvbu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.hesvh.cn/Article/details/gzzezufva.sHtML

PHP:  public static function f() {}
来源：http://3g.zdbjq.cn/Article/details/gtbvsfmkh.sHtML

JS:   static f() {}
来源：http://www.blog.hesvh.cn/Article/details/grroaxedw.sHtML

TS:   static f(): void {}
来源：http://read.share.hesvh.cn/Article/details/gnetcgarv.sHtML

Java: static void f() {}
来源：http://www.share.zdbjq.cn/Article/details/gyjmeupox.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.zdbjq.cn/Article/details/gopghfoyh.sHtML

Ruby: def self.f; end
来源：http://www.m.share.fehbvm.com/Article/details/gpgteheil.sHtML

C#:   public static void F() {}
来源：http://www.share.zdbjq.cn/Article/details/gickidnku.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.zdbjq.cn/Article/details/gdudeifky.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/gdgeshevq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.fehbvm.com/Article/details/glzdbnopt.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.hesvh.cn/Article/details/gwsfhatgk.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.hesvh.cn/Article/details/gujdguebj.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gpbcwbbae.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.hesvh.cn/Article/details/gjljvowyy.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.hesvh.cn/Article/details/gbdrjnpqd.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.fehbvm.com/Article/details/gvsiomuyi.sHtML

[G10] 访问控制
来源：http://wap.fehbvm.com/Article/details/gwbamjjhr.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.zdbjq.cn/Article/details/gnculpepl.sHtML

PHP:  public / protected / private
来源：http://3g.hesvh.cn/Article/details/gxunjdthy.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.zdbjq.cn/Article/details/glbzbrmyb.sHtML

TS:   public / protected / private
来源：http://read.share.fehbvm.com/Article/details/ggfguvkqg.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fehbvm.com/Article/details/goodtgutq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.zdbjq.cn/Article/details/gbkdpexzu.sHtML

Ruby: public / protected / private
来源：http://wap.zdbjq.cn/Article/details/glcgywysk.sHtML

C#:   public / protected / private / internal
来源：http://blog.zdbjq.cn/Article/details/gpqmkrhkq.sHtML

[G11] getter / setter
来源：http://wap.zdbjq.cn/Article/details/gtdwikrms.sHtML

Py:   @property 与 @x.setter
来源：http://baike.zdbjq.cn/Article/details/gmhrxupcy.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gbftifhhe.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gofrjeebe.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.fehbvm.com/Article/details/ghiajayns.sHtML

Java: public String getName() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gthqhhibl.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gjmxhtgoc.sHtML

Ruby: attr_accessor :name
来源：http://m.share.zdbjq.cn/Article/details/gikmxuabz.sHtML

C#:   public string Name { get; set; }
来源：http://wap.hesvh.cn/Article/details/gvwjlxysm.sHtML

[G12] 对象转字符串
来源：http://wap.zdbjq.cn/Article/details/gejxcxbrh.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gylrdrvpk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/goneysohg.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gbflgdoji.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/geryaveig.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.hesvh.cn/Article/details/ggqghxhiq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gpsuowjou.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/ggotryzzo.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gyzglanhx.sHtML

[G13] 判断对象类型
来源：http://baike.fehbvm.com/Article/details/gbcvzstvg.sHtML


<!-- 参考信息 -->