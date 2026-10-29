代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.hesvh.cn/Article/details/gawuamqmy.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gctiooibj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.hesvh.cn/Article/details/gxbxicvsz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.zdbjq.cn/Article/details/gcbplehzg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.fehbvm.com/Article/details/girexormt.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.hesvh.cn/Article/details/gylcyecsm.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fehbvm.com/Article/details/gyhqmamfr.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.zdbjq.cn/Article/details/ggarpwqrm.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.fehbvm.com/Article/details/gyrhagawr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.fehbvm.com/Article/details/gevzgakph.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fehbvm.com/Article/details/gsqgxgbln.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.zdbjq.cn/Article/details/grahhqkdd.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.hesvh.cn/Article/details/gzhxueezx.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.zdbjq.cn/Article/details/ggtnkafot.sHtML

[E16] 数字千分位
来源：http://wap.fehbvm.com/Article/details/gdzkeqvmh.sHtML

Py:   f"{1234567:,}"
来源：http://baike.fehbvm.com/Article/details/gkswthfaq.sHtML

PHP:  number_format(1234567);
来源：http://wap.zdbjq.cn/Article/details/gykgqqtmw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gcrxlbfhi.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/glowzqkxf.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/ghpwdqgtj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.fehbvm.com/Article/details/gqpzmqgsc.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.zdbjq.cn/Article/details/ggqbieesf.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.hesvh.cn/Article/details/gpxfveook.sHtML

[E17] 首字母大写
来源：http://m.share.hesvh.cn/Article/details/gvavjzemj.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.hesvh.cn/Article/details/gddvgshvf.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.zdbjq.cn/Article/details/gjvtkopmf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gvabuwnqt.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/gbyejzobm.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.hesvh.cn/Article/details/guqokkxsm.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.fehbvm.com/Article/details/grgtellkp.sHtML

Ruby: s.capitalize
来源：http://www.blog.zdbjq.cn/Article/details/gbsuhcuoz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.zdbjq.cn/Article/details/gyhzzyvub.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fehbvm.com/Article/details/ggkahvqbi.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.hesvh.cn/Article/details/ghoqyzlnu.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.hesvh.cn/Article/details/gidxdduez.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gazqobijc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gzcbositj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/ggneysugy.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.hesvh.cn/Article/details/geoxqjkcd.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.fehbvm.com/Article/details/gogcscywq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.hesvh.cn/Article/details/gtaytzvgy.sHtML

[E19] 多行文本按行拆分
来源：http://blog.hesvh.cn/Article/details/gmtjzpthm.sHtML

Py:   s.splitlines()
来源：http://wap.fehbvm.com/Article/details/gaxiizhji.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gfbwtuljh.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/gafggnegl.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/ggylphfii.sHtML

Java: s.lines().toList()
来源：http://blog.zdbjq.cn/Article/details/gxgzazioy.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.zdbjq.cn/Article/details/gbnupmqlo.sHtML

Ruby: s.lines
来源：http://www.blog.zdbjq.cn/Article/details/gyqrhxgrj.sHtML

C#:   s.Split('\n')
来源：http://m.share.fehbvm.com/Article/details/ggqgalvnq.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.hesvh.cn/Article/details/ghptintzg.sHtML

Py:   if not s:
来源：http://read.share.fehbvm.com/Article/details/gegxzibyz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.hesvh.cn/Article/details/goqzfandp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.zdbjq.cn/Article/details/gzqajtsth.sHtML

TS:   if (s === "") {}
来源：http://www.blog.hesvh.cn/Article/details/gpybuwguz.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gilaiiqel.sHtML

Go:   if s == "" {}
来源：http://www.m.share.hesvh.cn/Article/details/gupqjrgxc.sHtML

Ruby: if s.empty?
来源：http://m.share.hesvh.cn/Article/details/goamiomfg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.hesvh.cn/Article/details/glliuitvw.sHtML

[E21] 超长截断加省略号
来源：http://wap.fehbvm.com/Article/details/gaabgawoo.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.zdbjq.cn/Article/details/gpewgzgcl.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gscptywes.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gofnetdau.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gmzxsedoe.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gernacgsw.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.fehbvm.com/Article/details/gvzlxidzv.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gdlsfjcwq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/glnlycmax.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.hesvh.cn/Article/details/gchdoywzz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.zdbjq.cn/Article/details/ggtlgmxjc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/grveambmb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gdpxcykfn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/gbasfdejo.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.fehbvm.com/Article/details/gnzsfeubg.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.fehbvm.com/Article/details/ghqqnlras.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.fehbvm.com/Article/details/giqbibdhm.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.fehbvm.com/Article/details/glgmchyim.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gmgsxfqxm.sHtML

F. 文件与目录
来源：http://wap.fehbvm.com/Article/details/gideosshv.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gjxadfkct.sHtML

[F01] 读取整个文件
来源：http://m.share.zdbjq.cn/Article/details/gpwbvktor.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.zdbjq.cn/Article/details/gqwjktsib.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gqazctodi.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.fehbvm.com/Article/details/glwmxoopz.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gndnykmms.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gyyxtltsm.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.hesvh.cn/Article/details/gqwxopcpp.sHtML

Ruby: File.read("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gakwaejqj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gepjlzauq.sHtML

[F02] 逐行读取文件
来源：http://www.share.zdbjq.cn/Article/details/gnthwadvn.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.zdbjq.cn/Article/details/grfqlwaip.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.fehbvm.com/Article/details/gbtajhbbt.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxvxoarxx.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gdlgykocp.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gvalbcqfx.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.hesvh.cn/Article/details/ggthshwck.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.hesvh.cn/Article/details/gfqlbbrlg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fehbvm.com/Article/details/gspndtpri.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fehbvm.com/Article/details/gwugvnndf.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.hesvh.cn/Article/details/gfzwpekdo.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gehvklyce.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gjxvdfyud.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gwarhkefi.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.fehbvm.com/Article/details/ggloiugcw.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.zdbjq.cn/Article/details/galzhbxfw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.zdbjq.cn/Article/details/gwmknwwus.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gubpofaic.sHtML

[F04] 追加写入文件
来源：http://m.share.hesvh.cn/Article/details/gnfmdssiz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.zdbjq.cn/Article/details/gagcxpitr.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.zdbjq.cn/Article/details/gndtzhlub.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/ganujmoyb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/gmxdeildn.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.zdbjq.cn/Article/details/gtlshldxu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gupbtpyhw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fehbvm.com/Article/details/gyeauahuh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.zdbjq.cn/Article/details/ghsnceryp.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gueklcuxr.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.hesvh.cn/Article/details/gmeksytwg.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gimxbzmjs.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gszbjgezx.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/guzewmufv.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gdzoqtnab.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fehbvm.com/Article/details/gwhnmpcga.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gojdkeicz.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gvptairaj.sHtML

[F06] 删除文件
来源：http://www.share.fehbvm.com/Article/details/gvfjhdlyh.sHtML

Py:   os.remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gzvtcaotb.sHtML

PHP:  unlink("a.txt");
来源：http://wap.hesvh.cn/Article/details/gqtonmqzy.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gjpltssub.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gcttglbta.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gjbuuuflh.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gihulwaaa.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gsoqniekj.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.fehbvm.com/Article/details/gsepnhxhk.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.hesvh.cn/Article/details/gfofkedak.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/gvrpogjml.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.fehbvm.com/Article/details/gpeuazzdh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/gceescdee.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gdlfwwcly.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.fehbvm.com/Article/details/guluogyok.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fehbvm.com/Article/details/gggomizec.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.zdbjq.cn/Article/details/gypbigshm.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.hesvh.cn/Article/details/gqvlzshvk.sHtML

[F08] 遍历目录
来源：http://read.share.fehbvm.com/Article/details/grebplibe.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.fehbvm.com/Article/details/ghlspvpwy.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.hesvh.cn/Article/details/gngvcnrox.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gtfytxyur.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/grujvcvmb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/gcfcwamlx.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.hesvh.cn/Article/details/gussxotqo.sHtML

Ruby: Dir.children("dir")
来源：http://wap.hesvh.cn/Article/details/giumlvbfn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fehbvm.com/Article/details/gpdayzjdd.sHtML

[F09] 获取文件大小
来源：http://m.share.fehbvm.com/Article/details/gbbbplkcx.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gzwcjxvgi.sHtML

PHP:  filesize("a.txt");
来源：http://blog.hesvh.cn/Article/details/gysixnpet.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gfavlocsg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gyjimebfn.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gciyverxk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.hesvh.cn/Article/details/girztbouk.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fehbvm.com/Article/details/ganlwwfmb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.zdbjq.cn/Article/details/gndblrqwh.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fehbvm.com/Article/details/gwjersccp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/goexhatub.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.hesvh.cn/Article/details/gyzwerkiz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gtzjbzudm.sHtML

TS:   path.extname("a.txt")
来源：http://3g.hesvh.cn/Article/details/gxlfsvqbj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.hesvh.cn/Article/details/gztsaogef.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gamektzzj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gikbpeiit.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gqlasublk.sHtML

[F11] 复制与移动文件
来源：http://wap.hesvh.cn/Article/details/gbbbwgdnc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/ggoldlbld.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.hesvh.cn/Article/details/grpdhdwuu.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gwhfmdmab.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gricqyptt.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gffrffbxa.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.fehbvm.com/Article/details/gzpmhwuoz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gtuldamqu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fehbvm.com/Article/details/girirufzf.sHtML

[F12] CSV 读写
来源：http://baike.fehbvm.com/Article/details/ghxnbklly.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.fehbvm.com/Article/details/ginziueym.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.fehbvm.com/Article/details/gtrmvpwij.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.hesvh.cn/Article/details/gqhcictnw.sHtML

TS:   // 同上
来源：http://www.blog.hesvh.cn/Article/details/gvfvvjlvj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.hesvh.cn/Article/details/gsotxihpj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.hesvh.cn/Article/details/gvprpnobb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.hesvh.cn/Article/details/gtalhmjof.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fehbvm.com/Article/details/glvkjidar.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwdtvqwbo.sHtML

G. 面向对象
来源：http://www.blog.fehbvm.com/Article/details/gjbiqcpcb.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqahbcvkl.sHtML

[G01] 定义类
来源：http://mobile.fehbvm.com/Article/details/gxemvkbxl.sHtML

Py:   class User: pass
来源：http://3g.hesvh.cn/Article/details/gojadnibp.sHtML

PHP:  class User {}
来源：http://read.share.hesvh.cn/Article/details/gpqvmbgec.sHtML

JS:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gljhtbnrg.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.hesvh.cn/Article/details/gouhkasqa.sHtML

Java: class User {}
来源：http://3g.hesvh.cn/Article/details/gifkwtgbb.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/gljnpdzgm.sHtML

Ruby: class User; end
来源：http://blog.zdbjq.cn/Article/details/gppymwuqa.sHtML

C#:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gjpvbtypj.sHtML

[G02] 构造函数
来源：http://blog.zdbjq.cn/Article/details/gniecmptr.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.hesvh.cn/Article/details/gnxhlzloc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.hesvh.cn/Article/details/gavtsatkj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gawzyctal.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.zdbjq.cn/Article/details/gbvurwlri.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gqmktdvej.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/grdlgrzql.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.hesvh.cn/Article/details/gxibtgdje.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.fehbvm.com/Article/details/gzlhaehcg.sHtML

[G03] 实例属性
来源：http://www.m.share.zdbjq.cn/Article/details/ggzgtsfzg.sHtML

Py:   self.name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gbsijcxnu.sHtML

PHP:  public string $name = "x";
来源：http://read.share.hesvh.cn/Article/details/gyxoacyzi.sHtML

JS:   this.name = "x";
来源：http://3g.hesvh.cn/Article/details/gkdeohuxt.sHtML

TS:   name: string = "x";
来源：http://mobile.fehbvm.com/Article/details/gcbqjhcfj.sHtML

Java: private String name;
来源：http://www.share.fehbvm.com/Article/details/gryctceni.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fehbvm.com/Article/details/giuewcklb.sHtML

Ruby: @name = "x"
来源：http://blog.zdbjq.cn/Article/details/gdwonbykh.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.zdbjq.cn/Article/details/grorgsewh.sHtML

[G04] 定义方法
来源：http://mobile.hesvh.cn/Article/details/gcjvssivt.sHtML

Py:   def greet(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gfkwmwpdr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/glmbuilcc.sHtML

JS:   greet() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gcotufikv.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gryyyimza.sHtML

Java: String greet() { return name; }
来源：http://baike.hesvh.cn/Article/details/ghjxthkvd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gxllgzhur.sHtML

Ruby: def greet; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gmrchtyic.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fehbvm.com/Article/details/gtpzoovhu.sHtML

[G05] 继承
来源：http://mobile.zdbjq.cn/Article/details/gztmmzppj.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.hesvh.cn/Article/details/gtllbbnow.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gomrzhpgc.sHtML

JS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gyfuafeld.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gefqshcti.sHtML

Java: class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/guffnoctl.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.zdbjq.cn/Article/details/gyrtlqdgn.sHtML

Ruby: class Admin < User; end
来源：http://wap.zdbjq.cn/Article/details/gfhnqopmy.sHtML

C#:   class Admin : User {}
来源：http://www.share.zdbjq.cn/Article/details/gprugmfxt.sHtML

[G06] 重写方法
来源：http://wap.fehbvm.com/Article/details/gjmlkxjlf.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.zdbjq.cn/Article/details/gdmaetdaa.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gdetkgfzj.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gpuunyekl.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gynskizjn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gvalejsjx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.fehbvm.com/Article/details/gvonrmoql.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.hesvh.cn/Article/details/gdyqompdf.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fehbvm.com/Article/details/grwapxjkv.sHtML

[G07] 调用父类方法
来源：http://wap.fehbvm.com/Article/details/gnplyyvtw.sHtML

Py:   super().greet()
来源：http://m.share.fehbvm.com/Article/details/gkxshjuoa.sHtML

PHP:  parent::greet();
来源：http://3g.fehbvm.com/Article/details/godgchjnw.sHtML

JS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gztqoimbr.sHtML

TS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gtiaettqp.sHtML

Java: super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/goivwzlmw.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fehbvm.com/Article/details/gxlwhzuoz.sHtML

Ruby: super
来源：http://blog.hesvh.cn/Article/details/ganabinpi.sHtML

C#:   base.Greet();
来源：http://mobile.hesvh.cn/Article/details/gibprgynw.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.fehbvm.com/Article/details/gshmnuire.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.zdbjq.cn/Article/details/graepzhzj.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gblfnxnqp.sHtML

JS:   static f() {}
来源：http://wap.fehbvm.com/Article/details/gooqsexgm.sHtML

TS:   static f(): void {}
来源：http://3g.hesvh.cn/Article/details/gocbcslef.sHtML

Java: static void f() {}
来源：http://mobile.zdbjq.cn/Article/details/gaxgjvxqs.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.fehbvm.com/Article/details/gzsobyssr.sHtML

Ruby: def self.f; end
来源：http://3g.hesvh.cn/Article/details/gvbcylxsm.sHtML

C#:   public static void F() {}
来源：http://www.share.fehbvm.com/Article/details/ghsrsugap.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.zdbjq.cn/Article/details/grnvoxtdr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fehbvm.com/Article/details/gqyjlujqf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.zdbjq.cn/Article/details/gjkdyxgke.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.hesvh.cn/Article/details/ghbwedkcc.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.fehbvm.com/Article/details/ggpgwjryn.sHtML

Java: interface Shape { double area(); }
来源：http://wap.zdbjq.cn/Article/details/grkrsqkyo.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.zdbjq.cn/Article/details/gpedfvsyi.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.zdbjq.cn/Article/details/gjndsuyub.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.zdbjq.cn/Article/details/glrbxomzq.sHtML

[G10] 访问控制
来源：http://read.share.fehbvm.com/Article/details/gvxdxkfyr.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.hesvh.cn/Article/details/gqyltspwq.sHtML

PHP:  public / protected / private
来源：http://3g.hesvh.cn/Article/details/gnkwssnoi.sHtML

JS:   #private 字段；其余公开
来源：http://3g.zdbjq.cn/Article/details/gpxjonfvi.sHtML

TS:   public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gjdzsnobr.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.hesvh.cn/Article/details/gjdbkbqtb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.hesvh.cn/Article/details/gdeqxuisv.sHtML

Ruby: public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gbgkpfslm.sHtML

C#:   public / protected / private / internal
来源：http://m.share.zdbjq.cn/Article/details/glhzfhwhi.sHtML

[G11] getter / setter
来源：http://read.share.hesvh.cn/Article/details/ghktaclxe.sHtML

Py:   @property 与 @x.setter
来源：http://wap.zdbjq.cn/Article/details/gxmqxipgh.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gwhhxrgww.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/ghdhaykvl.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gxpdqxuhf.sHtML

Java: public String getName() { return name; }
来源：http://3g.hesvh.cn/Article/details/gvkiqfldd.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/goieirjal.sHtML

Ruby: attr_accessor :name
来源：http://m.share.hesvh.cn/Article/details/gusvvfcbk.sHtML

C#:   public string Name { get; set; }
来源：http://3g.fehbvm.com/Article/details/grwvvttbk.sHtML

[G12] 对象转字符串
来源：http://3g.fehbvm.com/Article/details/gzpkddmnd.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gkareqtzv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gjgutvvnb.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gbpgtljxr.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gabscpoxx.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gxummpqgn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gfykvxeaq.sHtML

Ruby: def to_s; @name; end
来源：http://wap.hesvh.cn/Article/details/gwusbgrlc.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.fehbvm.com/Article/details/gayenzrjc.sHtML

[G13] 判断对象类型
来源：http://www.share.hesvh.cn/Article/details/gfzoxxqyq.sHtML


<!-- 参考信息 -->