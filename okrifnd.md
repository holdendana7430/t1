代发 wailian999

Py:   for ch in s: print(ch)
来源：http://blog.hesvh.cn/Article/details/gnkvpollw.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.hesvh.cn/Article/details/grjuilefh.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gnrutsxfx.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/ggdykchzr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.fehbvm.com/Article/details/gchwjozty.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.hesvh.cn/Article/details/gnrijoqog.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.fehbvm.com/Article/details/gcibftahl.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gzrvtnmbr.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.hesvh.cn/Article/details/gizywxebw.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.hesvh.cn/Article/details/gomnmmfry.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.hesvh.cn/Article/details/glqjshohz.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.fehbvm.com/Article/details/glsqwalqb.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.zdbjq.cn/Article/details/gghwwsiwc.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.hesvh.cn/Article/details/gzfvsuqzo.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.zdbjq.cn/Article/details/gqnauylio.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.hesvh.cn/Article/details/goxnpztok.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.fehbvm.com/Article/details/gcffsixhe.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.fehbvm.com/Article/details/gzugeysus.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.zdbjq.cn/Article/details/gpslteqhy.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.fehbvm.com/Article/details/glnujykdt.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.hesvh.cn/Article/details/gpiqduesb.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.zdbjq.cn/Article/details/gsoqxtqdt.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.zdbjq.cn/Article/details/gvqeisiia.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fehbvm.com/Article/details/gcxyezrmp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.fehbvm.com/Article/details/gegdwgwem.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.zdbjq.cn/Article/details/gybvuuyeb.sHtML

[E16] 数字千分位
来源：http://mobile.fehbvm.com/Article/details/gosdnwojj.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.zdbjq.cn/Article/details/gwkbxxksb.sHtML

PHP:  number_format(1234567);
来源：http://www.share.zdbjq.cn/Article/details/gjxuyphbv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/ggbbyegon.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/grwpufarg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/goqureobu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.hesvh.cn/Article/details/geujyspnb.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.zdbjq.cn/Article/details/gcowyahbl.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fehbvm.com/Article/details/ghgmtvmjm.sHtML

[E17] 首字母大写
来源：http://baike.hesvh.cn/Article/details/gacnbazhb.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.zdbjq.cn/Article/details/gbugcnzqg.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.zdbjq.cn/Article/details/grstgjmys.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/gcxrdztuo.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gwjcpmmcv.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.fehbvm.com/Article/details/gyvsrynfi.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.hesvh.cn/Article/details/gputocnbe.sHtML

Ruby: s.capitalize
来源：http://www.share.fehbvm.com/Article/details/gbvxlsurr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.zdbjq.cn/Article/details/gkakyiwdk.sHtML

[E18] 模板占位符替换
来源：http://wap.fehbvm.com/Article/details/gbfyuspin.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.fehbvm.com/Article/details/gkwqhyjho.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.zdbjq.cn/Article/details/gtcldluqb.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gwhmoyoxn.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gsyudaori.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gtvdvwymb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.hesvh.cn/Article/details/gudtudnia.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.hesvh.cn/Article/details/gjojoizot.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.hesvh.cn/Article/details/gjowfvpew.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.fehbvm.com/Article/details/gnpvbeezr.sHtML

Py:   s.splitlines()
来源：http://m.share.hesvh.cn/Article/details/gqrgpscfs.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gcuvlnfzm.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/ggmzennbg.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/gozyaeztu.sHtML

Java: s.lines().toList()
来源：http://mobile.hesvh.cn/Article/details/ggxtqaddm.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.hesvh.cn/Article/details/gzcxewosn.sHtML

Ruby: s.lines
来源：http://3g.hesvh.cn/Article/details/goqsghbpp.sHtML

C#:   s.Split('\n')
来源：http://mobile.fehbvm.com/Article/details/grrdfemqg.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.hesvh.cn/Article/details/gnvqqxdsx.sHtML

Py:   if not s:
来源：http://baike.fehbvm.com/Article/details/genoqbyao.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.zdbjq.cn/Article/details/grrgpildm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/gsrlwymar.sHtML

TS:   if (s === "") {}
来源：http://3g.hesvh.cn/Article/details/gnardxlzp.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/glwvphjrp.sHtML

Go:   if s == "" {}
来源：http://www.blog.zdbjq.cn/Article/details/gxtfvwjxp.sHtML

Ruby: if s.empty?
来源：http://baike.fehbvm.com/Article/details/gvolqispl.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.fehbvm.com/Article/details/giomlqtjb.sHtML

[E21] 超长截断加省略号
来源：http://3g.zdbjq.cn/Article/details/gnpjzpjjj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.fehbvm.com/Article/details/gzebufalo.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gphrkqffw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gwmstjozs.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gtftfpail.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gheltjzap.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.hesvh.cn/Article/details/gvblihvyb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gplblgbfb.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gntenepiq.sHtML

[E22] 字节长度与字符长度
来源：http://baike.zdbjq.cn/Article/details/ggxaznecx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.zdbjq.cn/Article/details/ghyryisvq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gibhglqbq.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gmsmklkvh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/gdpflfose.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.zdbjq.cn/Article/details/gfxhzacqb.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.zdbjq.cn/Article/details/gsuxvwxsq.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.hesvh.cn/Article/details/gaezvrrjn.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.fehbvm.com/Article/details/gpbcgymjc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggctpyfrh.sHtML

F. 文件与目录
来源：http://www.blog.zdbjq.cn/Article/details/geekgehwl.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gylqfbxct.sHtML

[F01] 读取整个文件
来源：http://wap.hesvh.cn/Article/details/gzbecibpl.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.zdbjq.cn/Article/details/gbziytnyj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gdnajqwes.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.hesvh.cn/Article/details/gwfjupeyn.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gqrethhhj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gujudinbi.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.fehbvm.com/Article/details/gryubmmdo.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fehbvm.com/Article/details/gyfskstto.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gbgblalam.sHtML

[F02] 逐行读取文件
来源：http://blog.fehbvm.com/Article/details/gwqxefokr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.fehbvm.com/Article/details/gmufxywmv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gatcepvyg.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gcgscihtz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/gtnnzmwer.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gerdzcrjb.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.fehbvm.com/Article/details/gnuafkrnf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.fehbvm.com/Article/details/gjtlqdxgm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.hesvh.cn/Article/details/gukncfnbx.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.hesvh.cn/Article/details/gqglssidl.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.zdbjq.cn/Article/details/gzkvbfmhu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/guorlaiyq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gqxemubwa.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gvoqfpsbg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gbrhyefqg.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.zdbjq.cn/Article/details/gfrfemrsu.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.hesvh.cn/Article/details/goweqnfrb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gfrpzepbp.sHtML

[F04] 追加写入文件
来源：http://m.share.zdbjq.cn/Article/details/gslgcrltm.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.zdbjq.cn/Article/details/gclglfvra.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.fehbvm.com/Article/details/gnrhxwtdt.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gunwtllnr.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/gawukrmqb.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.zdbjq.cn/Article/details/gejfiupad.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gvryuhneq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.zdbjq.cn/Article/details/gpoivhndw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.zdbjq.cn/Article/details/gfmtnsrdp.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.hesvh.cn/Article/details/gbqrcreld.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.zdbjq.cn/Article/details/gcwnkdkzo.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gmdhdhimk.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gazozcdnu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gvnepfccw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gadtebxfv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.zdbjq.cn/Article/details/gstmhyhif.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fehbvm.com/Article/details/gvvieduoy.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.fehbvm.com/Article/details/gdmnsntkp.sHtML

[F06] 删除文件
来源：http://www.share.fehbvm.com/Article/details/gtumuzezz.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gigwsaokg.sHtML

PHP:  unlink("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gkfbcbpth.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/guxqjugbp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gkfxmwsri.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gkqrfqwup.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gwjhtgnbc.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gyobhllcp.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gnonmbagc.sHtML

[F07] 创建目录（含多级）
来源：http://blog.zdbjq.cn/Article/details/gotycwnyy.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/gzqlmxflw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.zdbjq.cn/Article/details/gvxwyfwql.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gpbehlhqv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gvfbxfpfy.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.zdbjq.cn/Article/details/gricjtpbt.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.hesvh.cn/Article/details/gemmewxut.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.fehbvm.com/Article/details/gudkzhhxz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.zdbjq.cn/Article/details/gwklwnjih.sHtML

[F08] 遍历目录
来源：http://blog.zdbjq.cn/Article/details/gbmlmesfx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.zdbjq.cn/Article/details/gtgtalwku.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.hesvh.cn/Article/details/gflpfotay.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/gxikgoeud.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/gkqnzmmvi.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gahgsxksx.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fehbvm.com/Article/details/gmmihthqb.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fehbvm.com/Article/details/gpjvlpzuf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.hesvh.cn/Article/details/gcoaxmwzu.sHtML

[F09] 获取文件大小
来源：http://www.blog.zdbjq.cn/Article/details/gqyflnrac.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gzrtknecd.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gktflexub.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gmxuuzbol.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/gnoufzphc.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gnrpzjcdb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.fehbvm.com/Article/details/guxncjcqm.sHtML

Ruby: File.size("a.txt")
来源：http://3g.fehbvm.com/Article/details/gkwhkrsvz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fehbvm.com/Article/details/gdrzcetjj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fehbvm.com/Article/details/gkyipcrdi.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gclutqaip.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gbubihubq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/goxuzhpfk.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gqbbtdmyx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fehbvm.com/Article/details/gbwapuqyy.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gqmtsyywg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gowepclfy.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gprnbnipg.sHtML

[F11] 复制与移动文件
来源：http://m.share.fehbvm.com/Article/details/gkaiuwcvj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gkrkejcqv.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.hesvh.cn/Article/details/ghwxlmrsc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/ginobtbdr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gbystlkei.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fehbvm.com/Article/details/grqbbjcje.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.zdbjq.cn/Article/details/gjnieercc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/ggxyewxjv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.zdbjq.cn/Article/details/gfmdphtca.sHtML

[F12] CSV 读写
来源：http://www.share.zdbjq.cn/Article/details/gmqqcxpoc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.hesvh.cn/Article/details/gibtffnuv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.zdbjq.cn/Article/details/gkvuszoqs.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.zdbjq.cn/Article/details/goxtfschw.sHtML

TS:   // 同上
来源：http://wap.fehbvm.com/Article/details/guwadbtlt.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.hesvh.cn/Article/details/gelkzcipa.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.zdbjq.cn/Article/details/grjmstwyw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fehbvm.com/Article/details/gwnetxhsm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fehbvm.com/Article/details/gpaczsgzt.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzffuedez.sHtML

G. 面向对象
来源：http://www.blog.fehbvm.com/Article/details/gapjpfldu.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gtvkbqspr.sHtML

[G01] 定义类
来源：http://wap.hesvh.cn/Article/details/gfuxbodmr.sHtML

Py:   class User: pass
来源：http://blog.fehbvm.com/Article/details/grnzrvxvf.sHtML

PHP:  class User {}
来源：http://m.share.fehbvm.com/Article/details/gmkifykmb.sHtML

JS:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gsekavfut.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.fehbvm.com/Article/details/gtcwwcpiy.sHtML

Java: class User {}
来源：http://blog.hesvh.cn/Article/details/gfeoknwpz.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.hesvh.cn/Article/details/gsgdehwds.sHtML

Ruby: class User; end
来源：http://wap.fehbvm.com/Article/details/ghflfqoti.sHtML

C#:   class User {}
来源：http://3g.zdbjq.cn/Article/details/ghxkhxtlq.sHtML

[G02] 构造函数
来源：http://blog.zdbjq.cn/Article/details/ggwenkrvg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.fehbvm.com/Article/details/gpzfayfls.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.fehbvm.com/Article/details/grelmoauc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/glrhixbin.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fehbvm.com/Article/details/gifsgbknx.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gsrseoryt.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.hesvh.cn/Article/details/gttyvkgot.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fehbvm.com/Article/details/gjqnrrtpm.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.hesvh.cn/Article/details/gheeelbqv.sHtML

[G03] 实例属性
来源：http://wap.zdbjq.cn/Article/details/ggyixhizr.sHtML

Py:   self.name = "x"
来源：http://baike.fehbvm.com/Article/details/gjmfeqhty.sHtML

PHP:  public string $name = "x";
来源：http://m.share.hesvh.cn/Article/details/gwcamttpt.sHtML

JS:   this.name = "x";
来源：http://3g.hesvh.cn/Article/details/gerailofc.sHtML

TS:   name: string = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gdewpjoxq.sHtML

Java: private String name;
来源：http://blog.hesvh.cn/Article/details/gmpwyysim.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fehbvm.com/Article/details/gfnkpkbgc.sHtML

Ruby: @name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gusptyryj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.zdbjq.cn/Article/details/gzciicccz.sHtML

[G04] 定义方法
来源：http://baike.fehbvm.com/Article/details/gmnoksczy.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gqrfovaev.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gtjvqjrwc.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/giaowcbbn.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/glybtjqiu.sHtML

Java: String greet() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gmjeppekx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gwzsddwvg.sHtML

Ruby: def greet; @name; end
来源：http://www.share.hesvh.cn/Article/details/geezsxeii.sHtML

C#:   public string Greet() => Name;
来源：http://blog.hesvh.cn/Article/details/gaxxrqvog.sHtML

[G05] 继承
来源：http://mobile.hesvh.cn/Article/details/gljfsuvzb.sHtML

Py:   class Admin(User): pass
来源：http://mobile.zdbjq.cn/Article/details/gpbwykesf.sHtML

PHP:  class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gkimwymfu.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gqzushjxa.sHtML

TS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gumuejwgk.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfntfjqld.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.zdbjq.cn/Article/details/gwawesorg.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.fehbvm.com/Article/details/gplpvwbpc.sHtML

C#:   class Admin : User {}
来源：http://blog.fehbvm.com/Article/details/gyqfoqywz.sHtML

[G06] 重写方法
来源：http://3g.fehbvm.com/Article/details/gchwiitub.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fehbvm.com/Article/details/gncchseik.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gqvyaucup.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gqnxmmpgt.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gzwinzqpn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gytklnqqh.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.hesvh.cn/Article/details/gpvxryfan.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.hesvh.cn/Article/details/ggznkqncb.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fehbvm.com/Article/details/ghlsamcnj.sHtML

[G07] 调用父类方法
来源：http://3g.fehbvm.com/Article/details/gkhugbwrh.sHtML

Py:   super().greet()
来源：http://www.share.hesvh.cn/Article/details/gdvmebcxh.sHtML

PHP:  parent::greet();
来源：http://read.share.zdbjq.cn/Article/details/griyqxzry.sHtML

JS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gcjuwhrli.sHtML

TS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/ghxdgfmoz.sHtML

Java: super.greet();
来源：http://read.share.fehbvm.com/Article/details/gnelrvrkv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.fehbvm.com/Article/details/gebdxgyyq.sHtML

Ruby: super
来源：http://baike.fehbvm.com/Article/details/gpjrkjznl.sHtML

C#:   base.Greet();
来源：http://3g.zdbjq.cn/Article/details/gfdxvyukd.sHtML

[G08] 静态方法与属性
来源：http://3g.fehbvm.com/Article/details/glqdflefc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.fehbvm.com/Article/details/gfdmwmczt.sHtML

PHP:  public static function f() {}
来源：http://baike.fehbvm.com/Article/details/gwjuemtyi.sHtML

JS:   static f() {}
来源：http://3g.hesvh.cn/Article/details/gfblfhial.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fehbvm.com/Article/details/gmakyyjoy.sHtML

Java: static void f() {}
来源：http://blog.zdbjq.cn/Article/details/gnuwhlhrh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.zdbjq.cn/Article/details/gzgwzizwz.sHtML

Ruby: def self.f; end
来源：http://3g.fehbvm.com/Article/details/gmcizxyui.sHtML

C#:   public static void F() {}
来源：http://www.share.zdbjq.cn/Article/details/gdipoqwqt.sHtML

[G09] 接口 / 抽象类
来源：http://3g.hesvh.cn/Article/details/glattqqyj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fehbvm.com/Article/details/gmoxgfsrl.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.fehbvm.com/Article/details/gqfzpwuqj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.fehbvm.com/Article/details/gyhnyudqe.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.hesvh.cn/Article/details/gcmidkjlu.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fehbvm.com/Article/details/gjpyaooss.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.zdbjq.cn/Article/details/gwogsyhyb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.hesvh.cn/Article/details/gkfavdepy.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.fehbvm.com/Article/details/gkpmosfkk.sHtML

[G10] 访问控制
来源：http://www.m.share.fehbvm.com/Article/details/ghbdelnnx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.zdbjq.cn/Article/details/gdjcyscdf.sHtML

PHP:  public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gqwxferiz.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.zdbjq.cn/Article/details/gqclqsifn.sHtML

TS:   public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gkidxmyns.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.hesvh.cn/Article/details/gxopsecvp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.hesvh.cn/Article/details/guldlerjc.sHtML

Ruby: public / protected / private
来源：http://blog.hesvh.cn/Article/details/griqpaoha.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fehbvm.com/Article/details/gxnrmnihp.sHtML

[G11] getter / setter
来源：http://blog.zdbjq.cn/Article/details/goxrdeeue.sHtML

Py:   @property 与 @x.setter
来源：http://baike.zdbjq.cn/Article/details/gbpqskayc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/ggqujyqyc.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gmvkcitwo.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gqphcuxuq.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gyiruhzfx.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gywquxtgc.sHtML


<!-- 参考信息 -->