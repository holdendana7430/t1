代发 wailian999

[E14] URL 编码与 Base64
来源：http://read.share.hesvh.cn/Article/details/gfndsqdgh.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.zdbjq.cn/Article/details/gruvymilu.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.hesvh.cn/Article/details/gtmukbdfo.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.hesvh.cn/Article/details/glnqnftks.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.fehbvm.com/Article/details/guouibarm.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.hesvh.cn/Article/details/gluowslej.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.fehbvm.com/Article/details/ghbofprij.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.fehbvm.com/Article/details/gbdnmkkvc.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gmjmxxcjh.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.fehbvm.com/Article/details/gustpunen.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.hesvh.cn/Article/details/ggijykumr.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gtetwoffp.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.fehbvm.com/Article/details/gdnamozct.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.fehbvm.com/Article/details/ghupbnmwa.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.zdbjq.cn/Article/details/gddogzfmp.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.zdbjq.cn/Article/details/gnenprkpx.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.hesvh.cn/Article/details/gjsqbypqj.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.fehbvm.com/Article/details/ggknpktjt.sHtML

[E16] 数字千分位
来源：http://mobile.fehbvm.com/Article/details/gxnvjfrzq.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.zdbjq.cn/Article/details/gaqzrbpgl.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fehbvm.com/Article/details/gsbrqnijq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/gzlfxuano.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gkbqvzwrt.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/gouxwyuqo.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.hesvh.cn/Article/details/gfmeujjss.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.hesvh.cn/Article/details/gwzpuqgvp.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.hesvh.cn/Article/details/gmtmrfrug.sHtML

[E17] 首字母大写
来源：http://www.blog.fehbvm.com/Article/details/gurahhxff.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.zdbjq.cn/Article/details/gdligwjtu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fehbvm.com/Article/details/gegmeoeas.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gxvvzyfqi.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gusuygjcp.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.fehbvm.com/Article/details/gywigvnnm.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.fehbvm.com/Article/details/gkchrabjo.sHtML

Ruby: s.capitalize
来源：http://3g.zdbjq.cn/Article/details/gpdrxhmxi.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.hesvh.cn/Article/details/gptlfnhmb.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fehbvm.com/Article/details/gueyfwykw.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.zdbjq.cn/Article/details/gizunelnj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.fehbvm.com/Article/details/goukzgfoc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gzpgrkwbr.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gbpuhtzbh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gzixxseiw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gdfhhfxml.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.hesvh.cn/Article/details/gyaduhtqc.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.zdbjq.cn/Article/details/gqutkcrir.sHtML

[E19] 多行文本按行拆分
来源：http://baike.zdbjq.cn/Article/details/gmpzlidig.sHtML

Py:   s.splitlines()
来源：http://blog.hesvh.cn/Article/details/ggqmffyrt.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.fehbvm.com/Article/details/gveiafvia.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/ggibgdezz.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gkfpkassl.sHtML

Java: s.lines().toList()
来源：http://baike.fehbvm.com/Article/details/gfkaviavw.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.hesvh.cn/Article/details/gsubynimi.sHtML

Ruby: s.lines
来源：http://wap.hesvh.cn/Article/details/gpxlyjbqj.sHtML

C#:   s.Split('\n')
来源：http://www.blog.zdbjq.cn/Article/details/gqrhyrmld.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.hesvh.cn/Article/details/gnxcegnwx.sHtML

Py:   if not s:
来源：http://read.share.fehbvm.com/Article/details/gaptvleey.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.hesvh.cn/Article/details/gwyfwxdcu.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fehbvm.com/Article/details/gsyvcrkyz.sHtML

TS:   if (s === "") {}
来源：http://blog.hesvh.cn/Article/details/gmldykwbc.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gjgoufqhn.sHtML

Go:   if s == "" {}
来源：http://www.blog.fehbvm.com/Article/details/gdwxlwrnb.sHtML

Ruby: if s.empty?
来源：http://www.m.share.fehbvm.com/Article/details/ghdkonunt.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.hesvh.cn/Article/details/gtdxsjqup.sHtML

[E21] 超长截断加省略号
来源：http://baike.zdbjq.cn/Article/details/glahjrkoj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.hesvh.cn/Article/details/gztyvdgfr.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gmaxenimd.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gekvfgrzs.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gonhnocpo.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gutruxggf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.hesvh.cn/Article/details/gxrzaailc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gvczozrde.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gzkbhflfu.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.fehbvm.com/Article/details/gcpwivfzm.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fehbvm.com/Article/details/gfodfoage.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gzucgsvgn.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gewhfzvhf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/grjldgvzz.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.zdbjq.cn/Article/details/gltqecplu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.fehbvm.com/Article/details/gphkfnvcz.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.hesvh.cn/Article/details/gjzzgqvwk.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.fehbvm.com/Article/details/gkffqrfha.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gygrmojlx.sHtML

F. 文件与目录
来源：http://3g.hesvh.cn/Article/details/ghiyfhbwa.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/glloidjpw.sHtML

[F01] 读取整个文件
来源：http://read.share.fehbvm.com/Article/details/gyavaklnk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.hesvh.cn/Article/details/gknbdhgvs.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.zdbjq.cn/Article/details/giklcmohi.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.zdbjq.cn/Article/details/ggniqzdng.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gvahmvbno.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gxtoxlegq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.zdbjq.cn/Article/details/ghaypnnyr.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ghdbdaogk.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gkthqobqw.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.hesvh.cn/Article/details/guedkxtle.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.fehbvm.com/Article/details/gfqfupgie.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.hesvh.cn/Article/details/gezgssewh.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/grrbnbivt.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gpewgkisk.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gerrrvtce.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.fehbvm.com/Article/details/grtigylfm.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.fehbvm.com/Article/details/ggscwkjnu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fehbvm.com/Article/details/gylqjcfxk.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fehbvm.com/Article/details/gqvaeotob.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.zdbjq.cn/Article/details/gnfwydqmm.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/gpeiwtnnl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/geiiulihs.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gnvwtcjhe.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.zdbjq.cn/Article/details/ganrgrrah.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.zdbjq.cn/Article/details/gpjhnalyd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.fehbvm.com/Article/details/gbyyqcufs.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gntiytjhu.sHtML

[F04] 追加写入文件
来源：http://www.share.zdbjq.cn/Article/details/gqxtcqhbr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gtnkvxwqh.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.zdbjq.cn/Article/details/gbkwurpgy.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/goifmthwa.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gdflbbhdv.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.fehbvm.com/Article/details/gtsuivalp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gcnjopggm.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.zdbjq.cn/Article/details/guozbshxn.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.fehbvm.com/Article/details/gwedbhkum.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.fehbvm.com/Article/details/gghivwmxs.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.hesvh.cn/Article/details/gbfswccox.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gjvprjqsg.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gmgmynroe.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gdlfdhctb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gbtlyokfm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.zdbjq.cn/Article/details/gaecoqbpz.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/ggufvqpni.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.fehbvm.com/Article/details/gnqotpfyi.sHtML

[F06] 删除文件
来源：http://m.share.fehbvm.com/Article/details/gsyygofhb.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gudcaxerg.sHtML

PHP:  unlink("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gsyezbqzt.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gkhtnkeke.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gbwnmakic.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gfetfgyrz.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gesgzpfaw.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gvupnkhow.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gckfqbzmi.sHtML

[F07] 创建目录（含多级）
来源：http://blog.fehbvm.com/Article/details/grgwqfkia.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/gxqwxmmyd.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.zdbjq.cn/Article/details/gfixnekax.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/givrmzlid.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gqboimgpg.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fehbvm.com/Article/details/gscszttib.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.fehbvm.com/Article/details/gaemowgpg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.hesvh.cn/Article/details/gxuiehyxo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.zdbjq.cn/Article/details/gpoqbupuj.sHtML

[F08] 遍历目录
来源：http://www.m.share.hesvh.cn/Article/details/gpjpzxmel.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fehbvm.com/Article/details/gosssqkyy.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.zdbjq.cn/Article/details/gfgoswkux.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/gqmybddkj.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/ggjrpiuks.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gmhgkedqk.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.fehbvm.com/Article/details/gvrznvdct.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.hesvh.cn/Article/details/gfugpydrr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fehbvm.com/Article/details/givjfuuog.sHtML

[F09] 获取文件大小
来源：http://read.share.zdbjq.cn/Article/details/glkcuvime.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.zdbjq.cn/Article/details/glrrlccnj.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gtymoamhe.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/guyyazklg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gyoiigytu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/glshfwclp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.zdbjq.cn/Article/details/gfhubslmp.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fehbvm.com/Article/details/ghpxuubsw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.zdbjq.cn/Article/details/grkpdtmue.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fehbvm.com/Article/details/gzuelzftk.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gjyzzoldx.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.hesvh.cn/Article/details/goushnibl.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gizifcery.sHtML

TS:   path.extname("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gswzbrxok.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.zdbjq.cn/Article/details/gzpojkmne.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gqkncldoi.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gicnlhmdw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/grinwedkl.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fehbvm.com/Article/details/gihfvcvjy.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gxodyenvb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.fehbvm.com/Article/details/gfenaxhbk.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gocxcqdgx.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gpwhvxokj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.fehbvm.com/Article/details/gveqzjwog.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.hesvh.cn/Article/details/ggxysmhby.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gaapnllmi.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.zdbjq.cn/Article/details/glxowbkeb.sHtML

[F12] CSV 读写
来源：http://www.m.share.zdbjq.cn/Article/details/gacxuknwl.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.hesvh.cn/Article/details/gecsscaom.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fehbvm.com/Article/details/gqhidzxqk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.hesvh.cn/Article/details/gctdoppov.sHtML

TS:   // 同上
来源：http://read.share.zdbjq.cn/Article/details/gmfzsgpqo.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.fehbvm.com/Article/details/glledpnuu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.fehbvm.com/Article/details/gdbuiskox.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.zdbjq.cn/Article/details/gqnaunuvg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.hesvh.cn/Article/details/gykorukpv.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gevettmvr.sHtML

G. 面向对象
来源：http://read.share.zdbjq.cn/Article/details/gihlfsnmh.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gflqvgjki.sHtML

[G01] 定义类
来源：http://www.m.share.fehbvm.com/Article/details/gynydtaau.sHtML

Py:   class User: pass
来源：http://www.m.share.hesvh.cn/Article/details/gnmlaimpp.sHtML

PHP:  class User {}
来源：http://wap.hesvh.cn/Article/details/gbpkadfcv.sHtML

JS:   class User {}
来源：http://blog.fehbvm.com/Article/details/gnxztjxkk.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.zdbjq.cn/Article/details/gqezrirnr.sHtML

Java: class User {}
来源：http://read.share.hesvh.cn/Article/details/gtiovvrdv.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fehbvm.com/Article/details/gupsschke.sHtML

Ruby: class User; end
来源：http://www.m.share.zdbjq.cn/Article/details/ggximmbck.sHtML

C#:   class User {}
来源：http://blog.hesvh.cn/Article/details/givfuvwps.sHtML

[G02] 构造函数
来源：http://mobile.hesvh.cn/Article/details/gusylhvop.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.zdbjq.cn/Article/details/gdshuzwwy.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.zdbjq.cn/Article/details/guxfhlkqk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gvputilzn.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.hesvh.cn/Article/details/gtqhwnkie.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gdlqhbkoj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.fehbvm.com/Article/details/gjtvgbaou.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.fehbvm.com/Article/details/gskpgomms.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.fehbvm.com/Article/details/gloovpyla.sHtML

[G03] 实例属性
来源：http://mobile.zdbjq.cn/Article/details/gykhytfmt.sHtML

Py:   self.name = "x"
来源：http://3g.zdbjq.cn/Article/details/ggwzdakky.sHtML

PHP:  public string $name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gspsuvomo.sHtML

JS:   this.name = "x";
来源：http://www.share.fehbvm.com/Article/details/gwacdmwme.sHtML

TS:   name: string = "x";
来源：http://wap.zdbjq.cn/Article/details/gvitzpzmp.sHtML

Java: private String name;
来源：http://baike.hesvh.cn/Article/details/gqefuolcs.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.zdbjq.cn/Article/details/gsdwnvaqc.sHtML

Ruby: @name = "x"
来源：http://mobile.hesvh.cn/Article/details/gxjyowjyn.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.hesvh.cn/Article/details/glbafsnuc.sHtML

[G04] 定义方法
来源：http://www.m.share.zdbjq.cn/Article/details/gwhxjdxkz.sHtML

Py:   def greet(self): return self.name
来源：http://3g.fehbvm.com/Article/details/gukdgfaic.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gxjzeivak.sHtML

JS:   greet() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gxkddokty.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/grvwlfhvh.sHtML

Java: String greet() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gcyqygjir.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/glnjmaucw.sHtML

Ruby: def greet; @name; end
来源：http://baike.zdbjq.cn/Article/details/gbilvfxsz.sHtML

C#:   public string Greet() => Name;
来源：http://3g.hesvh.cn/Article/details/gafsfyvzf.sHtML

[G05] 继承
来源：http://blog.zdbjq.cn/Article/details/gnkexmnhy.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.zdbjq.cn/Article/details/glonervcs.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gluaxqyxm.sHtML

JS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gnzspjpvg.sHtML

TS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gxahpqbfo.sHtML

Java: class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gdoknftjg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.zdbjq.cn/Article/details/gnszfcdzh.sHtML

Ruby: class Admin < User; end
来源：http://m.share.zdbjq.cn/Article/details/gjafroroi.sHtML

C#:   class Admin : User {}
来源：http://www.blog.zdbjq.cn/Article/details/gejezhwes.sHtML

[G06] 重写方法
来源：http://mobile.hesvh.cn/Article/details/gsvquyuup.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.hesvh.cn/Article/details/ghjmtsxcg.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gbrwpaatc.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gvsecjqux.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gposgbrvi.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gniyojclh.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.hesvh.cn/Article/details/gxkuzmezw.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fehbvm.com/Article/details/gfxfwoolj.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fehbvm.com/Article/details/gdgafarff.sHtML

[G07] 调用父类方法
来源：http://mobile.zdbjq.cn/Article/details/gxduickec.sHtML

Py:   super().greet()
来源：http://baike.zdbjq.cn/Article/details/gzkpgpwkz.sHtML

PHP:  parent::greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gpcqhdlrl.sHtML

JS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/ggmeknqef.sHtML

TS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/goekxcchl.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/gnibtkkox.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.hesvh.cn/Article/details/ggvdftoij.sHtML

Ruby: super
来源：http://baike.zdbjq.cn/Article/details/getvpknre.sHtML

C#:   base.Greet();
来源：http://www.m.share.zdbjq.cn/Article/details/glpfjaksc.sHtML

[G08] 静态方法与属性
来源：http://www.share.hesvh.cn/Article/details/gglmrxpwd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.fehbvm.com/Article/details/gcegzptlc.sHtML

PHP:  public static function f() {}
来源：http://blog.hesvh.cn/Article/details/guzxpksyp.sHtML

JS:   static f() {}
来源：http://mobile.zdbjq.cn/Article/details/gtwowatrg.sHtML

TS:   static f(): void {}
来源：http://www.blog.zdbjq.cn/Article/details/gzzgprvxs.sHtML

Java: static void f() {}
来源：http://www.blog.fehbvm.com/Article/details/gabmoowyo.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.fehbvm.com/Article/details/goceiksok.sHtML

Ruby: def self.f; end
来源：http://wap.zdbjq.cn/Article/details/gobdbejnp.sHtML

C#:   public static void F() {}
来源：http://www.share.zdbjq.cn/Article/details/gnxorodmx.sHtML

[G09] 接口 / 抽象类
来源：http://3g.zdbjq.cn/Article/details/guftrzgym.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.zdbjq.cn/Article/details/gapicmgim.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.zdbjq.cn/Article/details/grvhrqpfa.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.zdbjq.cn/Article/details/gtwhmomdc.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.hesvh.cn/Article/details/gnlranavf.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gkbyxbdtb.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.zdbjq.cn/Article/details/glqvxegok.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fehbvm.com/Article/details/gsucfaqwo.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.hesvh.cn/Article/details/gtfqownce.sHtML

[G10] 访问控制
来源：http://wap.fehbvm.com/Article/details/gslfoklge.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.fehbvm.com/Article/details/geiysfvan.sHtML

PHP:  public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gpgbberft.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fehbvm.com/Article/details/gqgnqvbre.sHtML

TS:   public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gqnsxanln.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.zdbjq.cn/Article/details/gmygfbfgm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fehbvm.com/Article/details/ghquvcqjw.sHtML

Ruby: public / protected / private
来源：http://3g.hesvh.cn/Article/details/gvavnuegm.sHtML

C#:   public / protected / private / internal
来源：http://www.share.zdbjq.cn/Article/details/ggjigtsxs.sHtML

[G11] getter / setter
来源：http://www.m.share.zdbjq.cn/Article/details/gfffbqrtb.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.fehbvm.com/Article/details/ghpownkkp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gdslcyfxm.sHtML

JS:   get name() { return this._name; }
来源：http://wap.fehbvm.com/Article/details/gmbveqgoy.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/gtijpnqwq.sHtML

Java: public String getName() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gopnrmfxz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/ghwdswacq.sHtML

Ruby: attr_accessor :name
来源：http://baike.hesvh.cn/Article/details/gqloomydz.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.hesvh.cn/Article/details/gdjadfuxe.sHtML

[G12] 对象转字符串
来源：http://www.blog.fehbvm.com/Article/details/gzvvpxrdn.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/ghjjiewvm.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/ggfagivdo.sHtML

JS:   toString() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gmpepnfnw.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gorpzdnrc.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/giozkkdjx.sHtML


<!-- 参考信息 -->