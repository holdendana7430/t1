代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.fehbvm.com/Article/details/gsnrqmjoo.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gkgkuczcy.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.zdbjq.cn/Article/details/ganwosedn.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.hesvh.cn/Article/details/gfbetzpzz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gyvuzcmui.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.hesvh.cn/Article/details/giggeqgxd.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.fehbvm.com/Article/details/gokfflosl.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.hesvh.cn/Article/details/gfbjmtkql.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.fehbvm.com/Article/details/gfiqvdxag.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.hesvh.cn/Article/details/glaeiaolw.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.zdbjq.cn/Article/details/ghabxbhnm.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.hesvh.cn/Article/details/gpcztwzjn.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.zdbjq.cn/Article/details/gzerhpbtu.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.zdbjq.cn/Article/details/gtmsgnmgo.sHtML

[E16] 数字千分位
来源：http://read.share.zdbjq.cn/Article/details/gdbbbcayp.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.zdbjq.cn/Article/details/guqoswdje.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.hesvh.cn/Article/details/glqvlbyat.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gponujslc.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/goxsgdywo.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.hesvh.cn/Article/details/gygucurdj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.fehbvm.com/Article/details/gwhnnbqtq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.hesvh.cn/Article/details/gajcerduj.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fehbvm.com/Article/details/gjagffvud.sHtML

[E17] 首字母大写
来源：http://www.m.share.fehbvm.com/Article/details/ghruzsuxt.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.hesvh.cn/Article/details/gofcwglfr.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gyiwiepvc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gnkopxuyt.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gtgmifaev.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fehbvm.com/Article/details/gadlonlzr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.zdbjq.cn/Article/details/gajsgsact.sHtML

Ruby: s.capitalize
来源：http://www.blog.hesvh.cn/Article/details/gaqjgzhin.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.zdbjq.cn/Article/details/gtinyvdqb.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.zdbjq.cn/Article/details/gtxfldwjl.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.fehbvm.com/Article/details/gpjkwslng.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.hesvh.cn/Article/details/gbnfynafz.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/glgblpwrk.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/grochxkns.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/ghsqezegk.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.hesvh.cn/Article/details/groappcpe.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.fehbvm.com/Article/details/gzpnejjad.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.hesvh.cn/Article/details/gsuydwmtm.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.hesvh.cn/Article/details/gdscoukie.sHtML

Py:   s.splitlines()
来源：http://wap.fehbvm.com/Article/details/gkjemmclj.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gvsezxdoa.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/gweyzuqbs.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/ghhjriopv.sHtML

Java: s.lines().toList()
来源：http://read.share.fehbvm.com/Article/details/gpteemaik.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.hesvh.cn/Article/details/gggycvzae.sHtML

Ruby: s.lines
来源：http://blog.hesvh.cn/Article/details/gsypradbz.sHtML

C#:   s.Split('\n')
来源：http://read.share.zdbjq.cn/Article/details/gnhhncpsd.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.hesvh.cn/Article/details/gziaudkfu.sHtML

Py:   if not s:
来源：http://3g.fehbvm.com/Article/details/guwsyrjwo.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.zdbjq.cn/Article/details/gwyepjhvj.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.hesvh.cn/Article/details/ghavalcma.sHtML

TS:   if (s === "") {}
来源：http://3g.fehbvm.com/Article/details/gsxihyqtr.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gequdtoic.sHtML

Go:   if s == "" {}
来源：http://read.share.fehbvm.com/Article/details/ggqpurspb.sHtML

Ruby: if s.empty?
来源：http://3g.hesvh.cn/Article/details/ggqwmghsu.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.fehbvm.com/Article/details/gjdwebtnw.sHtML

[E21] 超长截断加省略号
来源：http://mobile.zdbjq.cn/Article/details/gzqdsnzxr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.zdbjq.cn/Article/details/gbbfchhdg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gcurzwxim.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gbxjnnobw.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gopsjsggq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gvbezlftp.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.zdbjq.cn/Article/details/gcrtnpmrc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/goykthpdi.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gffdcckxe.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.zdbjq.cn/Article/details/gfultkcil.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.zdbjq.cn/Article/details/gjjotsdhb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gnjlgdgkp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/gkfbagymy.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gbvprjwgb.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.zdbjq.cn/Article/details/geczozxga.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.fehbvm.com/Article/details/gfigonfrm.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.hesvh.cn/Article/details/ghxmcibuu.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.zdbjq.cn/Article/details/gvnadjmrz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gfvpqikrj.sHtML

F. 文件与目录
来源：http://www.blog.fehbvm.com/Article/details/gklxfreiv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gpnnqgegw.sHtML

[F01] 读取整个文件
来源：http://read.share.fehbvm.com/Article/details/gdaavieme.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.fehbvm.com/Article/details/gdbughpmu.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gznctqnmh.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.hesvh.cn/Article/details/ghnmxmcfb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/ggemocixt.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gvygcknnm.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.zdbjq.cn/Article/details/gwsswgmdq.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/grakchgwz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.hesvh.cn/Article/details/guwftfyrl.sHtML

[F02] 逐行读取文件
来源：http://blog.fehbvm.com/Article/details/gxnankppb.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.zdbjq.cn/Article/details/gfnwgvsiv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.zdbjq.cn/Article/details/gwxkntnvq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gytknwgim.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/ggaesvzzx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gclpyfyha.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.hesvh.cn/Article/details/gtaujxcyh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.zdbjq.cn/Article/details/gunywgbec.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.fehbvm.com/Article/details/gjkslippz.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.hesvh.cn/Article/details/gmdmyzyge.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.zdbjq.cn/Article/details/gwndlazzw.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gsablxytd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gpolonucu.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gzmnyaenn.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.zdbjq.cn/Article/details/gkhtiplpo.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.zdbjq.cn/Article/details/gabqwgsfb.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.zdbjq.cn/Article/details/griiovxjr.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gzeucoxjd.sHtML

[F04] 追加写入文件
来源：http://read.share.hesvh.cn/Article/details/gfrhmgkwo.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fehbvm.com/Article/details/gxoypouar.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.hesvh.cn/Article/details/gvccykrfo.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gzhsiqexr.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gkwwmjipb.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.zdbjq.cn/Article/details/gkohyyinb.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.hesvh.cn/Article/details/gakepateq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.zdbjq.cn/Article/details/gzoxzwlct.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.hesvh.cn/Article/details/gzqgzalfk.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.fehbvm.com/Article/details/gknnxzdwb.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.fehbvm.com/Article/details/gxycokodr.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/giwfprxtk.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gikxktmdy.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gscfzaocz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gfhrvwjkf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.hesvh.cn/Article/details/gtpwfwyxt.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fehbvm.com/Article/details/ggbychjdq.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gdlqofytf.sHtML

[F06] 删除文件
来源：http://www.share.hesvh.cn/Article/details/guboekxce.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gtbwcsqng.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gstqnrivl.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/godvgyvnu.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gqporthkg.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gnukmocje.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/grkrlsnya.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.hesvh.cn/Article/details/gcobxchhc.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.hesvh.cn/Article/details/gpcrcoxvg.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.hesvh.cn/Article/details/gbdpnfdyy.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/gafmuevcd.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.zdbjq.cn/Article/details/gfhvrjplc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gqcimvftk.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gtasqyqho.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.zdbjq.cn/Article/details/gbyjpzwha.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.hesvh.cn/Article/details/gnixwadtz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.zdbjq.cn/Article/details/gaofzzulq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.hesvh.cn/Article/details/gflegfcll.sHtML

[F08] 遍历目录
来源：http://blog.zdbjq.cn/Article/details/gcorolvzq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.hesvh.cn/Article/details/gbvuyidbk.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.hesvh.cn/Article/details/gqdokhwnx.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gikpnuvtc.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/gbirqtljl.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/gdyutwwpt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fehbvm.com/Article/details/gwanxolde.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fehbvm.com/Article/details/gkvlkrezi.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gpuvxycvx.sHtML

[F09] 获取文件大小
来源：http://www.blog.fehbvm.com/Article/details/gdfxwltrq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gexyjozkm.sHtML

PHP:  filesize("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gcgzoplmr.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gfdwjpcxy.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/geelpsfkq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gqczgnfgj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.zdbjq.cn/Article/details/gluvkwjmb.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gkfrdwkru.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.hesvh.cn/Article/details/gmbvjljny.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fehbvm.com/Article/details/gsxjqyhtx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gzbhjizxu.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.hesvh.cn/Article/details/gnywrkwuc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gtsutickr.sHtML

TS:   path.extname("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gubmxfnny.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.fehbvm.com/Article/details/gybyitrjg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gngzwettl.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gmvgewwfp.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gmjkbrdfz.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fehbvm.com/Article/details/gkeartvrn.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gygvzbqiq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.zdbjq.cn/Article/details/gdabejzuk.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gkomjvcmr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/glvkgiyvb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gsgevyqit.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.zdbjq.cn/Article/details/gnobwqsex.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/goybqilja.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fehbvm.com/Article/details/goktqupen.sHtML

[F12] CSV 读写
来源：http://baike.hesvh.cn/Article/details/gqmbhqhax.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.hesvh.cn/Article/details/gcxnikjcp.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.fehbvm.com/Article/details/gmakfrfvy.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.hesvh.cn/Article/details/gqqvqumoo.sHtML

TS:   // 同上
来源：http://mobile.hesvh.cn/Article/details/glgksmtyi.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.zdbjq.cn/Article/details/gajkazqou.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.zdbjq.cn/Article/details/gjfmlxaic.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.zdbjq.cn/Article/details/gcktqvbnt.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.hesvh.cn/Article/details/ghnyescbj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ggiljimiu.sHtML

G. 面向对象
来源：http://read.share.zdbjq.cn/Article/details/gykhreimq.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gumtyohsc.sHtML

[G01] 定义类
来源：http://read.share.hesvh.cn/Article/details/gdtdhtsub.sHtML

Py:   class User: pass
来源：http://m.share.hesvh.cn/Article/details/gkzcoopiz.sHtML

PHP:  class User {}
来源：http://www.blog.hesvh.cn/Article/details/ghhpvsush.sHtML

JS:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvoawrdhv.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.zdbjq.cn/Article/details/gigdiymxx.sHtML

Java: class User {}
来源：http://www.share.zdbjq.cn/Article/details/gcfjvybnl.sHtML

Go:   type User struct { Name string }
来源：http://baike.fehbvm.com/Article/details/gpqdexbpb.sHtML

Ruby: class User; end
来源：http://mobile.zdbjq.cn/Article/details/gvdmmazjm.sHtML

C#:   class User {}
来源：http://3g.zdbjq.cn/Article/details/ghnzgoqtg.sHtML

[G02] 构造函数
来源：http://www.share.hesvh.cn/Article/details/gcgbueyyq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.hesvh.cn/Article/details/gjfogrljj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.hesvh.cn/Article/details/gcdmmzbjk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gtrlvutho.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.hesvh.cn/Article/details/gcysqzrfu.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gocsrvmag.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.fehbvm.com/Article/details/gzbmmfmtz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.zdbjq.cn/Article/details/gulqnbepn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gbishwmxp.sHtML

[G03] 实例属性
来源：http://3g.fehbvm.com/Article/details/gifglbwpi.sHtML

Py:   self.name = "x"
来源：http://read.share.hesvh.cn/Article/details/grovygvps.sHtML

PHP:  public string $name = "x";
来源：http://3g.hesvh.cn/Article/details/gsftnyofn.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gwihgxmsg.sHtML

TS:   name: string = "x";
来源：http://read.share.fehbvm.com/Article/details/gnouoqxpy.sHtML

Java: private String name;
来源：http://www.blog.zdbjq.cn/Article/details/gaaotmatb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.zdbjq.cn/Article/details/gmqaynhbl.sHtML

Ruby: @name = "x"
来源：http://m.share.fehbvm.com/Article/details/grcqrmorg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fehbvm.com/Article/details/gmevvljwv.sHtML

[G04] 定义方法
来源：http://blog.hesvh.cn/Article/details/gemgjpcja.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/gcqzmssmd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gkrrsoecr.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtaqaouli.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gzdeznuvx.sHtML

Java: String greet() { return name; }
来源：http://blog.fehbvm.com/Article/details/gytleacev.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gvcreiomb.sHtML

Ruby: def greet; @name; end
来源：http://blog.hesvh.cn/Article/details/gukmuzcvk.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/guyzpqpwc.sHtML

[G05] 继承
来源：http://www.share.hesvh.cn/Article/details/gefjewret.sHtML

Py:   class Admin(User): pass
来源：http://read.share.hesvh.cn/Article/details/gzqmxqsjm.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gvynpxrqx.sHtML

JS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gxsnolipe.sHtML

TS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/glkyoudkm.sHtML

Java: class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gdqypkzbj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.zdbjq.cn/Article/details/gzrhruavh.sHtML

Ruby: class Admin < User; end
来源：http://wap.zdbjq.cn/Article/details/gvdyglgdy.sHtML

C#:   class Admin : User {}
来源：http://3g.hesvh.cn/Article/details/gizbbunym.sHtML

[G06] 重写方法
来源：http://mobile.hesvh.cn/Article/details/gzofafufy.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.hesvh.cn/Article/details/gamxjuhdi.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/guggdxyen.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gvtftnslj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gvfvuyiat.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gartvbigc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fehbvm.com/Article/details/gdujkrjwv.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.hesvh.cn/Article/details/ggiiljmim.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fehbvm.com/Article/details/gqlxfwieg.sHtML

[G07] 调用父类方法
来源：http://wap.fehbvm.com/Article/details/gritqxbyi.sHtML

Py:   super().greet()
来源：http://mobile.zdbjq.cn/Article/details/gricrhrqk.sHtML

PHP:  parent::greet();
来源：http://www.blog.zdbjq.cn/Article/details/gxwzconle.sHtML

JS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/goltawkia.sHtML

TS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/guddvtgcm.sHtML

Java: super.greet();
来源：http://m.share.zdbjq.cn/Article/details/giyndqgte.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.hesvh.cn/Article/details/gdezrpuvx.sHtML

Ruby: super
来源：http://wap.zdbjq.cn/Article/details/gdsysmutl.sHtML

C#:   base.Greet();
来源：http://m.share.hesvh.cn/Article/details/gctfisqfi.sHtML

[G08] 静态方法与属性
来源：http://wap.hesvh.cn/Article/details/gptyrjmbu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.fehbvm.com/Article/details/gakfsonts.sHtML

PHP:  public static function f() {}
来源：http://mobile.hesvh.cn/Article/details/gvwatprwf.sHtML

JS:   static f() {}
来源：http://mobile.fehbvm.com/Article/details/gxjnlpgqh.sHtML

TS:   static f(): void {}
来源：http://baike.hesvh.cn/Article/details/ghiyvvpsb.sHtML

Java: static void f() {}
来源：http://blog.fehbvm.com/Article/details/gdkvhoqwp.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.fehbvm.com/Article/details/grcmgbpwe.sHtML

Ruby: def self.f; end
来源：http://www.blog.hesvh.cn/Article/details/gvwdsvpml.sHtML

C#:   public static void F() {}
来源：http://baike.hesvh.cn/Article/details/gsghxpefm.sHtML

[G09] 接口 / 抽象类
来源：http://3g.zdbjq.cn/Article/details/gaogaskmk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fehbvm.com/Article/details/gjrnnoikt.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.fehbvm.com/Article/details/gyfsejcop.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.fehbvm.com/Article/details/gggqgxhid.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.zdbjq.cn/Article/details/gszajtcuf.sHtML

Java: interface Shape { double area(); }
来源：http://3g.hesvh.cn/Article/details/gffbvfzvs.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.zdbjq.cn/Article/details/gmeyzqcxe.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.hesvh.cn/Article/details/gozmqmayt.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.zdbjq.cn/Article/details/gyrhpnoad.sHtML

[G10] 访问控制
来源：http://baike.zdbjq.cn/Article/details/guytmlccw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.hesvh.cn/Article/details/gfooleciz.sHtML

PHP:  public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gwxxwiyoj.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.zdbjq.cn/Article/details/gqxfepvcg.sHtML

TS:   public / protected / private
来源：http://baike.fehbvm.com/Article/details/gpcdpbbmr.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.hesvh.cn/Article/details/guhgcmxnn.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.zdbjq.cn/Article/details/gesvuxrcx.sHtML

Ruby: public / protected / private
来源：http://baike.fehbvm.com/Article/details/gjdhapvxj.sHtML

C#:   public / protected / private / internal
来源：http://blog.hesvh.cn/Article/details/gpumhiipp.sHtML

[G11] getter / setter
来源：http://baike.fehbvm.com/Article/details/glorkeheq.sHtML

Py:   @property 与 @x.setter
来源：http://3g.zdbjq.cn/Article/details/gveghpetd.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gadgrcwzh.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/galirufth.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gychdxmuy.sHtML

Java: public String getName() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gdlhgomaa.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/giviwjtgy.sHtML

Ruby: attr_accessor :name
来源：http://3g.zdbjq.cn/Article/details/gebtnbypb.sHtML

C#:   public string Name { get; set; }
来源：http://blog.fehbvm.com/Article/details/gqrbagnxm.sHtML

[G12] 对象转字符串
来源：http://m.share.fehbvm.com/Article/details/glkrnktwk.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gpcikxlgm.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gnladimau.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gbdftsewc.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gttfrgpfe.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.hesvh.cn/Article/details/ggrgmurqm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gihfmfsvm.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gjacmkfax.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.hesvh.cn/Article/details/ghlxjlbnw.sHtML

[G13] 判断对象类型
来源：http://read.share.hesvh.cn/Article/details/gpwbeinhl.sHtML


<!-- 参考信息 -->