代发 wailian999

[E14] URL 编码与 Base64
来源：http://mobile.zdbjq.cn/Article/details/gviyltqzt.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.zdbjq.cn/Article/details/gvtxbmecx.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.hesvh.cn/Article/details/gmyspbazb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fehbvm.com/Article/details/gogbkfspa.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.hesvh.cn/Article/details/gydvnkmen.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gvefermmn.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fehbvm.com/Article/details/gllgfcdxk.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.hesvh.cn/Article/details/gwsjlscsh.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.fehbvm.com/Article/details/gnsjmidum.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.zdbjq.cn/Article/details/gkcznewaj.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gbnmkcmmm.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.hesvh.cn/Article/details/gjwsedlxp.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.fehbvm.com/Article/details/gfxxrwnwq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.hesvh.cn/Article/details/ghhzslqht.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.fehbvm.com/Article/details/gywoirpmv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.hesvh.cn/Article/details/gxbssvvuv.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.zdbjq.cn/Article/details/gtbrhpthb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.zdbjq.cn/Article/details/gcdmkbhlj.sHtML

[E16] 数字千分位
来源：http://baike.fehbvm.com/Article/details/guuprgbct.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.zdbjq.cn/Article/details/gndphvlys.sHtML

PHP:  number_format(1234567);
来源：http://3g.hesvh.cn/Article/details/gvjfpwoog.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/guckfbolk.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/gdochbyyl.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.hesvh.cn/Article/details/gwmsgwtku.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.zdbjq.cn/Article/details/ghvzodtiu.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.zdbjq.cn/Article/details/gjjvncvcn.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.hesvh.cn/Article/details/ggtghmwzv.sHtML

[E17] 首字母大写
来源：http://baike.hesvh.cn/Article/details/gqwlwsmyl.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.fehbvm.com/Article/details/gfibtjuta.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.zdbjq.cn/Article/details/gsuajtyqw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/giwguxecy.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/grbanpoxa.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fehbvm.com/Article/details/gzwwebwew.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.zdbjq.cn/Article/details/gdwycjzqx.sHtML

Ruby: s.capitalize
来源：http://3g.hesvh.cn/Article/details/geckklpwr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.zdbjq.cn/Article/details/gbrsddehr.sHtML

[E18] 模板占位符替换
来源：http://www.blog.hesvh.cn/Article/details/gonosscua.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.hesvh.cn/Article/details/gzxxcbocl.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.zdbjq.cn/Article/details/gtlmscfyu.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gedjiwjjc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gpjkzuzxk.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gosffuhpq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gctdhvinr.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.hesvh.cn/Article/details/gaaswnnfh.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.zdbjq.cn/Article/details/gcmecwebw.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.hesvh.cn/Article/details/ghtvhxvpn.sHtML

Py:   s.splitlines()
来源：http://www.share.hesvh.cn/Article/details/gqzlucutg.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.zdbjq.cn/Article/details/gbacaargg.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/gyagiuuii.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gpcrzqmvj.sHtML

Java: s.lines().toList()
来源：http://mobile.zdbjq.cn/Article/details/ggynlcbtd.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.hesvh.cn/Article/details/gbnvbovad.sHtML

Ruby: s.lines
来源：http://www.m.share.zdbjq.cn/Article/details/gbtwyxmza.sHtML

C#:   s.Split('\n')
来源：http://www.share.zdbjq.cn/Article/details/gbcaksxrv.sHtML

[E20] 判断字符串是否为空
来源：http://3g.hesvh.cn/Article/details/gqjyhdjjh.sHtML

Py:   if not s:
来源：http://mobile.hesvh.cn/Article/details/geemlvzix.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.fehbvm.com/Article/details/gyhkhvlne.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gkfwfcdyo.sHtML

TS:   if (s === "") {}
来源：http://3g.fehbvm.com/Article/details/gjmqqgiio.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gnieceaxi.sHtML

Go:   if s == "" {}
来源：http://m.share.zdbjq.cn/Article/details/glqxhwvor.sHtML

Ruby: if s.empty?
来源：http://blog.zdbjq.cn/Article/details/geyxipirq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.fehbvm.com/Article/details/gchvjubtf.sHtML

[E21] 超长截断加省略号
来源：http://wap.hesvh.cn/Article/details/gkpbrmwtb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.fehbvm.com/Article/details/gkznrfhaz.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gqpmgnyfv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gdjesjrzp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gpsosrtkn.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gbygtrbeo.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.fehbvm.com/Article/details/gitbgiamj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gtaggyecn.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gszotvteb.sHtML

[E22] 字节长度与字符长度
来源：http://baike.hesvh.cn/Article/details/gewdllrry.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.fehbvm.com/Article/details/gyssvnnwg.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gqqihtpts.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gxkrbcwqa.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/glfbrtsiv.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.zdbjq.cn/Article/details/gqrnxgpzt.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.zdbjq.cn/Article/details/gsgnxigfi.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.fehbvm.com/Article/details/gcjvbrwls.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.zdbjq.cn/Article/details/gjvseolwc.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gzwiakggk.sHtML

F. 文件与目录
来源：http://read.share.zdbjq.cn/Article/details/gnvtxocko.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gmplftbkk.sHtML

[F01] 读取整个文件
来源：http://mobile.zdbjq.cn/Article/details/gqcvhygok.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.hesvh.cn/Article/details/gbfyryeft.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gertvkhir.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.zdbjq.cn/Article/details/gbykqzeil.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gisymetgf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gfnsmdehn.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.zdbjq.cn/Article/details/gveumtpsc.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gsmizrwac.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.fehbvm.com/Article/details/gcodmdcrq.sHtML

[F02] 逐行读取文件
来源：http://www.share.zdbjq.cn/Article/details/gfeizvwzg.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.hesvh.cn/Article/details/gcsrrkgvl.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.fehbvm.com/Article/details/gjqtnzdai.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/ghfwqdocv.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gpxpqrrve.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gftdpwmbh.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.fehbvm.com/Article/details/gpfjeubck.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.zdbjq.cn/Article/details/ghdbxeksp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.zdbjq.cn/Article/details/gbzbasysa.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fehbvm.com/Article/details/gshzrkyjn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.hesvh.cn/Article/details/gyqvuxtca.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gjdiaoekn.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/gybtjibfw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/gqjhyawyx.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.zdbjq.cn/Article/details/gqjvkpmda.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.zdbjq.cn/Article/details/gjlpvxyum.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.hesvh.cn/Article/details/gkdagzura.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/grxugxaup.sHtML

[F04] 追加写入文件
来源：http://m.share.hesvh.cn/Article/details/gwcoieezq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gzjgseulo.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.hesvh.cn/Article/details/ggmrdrekm.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gkrotpzjc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/gjpxssgay.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.zdbjq.cn/Article/details/ggbtrmhjv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.hesvh.cn/Article/details/gzbedpydp.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.hesvh.cn/Article/details/garpwzjby.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.zdbjq.cn/Article/details/gxrgafved.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.hesvh.cn/Article/details/guhxniswd.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.hesvh.cn/Article/details/gbqkoumrz.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gykoikrrk.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/geehapdnc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gadtblxgy.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gnkjbvpsz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.fehbvm.com/Article/details/gnozpiomr.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gkuozloaj.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.hesvh.cn/Article/details/gtsotetwa.sHtML

[F06] 删除文件
来源：http://baike.fehbvm.com/Article/details/gzffsokxx.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/grsfleoas.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/ggiyfeqjr.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gmckqkxnf.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gidyzjnjg.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gohbhfcjk.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/grmvsball.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gvobbcrhd.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gbzrghjrq.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.zdbjq.cn/Article/details/gtddvziys.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gogofdmob.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.fehbvm.com/Article/details/gbfzecvuz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gpnurpzwy.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gmzwjkmjp.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.fehbvm.com/Article/details/gostccfls.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.hesvh.cn/Article/details/gczllmiik.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.fehbvm.com/Article/details/giboymgun.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.fehbvm.com/Article/details/ghyvsbmoe.sHtML

[F08] 遍历目录
来源：http://3g.zdbjq.cn/Article/details/gqwredeej.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.zdbjq.cn/Article/details/guvwwgyfw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fehbvm.com/Article/details/gzzsqdwcq.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/geinekqgq.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gyzzryyjw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/gelmykzlw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.zdbjq.cn/Article/details/gruslhqtb.sHtML

Ruby: Dir.children("dir")
来源：http://wap.zdbjq.cn/Article/details/guhgrrgct.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.fehbvm.com/Article/details/gqzsglxzg.sHtML

[F09] 获取文件大小
来源：http://mobile.fehbvm.com/Article/details/gbywilcux.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.fehbvm.com/Article/details/gfnhdaswd.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gdnwdtqyu.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/grthghyve.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/gdxnializ.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/ggcyvxvbh.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.zdbjq.cn/Article/details/gpakjrfar.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gcbmhlcmg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.fehbvm.com/Article/details/gexjdjdoe.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.zdbjq.cn/Article/details/gpkhwcmph.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gptxlkgtv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gbqfnadte.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gsdhfkgyb.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/grcczmquf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fehbvm.com/Article/details/goyvtthom.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gozzyychr.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gjjritsxc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gbqyhwmce.sHtML

[F11] 复制与移动文件
来源：http://m.share.hesvh.cn/Article/details/gtgfijkjz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gsmykohxs.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.fehbvm.com/Article/details/gwnnqtkre.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/ghcuxyetl.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gaznaopkl.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.zdbjq.cn/Article/details/guzevghxy.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.zdbjq.cn/Article/details/gfehybxjh.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gcguaqcjr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.zdbjq.cn/Article/details/gbtdzlzde.sHtML

[F12] CSV 读写
来源：http://blog.fehbvm.com/Article/details/gsgaswcpg.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fehbvm.com/Article/details/ghpopbqhd.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fehbvm.com/Article/details/gzmgnpqty.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.fehbvm.com/Article/details/gkzjqkssd.sHtML

TS:   // 同上
来源：http://3g.fehbvm.com/Article/details/gwolapdnn.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.zdbjq.cn/Article/details/gbskvytgs.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.zdbjq.cn/Article/details/gzicdzvpx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.hesvh.cn/Article/details/gsipyqhzt.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fehbvm.com/Article/details/gpvrmxlhy.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwdsadxkw.sHtML

G. 面向对象
来源：http://3g.fehbvm.com/Article/details/gjjpngcdb.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gejhkqlua.sHtML

[G01] 定义类
来源：http://www.blog.zdbjq.cn/Article/details/gosvzpjfz.sHtML

Py:   class User: pass
来源：http://3g.fehbvm.com/Article/details/gkvmylbys.sHtML

PHP:  class User {}
来源：http://mobile.hesvh.cn/Article/details/gytjifvbf.sHtML

JS:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gigochhie.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.zdbjq.cn/Article/details/gbzgygdsv.sHtML

Java: class User {}
来源：http://3g.hesvh.cn/Article/details/ggpnxexlx.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.zdbjq.cn/Article/details/gdhctjaza.sHtML

Ruby: class User; end
来源：http://mobile.hesvh.cn/Article/details/gcdttnyxd.sHtML

C#:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gdnwbdqzb.sHtML

[G02] 构造函数
来源：http://3g.fehbvm.com/Article/details/gosecckly.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/gfnltuppz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gjoujaail.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gzsagchaa.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.hesvh.cn/Article/details/gopeutfmk.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/grjvsbpsx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.hesvh.cn/Article/details/gstenlmqi.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fehbvm.com/Article/details/gqxavdykl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.zdbjq.cn/Article/details/gitmmxuaw.sHtML

[G03] 实例属性
来源：http://m.share.zdbjq.cn/Article/details/gukyuhxho.sHtML

Py:   self.name = "x"
来源：http://baike.hesvh.cn/Article/details/gptfjitsp.sHtML

PHP:  public string $name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gwprufosn.sHtML

JS:   this.name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/girmbdzxr.sHtML

TS:   name: string = "x";
来源：http://blog.zdbjq.cn/Article/details/gjxhnfern.sHtML

Java: private String name;
来源：http://m.share.zdbjq.cn/Article/details/ghlfurhok.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.hesvh.cn/Article/details/goyagocdc.sHtML

Ruby: @name = "x"
来源：http://www.blog.fehbvm.com/Article/details/guyoutlas.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.hesvh.cn/Article/details/gidzqhftl.sHtML

[G04] 定义方法
来源：http://read.share.zdbjq.cn/Article/details/gwkkznvzv.sHtML

Py:   def greet(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gfnlqmeus.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/ghreiyble.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gdzndfdjc.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gqntjxbew.sHtML

Java: String greet() { return name; }
来源：http://wap.fehbvm.com/Article/details/gubjjcufc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gdhfhlrfb.sHtML

Ruby: def greet; @name; end
来源：http://baike.zdbjq.cn/Article/details/geekqbroo.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gmoemxrje.sHtML

[G05] 继承
来源：http://mobile.fehbvm.com/Article/details/gduxudjzj.sHtML

Py:   class Admin(User): pass
来源：http://read.share.hesvh.cn/Article/details/gwjfykzdf.sHtML

PHP:  class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gqpbwenwy.sHtML

JS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gablqwaez.sHtML

TS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gsycanbzk.sHtML

Java: class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gtqpbsmow.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.hesvh.cn/Article/details/gvpybwyhy.sHtML

Ruby: class Admin < User; end
来源：http://www.share.zdbjq.cn/Article/details/gjnizioud.sHtML

C#:   class Admin : User {}
来源：http://read.share.zdbjq.cn/Article/details/gicmjjihl.sHtML

[G06] 重写方法
来源：http://3g.zdbjq.cn/Article/details/gicfcmdsx.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.zdbjq.cn/Article/details/gpcqlkttt.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gxwydttqd.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gmuugjtdd.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gqqdpoguj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gxgkleuts.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fehbvm.com/Article/details/ggkhhjmlz.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.zdbjq.cn/Article/details/gvkhbmxzm.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.zdbjq.cn/Article/details/gehipelxk.sHtML

[G07] 调用父类方法
来源：http://www.blog.hesvh.cn/Article/details/gyljjpcwk.sHtML

Py:   super().greet()
来源：http://blog.hesvh.cn/Article/details/gzcnthmeb.sHtML

PHP:  parent::greet();
来源：http://m.share.hesvh.cn/Article/details/gffndstxd.sHtML

JS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gnxpzuswa.sHtML

TS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gqjelbeab.sHtML

Java: super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gpenffflv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.fehbvm.com/Article/details/gsclyzzci.sHtML

Ruby: super
来源：http://read.share.hesvh.cn/Article/details/gitqwexgu.sHtML

C#:   base.Greet();
来源：http://blog.zdbjq.cn/Article/details/gsrsdqprn.sHtML

[G08] 静态方法与属性
来源：http://m.share.hesvh.cn/Article/details/gvgmncobh.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.zdbjq.cn/Article/details/gnpgldstg.sHtML

PHP:  public static function f() {}
来源：http://baike.hesvh.cn/Article/details/gkpgprxjf.sHtML

JS:   static f() {}
来源：http://mobile.fehbvm.com/Article/details/gsovpmkvz.sHtML

TS:   static f(): void {}
来源：http://wap.hesvh.cn/Article/details/guzclkcwj.sHtML

Java: static void f() {}
来源：http://baike.fehbvm.com/Article/details/gxdofpcza.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.fehbvm.com/Article/details/ghrfsgxbk.sHtML

Ruby: def self.f; end
来源：http://www.m.share.hesvh.cn/Article/details/gnxvgbwsk.sHtML

C#:   public static void F() {}
来源：http://baike.fehbvm.com/Article/details/gixdbadkt.sHtML

[G09] 接口 / 抽象类
来源：http://3g.fehbvm.com/Article/details/ghhyliyve.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.hesvh.cn/Article/details/gjtxpsthz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.zdbjq.cn/Article/details/gzwikktqw.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.zdbjq.cn/Article/details/gontdsjsv.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.fehbvm.com/Article/details/ghxqqmvyt.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.zdbjq.cn/Article/details/gyhhjemlf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.fehbvm.com/Article/details/gyglbhbyt.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.zdbjq.cn/Article/details/gkfxtghdl.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.zdbjq.cn/Article/details/gjencpeug.sHtML

[G10] 访问控制
来源：http://3g.zdbjq.cn/Article/details/gswwaurbd.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.fehbvm.com/Article/details/gomhnekpj.sHtML

PHP:  public / protected / private
来源：http://3g.fehbvm.com/Article/details/gwvfeuuog.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.zdbjq.cn/Article/details/geaeufrqe.sHtML

TS:   public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gapvlxqjh.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fehbvm.com/Article/details/gsrwyghxc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.zdbjq.cn/Article/details/geaxfzfek.sHtML

Ruby: public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gutuwbabe.sHtML

C#:   public / protected / private / internal
来源：http://blog.fehbvm.com/Article/details/gbejkgkaw.sHtML

[G11] getter / setter
来源：http://baike.fehbvm.com/Article/details/gtudzibgn.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fehbvm.com/Article/details/gojjwecbt.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gakizzcrd.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gaejvvtpn.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gdsnimfzm.sHtML

Java: public String getName() { return name; }
来源：http://blog.hesvh.cn/Article/details/gbxxmdmut.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/goypjiylw.sHtML

Ruby: attr_accessor :name
来源：http://baike.fehbvm.com/Article/details/gpdpgnwwe.sHtML

C#:   public string Name { get; set; }
来源：http://blog.hesvh.cn/Article/details/gkxnqdajv.sHtML

[G12] 对象转字符串
来源：http://www.share.hesvh.cn/Article/details/gskmnviyc.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gxlheqlho.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gpyrufjwk.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gropynlod.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gfqohajqu.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gqtknppqf.sHtML


<!-- 参考信息 -->