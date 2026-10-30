代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gthjuwdwr.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.hesvh.cn/Article/details/goensznfg.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.zdbjq.cn/Article/details/gntysfckj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.hesvh.cn/Article/details/gfsleipye.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.hesvh.cn/Article/details/gbtexrlqb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fehbvm.com/Article/details/gavpzhlvm.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.fehbvm.com/Article/details/gzccbbsax.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.fehbvm.com/Article/details/gwdbmduzb.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.hesvh.cn/Article/details/gvpeqbcmi.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.hesvh.cn/Article/details/gmgbzovsk.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.fehbvm.com/Article/details/gjgfuaecy.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.hesvh.cn/Article/details/geznqbuoz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gtuwdxdsp.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.hesvh.cn/Article/details/gvvjwnbup.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.fehbvm.com/Article/details/gyizzhvgx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.fehbvm.com/Article/details/gbnsdjooz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.zdbjq.cn/Article/details/granqoiuj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.hesvh.cn/Article/details/gzbsaimhv.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.zdbjq.cn/Article/details/gccpxhxwl.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.zdbjq.cn/Article/details/gtxjcywbs.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.zdbjq.cn/Article/details/gwyvtdiva.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.fehbvm.com/Article/details/glgcmoliw.sHtML

[E16] 数字千分位
来源：http://www.blog.fehbvm.com/Article/details/giddeclap.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.hesvh.cn/Article/details/ghhenoxrf.sHtML

PHP:  number_format(1234567);
来源：http://3g.zdbjq.cn/Article/details/gvxizoudt.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/gmoxfpett.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gxgczorit.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/gyceuooxc.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.zdbjq.cn/Article/details/gtslhpjab.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.fehbvm.com/Article/details/gtcxilqdu.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.zdbjq.cn/Article/details/gftuhetdf.sHtML

[E17] 首字母大写
来源：http://mobile.zdbjq.cn/Article/details/gtefzrsba.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.hesvh.cn/Article/details/gvtnlgasp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.hesvh.cn/Article/details/gcsxqftut.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gyaudegno.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/gvcqoxbyi.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.fehbvm.com/Article/details/gkjudgucu.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.zdbjq.cn/Article/details/gswnwoegg.sHtML

Ruby: s.capitalize
来源：http://mobile.hesvh.cn/Article/details/gqajijlst.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.fehbvm.com/Article/details/gxvwjlvzs.sHtML

[E18] 模板占位符替换
来源：http://mobile.zdbjq.cn/Article/details/gyhhwrzks.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.zdbjq.cn/Article/details/gdjsycwnw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.zdbjq.cn/Article/details/gtwwzlugl.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gubqrmmlv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gmvsgqcbj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gkirarqae.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gjezkoiol.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.zdbjq.cn/Article/details/gxhxlxthp.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.zdbjq.cn/Article/details/gxxujyywj.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.hesvh.cn/Article/details/gvwlxuois.sHtML

Py:   s.splitlines()
来源：http://www.share.hesvh.cn/Article/details/gmhrgvwti.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.hesvh.cn/Article/details/gdoayjvuw.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/gmcafhplw.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gjmpgucqs.sHtML

Java: s.lines().toList()
来源：http://wap.fehbvm.com/Article/details/gmubvuwsm.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fehbvm.com/Article/details/gzqhcagro.sHtML

Ruby: s.lines
来源：http://wap.hesvh.cn/Article/details/gmywvgcyp.sHtML

C#:   s.Split('\n')
来源：http://www.share.hesvh.cn/Article/details/gyvlujhrm.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.zdbjq.cn/Article/details/gqakbbfmc.sHtML

Py:   if not s:
来源：http://www.share.fehbvm.com/Article/details/gujimwnbt.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.hesvh.cn/Article/details/gxhsmubsj.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.fehbvm.com/Article/details/gqfzlqpjn.sHtML

TS:   if (s === "") {}
来源：http://mobile.hesvh.cn/Article/details/gpcplofin.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gfykrtujm.sHtML

Go:   if s == "" {}
来源：http://baike.fehbvm.com/Article/details/goymaslla.sHtML

Ruby: if s.empty?
来源：http://m.share.zdbjq.cn/Article/details/gzcuwjiwj.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.hesvh.cn/Article/details/goxuqytrm.sHtML

[E21] 超长截断加省略号
来源：http://m.share.hesvh.cn/Article/details/gwmafhodp.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.zdbjq.cn/Article/details/gblbbekcd.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gieteznyb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gzgvfigqd.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gwwqzdybt.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gfobjtpme.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.zdbjq.cn/Article/details/grydrrnof.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gaxfwclzn.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gtsurhqpm.sHtML

[E22] 字节长度与字符长度
来源：http://baike.zdbjq.cn/Article/details/gplkfwjzb.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.fehbvm.com/Article/details/gjiubqkic.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/ggxqasyvs.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gxvdwkwjr.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gceareauh.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.fehbvm.com/Article/details/gkiwarcho.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.fehbvm.com/Article/details/guunpwvrh.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.hesvh.cn/Article/details/gnomzmfqb.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.fehbvm.com/Article/details/gqeqnssad.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/glviluzcp.sHtML

F. 文件与目录
来源：http://read.share.hesvh.cn/Article/details/gcadnvyis.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gtypmzruu.sHtML

[F01] 读取整个文件
来源：http://wap.fehbvm.com/Article/details/gjsswsywl.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.zdbjq.cn/Article/details/gtgquzcbo.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.fehbvm.com/Article/details/gwgkblckp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.zdbjq.cn/Article/details/gaerbyoua.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gbgmlfqtf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/geunhhlas.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.hesvh.cn/Article/details/ghcufaang.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gwgiokldb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.hesvh.cn/Article/details/gndvyybds.sHtML

[F02] 逐行读取文件
来源：http://mobile.zdbjq.cn/Article/details/ghjlhssci.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.fehbvm.com/Article/details/gwvxyemaw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.hesvh.cn/Article/details/gjlaihbuj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/govuyadsv.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gdpvduqsv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/ggnjrfxca.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.hesvh.cn/Article/details/gmlmnljba.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.hesvh.cn/Article/details/gyjmojunq.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.fehbvm.com/Article/details/gpdhduivb.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.hesvh.cn/Article/details/gkewvxphq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.hesvh.cn/Article/details/gouofpmdk.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gauxvegtd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/gnbowonrg.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gnfhnfkzn.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.fehbvm.com/Article/details/gyyujdtgl.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.fehbvm.com/Article/details/gcxrvygkg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.zdbjq.cn/Article/details/gtpjician.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/gtfvdsnnz.sHtML

[F04] 追加写入文件
来源：http://www.m.share.hesvh.cn/Article/details/grizpvzgc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gfuhrslkr.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.fehbvm.com/Article/details/ggigeclpu.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gbwputrmb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/gcbnymhjy.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.zdbjq.cn/Article/details/ghtfmdvuo.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.hesvh.cn/Article/details/gabtwkfvg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.zdbjq.cn/Article/details/gknxmveki.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.zdbjq.cn/Article/details/gwiyaaspo.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.hesvh.cn/Article/details/gbjzdzits.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.zdbjq.cn/Article/details/gekmbaywb.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gczgwkqzo.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gtcvjpopg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gtbjiseoc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gskrijrkz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.fehbvm.com/Article/details/gbxyxsgnm.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gtyuwfieq.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gnftwcsvw.sHtML

[F06] 删除文件
来源：http://3g.hesvh.cn/Article/details/gamlmmjnj.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gcsgrqkcd.sHtML

PHP:  unlink("a.txt");
来源：http://blog.fehbvm.com/Article/details/gajxpqqwp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gqjwoimtc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/grvqiquyt.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/ggeotjnip.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gfmoqcivm.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gfyhqfpbb.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gszfqcoev.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.hesvh.cn/Article/details/gwqalvbqv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/grskhebgf.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.hesvh.cn/Article/details/gekxplrsw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gvlfzrrph.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gdeuupdkq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.zdbjq.cn/Article/details/gppxsxwbi.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.hesvh.cn/Article/details/geijxgiom.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.hesvh.cn/Article/details/gugyhwkdi.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.hesvh.cn/Article/details/gwmjlfqsm.sHtML

[F08] 遍历目录
来源：http://3g.zdbjq.cn/Article/details/gyekfcuvd.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fehbvm.com/Article/details/gtmsyoxbj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.zdbjq.cn/Article/details/gnqmrgwrz.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gctzwxdwl.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/gbrywolxf.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gvrmlmekm.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.fehbvm.com/Article/details/gfqevfdig.sHtML

Ruby: Dir.children("dir")
来源：http://blog.fehbvm.com/Article/details/gklfwardz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.hesvh.cn/Article/details/gnpwrobth.sHtML

[F09] 获取文件大小
来源：http://baike.fehbvm.com/Article/details/gofugiglu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gdtdpgysa.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gfooiyamc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/ggkfsdumz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gpusftxtt.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/goqdsoraj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.zdbjq.cn/Article/details/gojdirutb.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gxwhxceld.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.hesvh.cn/Article/details/gviuoxuli.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.zdbjq.cn/Article/details/gxqkineat.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gxdqhsrli.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gsloauyrm.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gcjpnpsir.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/guzgyzupl.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.zdbjq.cn/Article/details/gnciothmh.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gppnrnnzb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/grpobpdle.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gtscsembe.sHtML

[F11] 复制与移动文件
来源：http://baike.fehbvm.com/Article/details/gouxttyeo.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ggawxqmuw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gdwrgjiqg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gjmwooobv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gzbwykjxe.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gizivtwha.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.fehbvm.com/Article/details/gwdxneeli.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gziknzuwq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.hesvh.cn/Article/details/gcfsxyorw.sHtML

[F12] CSV 读写
来源：http://m.share.fehbvm.com/Article/details/gnpbaxohy.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.fehbvm.com/Article/details/gcivwubuc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.zdbjq.cn/Article/details/ggaufrbmb.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.fehbvm.com/Article/details/gdlhldpxq.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/gcbowntrj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.zdbjq.cn/Article/details/guxaxmguz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fehbvm.com/Article/details/gvqojnkjq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fehbvm.com/Article/details/gpdsfhrcd.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.fehbvm.com/Article/details/gotjnqmdo.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gbeimocgn.sHtML

G. 面向对象
来源：http://m.share.hesvh.cn/Article/details/gainwxtey.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gjccyhnmv.sHtML

[G01] 定义类
来源：http://www.m.share.fehbvm.com/Article/details/gluqknbfz.sHtML

Py:   class User: pass
来源：http://wap.fehbvm.com/Article/details/gbeczqzri.sHtML

PHP:  class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gpxflphbg.sHtML

JS:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gfvvcegwe.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.zdbjq.cn/Article/details/galdfpjyn.sHtML

Java: class User {}
来源：http://3g.zdbjq.cn/Article/details/geexdmumu.sHtML

Go:   type User struct { Name string }
来源：http://3g.fehbvm.com/Article/details/gzmmeuqym.sHtML

Ruby: class User; end
来源：http://blog.hesvh.cn/Article/details/gdhrjjmzo.sHtML

C#:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gjizywzej.sHtML

[G02] 构造函数
来源：http://mobile.zdbjq.cn/Article/details/gcvfinynt.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fehbvm.com/Article/details/ghufpjhva.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.hesvh.cn/Article/details/gqsgkkfts.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/grbzayexb.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.hesvh.cn/Article/details/gcmiwcmot.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gqkxictnr.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.zdbjq.cn/Article/details/gvvndrbkz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fehbvm.com/Article/details/gesrqtlwo.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.hesvh.cn/Article/details/gtgksrgrd.sHtML

[G03] 实例属性
来源：http://www.m.share.zdbjq.cn/Article/details/gzjspkorh.sHtML

Py:   self.name = "x"
来源：http://3g.hesvh.cn/Article/details/grbbxqjwj.sHtML

PHP:  public string $name = "x";
来源：http://3g.zdbjq.cn/Article/details/ghhcvatfr.sHtML

JS:   this.name = "x";
来源：http://read.share.fehbvm.com/Article/details/gakyjcoii.sHtML

TS:   name: string = "x";
来源：http://3g.hesvh.cn/Article/details/gmyaiohrb.sHtML

Java: private String name;
来源：http://3g.hesvh.cn/Article/details/gxicaqjbu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fehbvm.com/Article/details/gwzsvkxjd.sHtML

Ruby: @name = "x"
来源：http://read.share.fehbvm.com/Article/details/gbjzvorbd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.hesvh.cn/Article/details/glqtyibuk.sHtML

[G04] 定义方法
来源：http://mobile.hesvh.cn/Article/details/ggfrexuux.sHtML

Py:   def greet(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gryasbqxw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/glhwfkhhn.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/glzughtlw.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/givdgsmxp.sHtML

Java: String greet() { return name; }
来源：http://3g.zdbjq.cn/Article/details/ggzfuxrli.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gwbnanlpp.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gwctrkrcu.sHtML

C#:   public string Greet() => Name;
来源：http://baike.fehbvm.com/Article/details/ggtpzowpk.sHtML

[G05] 继承
来源：http://wap.fehbvm.com/Article/details/ggbugehbd.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.zdbjq.cn/Article/details/gozlbmsag.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gmzmitvrr.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/geevxcjjj.sHtML

TS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gsxcycrxw.sHtML

Java: class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gprxyyjbm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.hesvh.cn/Article/details/ggnefewms.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.zdbjq.cn/Article/details/ggrcvstzx.sHtML

C#:   class Admin : User {}
来源：http://www.share.fehbvm.com/Article/details/gmjpxmskq.sHtML

[G06] 重写方法
来源：http://blog.fehbvm.com/Article/details/gqyjlskdc.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.zdbjq.cn/Article/details/gkxjzapgb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gdxwbpttd.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gvwdyfaxi.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gzmpmdrhp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/ghejmoqwh.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.hesvh.cn/Article/details/gfqzapxgh.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.fehbvm.com/Article/details/gzdajszph.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.fehbvm.com/Article/details/gyksgivtq.sHtML

[G07] 调用父类方法
来源：http://read.share.zdbjq.cn/Article/details/goabjtcrw.sHtML

Py:   super().greet()
来源：http://www.blog.zdbjq.cn/Article/details/goftrwivn.sHtML

PHP:  parent::greet();
来源：http://www.share.fehbvm.com/Article/details/ghvijjtyd.sHtML

JS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gtsauqutr.sHtML

TS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gzxruerim.sHtML

Java: super.greet();
来源：http://3g.zdbjq.cn/Article/details/gjvdsoqth.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.hesvh.cn/Article/details/guvdgusjs.sHtML

Ruby: super
来源：http://wap.hesvh.cn/Article/details/ghfxtjewv.sHtML

C#:   base.Greet();
来源：http://www.blog.zdbjq.cn/Article/details/gjulpckkw.sHtML

[G08] 静态方法与属性
来源：http://www.blog.zdbjq.cn/Article/details/gabpsiwlc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.zdbjq.cn/Article/details/gjcylbprj.sHtML

PHP:  public static function f() {}
来源：http://m.share.fehbvm.com/Article/details/gkavfzgzm.sHtML

JS:   static f() {}
来源：http://wap.fehbvm.com/Article/details/gwotkjgye.sHtML

TS:   static f(): void {}
来源：http://blog.zdbjq.cn/Article/details/ggrjjxnkz.sHtML

Java: static void f() {}
来源：http://3g.hesvh.cn/Article/details/gxkjddhvh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.fehbvm.com/Article/details/gltwktqkh.sHtML

Ruby: def self.f; end
来源：http://baike.zdbjq.cn/Article/details/gdshpbbpz.sHtML

C#:   public static void F() {}
来源：http://m.share.zdbjq.cn/Article/details/gescgahvx.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fehbvm.com/Article/details/gysrrewzm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.hesvh.cn/Article/details/ggzbddzns.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fehbvm.com/Article/details/gltyuhsoh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.hesvh.cn/Article/details/gizmbgxfb.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.hesvh.cn/Article/details/gisayjlqm.sHtML

Java: interface Shape { double area(); }
来源：http://baike.zdbjq.cn/Article/details/godycjwap.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.fehbvm.com/Article/details/gicbwxhtw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.zdbjq.cn/Article/details/gohauysku.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.zdbjq.cn/Article/details/goyfdbrkv.sHtML

[G10] 访问控制
来源：http://www.m.share.zdbjq.cn/Article/details/gctcnecya.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.zdbjq.cn/Article/details/gbauwzfit.sHtML

PHP:  public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gzyyittfk.sHtML

JS:   #private 字段；其余公开
来源：http://blog.hesvh.cn/Article/details/gxnazmfbz.sHtML

TS:   public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gxysplqrz.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.hesvh.cn/Article/details/gnrtwuohc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.hesvh.cn/Article/details/gqaqjbqpf.sHtML

Ruby: public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gkrnchgvs.sHtML

C#:   public / protected / private / internal
来源：http://3g.hesvh.cn/Article/details/gafsgrlye.sHtML

[G11] getter / setter
来源：http://m.share.zdbjq.cn/Article/details/gwxbuzrqd.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.zdbjq.cn/Article/details/gbxbxkhdq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/guavboitw.sHtML

JS:   get name() { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gbipehydw.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gmttzubty.sHtML

Java: public String getName() { return name; }
来源：http://blog.hesvh.cn/Article/details/gtrcbqrhr.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gcaudnokt.sHtML

Ruby: attr_accessor :name
来源：http://www.share.hesvh.cn/Article/details/gdbahwgxc.sHtML

C#:   public string Name { get; set; }
来源：http://baike.zdbjq.cn/Article/details/gmncvldfn.sHtML

[G12] 对象转字符串
来源：http://read.share.hesvh.cn/Article/details/gfofqgnli.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gnwxyzfos.sHtML


<!-- 参考信息 -->