代发 wailian999

PHP:  substr_count($s, "a");
来源：http://m.share.zdbjq.cn/Article/details/gffrgtgyl.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/gobmfaeac.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gnwfabbwz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.zdbjq.cn/Article/details/gtzepauvg.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.hesvh.cn/Article/details/gopmkapfj.sHtML

Ruby: s.count("a")
来源：http://read.share.hesvh.cn/Article/details/gzguffuot.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.zdbjq.cn/Article/details/gwzovazzo.sHtML

[E13] 逐字符遍历
来源：http://www.blog.hesvh.cn/Article/details/ggvnejocb.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.hesvh.cn/Article/details/gebpgmggg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.fehbvm.com/Article/details/gwpkyiwku.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gftyjhqyf.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gbcqmpgku.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gpyydisal.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.hesvh.cn/Article/details/gqpzjwxhm.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.zdbjq.cn/Article/details/gjuddwqll.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.hesvh.cn/Article/details/gkwdhenex.sHtML

[E14] URL 编码与 Base64
来源：http://blog.fehbvm.com/Article/details/ggtclfoyh.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.hesvh.cn/Article/details/gpgzzucfx.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.hesvh.cn/Article/details/ghkjpluaj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.fehbvm.com/Article/details/gpkllknja.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.zdbjq.cn/Article/details/gyzkcjusi.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.fehbvm.com/Article/details/gbtudaksm.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.zdbjq.cn/Article/details/gaxeydezr.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.hesvh.cn/Article/details/gmfckskvg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gijbanrfe.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.hesvh.cn/Article/details/gfkccbvhf.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.fehbvm.com/Article/details/gawvukyqq.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.fehbvm.com/Article/details/gpqlkvynq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.hesvh.cn/Article/details/gutvbinyj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.zdbjq.cn/Article/details/gpzoloufj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.fehbvm.com/Article/details/gqlrsqkln.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.fehbvm.com/Article/details/gjcftrytb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fehbvm.com/Article/details/gdokyojqp.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.hesvh.cn/Article/details/gdmsfawft.sHtML

[E16] 数字千分位
来源：http://www.blog.fehbvm.com/Article/details/gylvbtagz.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.fehbvm.com/Article/details/gcmtgpdti.sHtML

PHP:  number_format(1234567);
来源：http://wap.hesvh.cn/Article/details/grzbpopyf.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gwriamqbd.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/gpawcldow.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.zdbjq.cn/Article/details/grivlponi.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.hesvh.cn/Article/details/grgbfjinl.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.hesvh.cn/Article/details/gajymiwvb.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.hesvh.cn/Article/details/gxwebyyjr.sHtML

[E17] 首字母大写
来源：http://blog.zdbjq.cn/Article/details/gdahkrcqa.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.hesvh.cn/Article/details/ghmjiaxwz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.hesvh.cn/Article/details/gslaojdcr.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/ghwphtvbr.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/gnxiwseae.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.hesvh.cn/Article/details/ghhrvtfsr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.fehbvm.com/Article/details/gcwzwclmu.sHtML

Ruby: s.capitalize
来源：http://read.share.hesvh.cn/Article/details/ghpvenjae.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.zdbjq.cn/Article/details/gmxpznwlr.sHtML

[E18] 模板占位符替换
来源：http://3g.fehbvm.com/Article/details/gtqmpggjn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.zdbjq.cn/Article/details/gbfnujwgf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.zdbjq.cn/Article/details/giuohwtzk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gvhpfssmy.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gfsugkpmp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gjlbrytxt.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.hesvh.cn/Article/details/gglnsyfoo.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.fehbvm.com/Article/details/gsmdieuaq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.fehbvm.com/Article/details/gxabhsejc.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.fehbvm.com/Article/details/gyqyewsly.sHtML

Py:   s.splitlines()
来源：http://blog.hesvh.cn/Article/details/gigaukdpc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gmhrdlruz.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/gwfmhvihq.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/gwqftreaw.sHtML

Java: s.lines().toList()
来源：http://read.share.hesvh.cn/Article/details/gvnflawwo.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.fehbvm.com/Article/details/gczeohxso.sHtML

Ruby: s.lines
来源：http://blog.zdbjq.cn/Article/details/gxzhorgxk.sHtML

C#:   s.Split('\n')
来源：http://read.share.zdbjq.cn/Article/details/gylnmbpqq.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.hesvh.cn/Article/details/gyjeemybn.sHtML

Py:   if not s:
来源：http://blog.hesvh.cn/Article/details/gkoekfeak.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.fehbvm.com/Article/details/ghtvstwrb.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.fehbvm.com/Article/details/gpfhlwbzs.sHtML

TS:   if (s === "") {}
来源：http://wap.fehbvm.com/Article/details/gynsnupqj.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gvnskgxlp.sHtML

Go:   if s == "" {}
来源：http://wap.fehbvm.com/Article/details/gonzzwqzi.sHtML

Ruby: if s.empty?
来源：http://www.blog.fehbvm.com/Article/details/gqftxbkfp.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.fehbvm.com/Article/details/geieqzhmo.sHtML

[E21] 超长截断加省略号
来源：http://read.share.zdbjq.cn/Article/details/gmaodywjz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.zdbjq.cn/Article/details/ghhbkzmbl.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gltohbayj.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gnlsnlwxn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gvnuyhdzc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gmszbzggq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.hesvh.cn/Article/details/goyjzhrrq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gxtastxcj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gemarzamh.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.fehbvm.com/Article/details/gezwuewjl.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.zdbjq.cn/Article/details/gozybzpin.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gmromddeh.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/gjoqqylky.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/ggwiyiuwa.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.zdbjq.cn/Article/details/ggalgsdzu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.hesvh.cn/Article/details/gqztlrcyz.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fehbvm.com/Article/details/gabranzxq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gpzqsorwj.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gdmklcutp.sHtML

F. 文件与目录
来源：http://mobile.zdbjq.cn/Article/details/gswxeopwv.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/glcvvfzwq.sHtML

[F01] 读取整个文件
来源：http://wap.hesvh.cn/Article/details/ggftzxrpp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.zdbjq.cn/Article/details/gmatozoip.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/goeskkusg.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.zdbjq.cn/Article/details/gesvtambr.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.zdbjq.cn/Article/details/ghvirorxz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gdetpxrew.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.fehbvm.com/Article/details/gemytaauh.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gozcmvgmb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.fehbvm.com/Article/details/gdveszsti.sHtML

[F02] 逐行读取文件
来源：http://read.share.hesvh.cn/Article/details/gzifufiow.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fehbvm.com/Article/details/ggknomrih.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.fehbvm.com/Article/details/grolwfgxq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/gzbmxhbdo.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/ggmjnzvcf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/gitldhlld.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.zdbjq.cn/Article/details/grfgstqgi.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.zdbjq.cn/Article/details/gwzbdsevt.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.fehbvm.com/Article/details/gmhhwdezs.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fehbvm.com/Article/details/grwcbsqvd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.hesvh.cn/Article/details/goalkqulh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gbyexmlgy.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/ghydyxcab.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/genwlkjmd.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.zdbjq.cn/Article/details/gyyykafsi.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.fehbvm.com/Article/details/gzbdhhstt.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.hesvh.cn/Article/details/gxmbsjthk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/gcsugfdas.sHtML

[F04] 追加写入文件
来源：http://3g.fehbvm.com/Article/details/giihwrayp.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.hesvh.cn/Article/details/guqhukxik.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.zdbjq.cn/Article/details/gqadjksmf.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/goxsnpvoa.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/gqnlrftsp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.zdbjq.cn/Article/details/gejlfhdoq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/goarhkmgs.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.hesvh.cn/Article/details/guvxljegb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.hesvh.cn/Article/details/gagblpmpl.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.zdbjq.cn/Article/details/goenndfqc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.zdbjq.cn/Article/details/gkucpmwwc.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gszjnhaby.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gngagxghl.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gbqpqsdia.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/ggguvkwar.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.fehbvm.com/Article/details/gqjcxcemo.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.hesvh.cn/Article/details/gqixcxxcb.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gwnhmxlek.sHtML

[F06] 删除文件
来源：http://3g.zdbjq.cn/Article/details/goiwspxmd.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/geljuuxed.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gazaumqpk.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gfhquhorm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gasfhhwzx.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gjvqexyyd.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gyxxwdjcl.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gdvwiqhpg.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gzufkpatq.sHtML

[F07] 创建目录（含多级）
来源：http://blog.hesvh.cn/Article/details/gxzuwfung.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.fehbvm.com/Article/details/gorhtzhit.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gyustnhdv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/gbtqrrgvv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/gftizmfjv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.hesvh.cn/Article/details/goawvuapv.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.zdbjq.cn/Article/details/gyacmyvwu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.fehbvm.com/Article/details/gzgcgjmct.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.hesvh.cn/Article/details/grzlopvql.sHtML

[F08] 遍历目录
来源：http://www.share.zdbjq.cn/Article/details/ghsuvvfqh.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.zdbjq.cn/Article/details/gjwogkxfh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fehbvm.com/Article/details/gnrogdtql.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gnuqzujxu.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/ggvniurds.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gobbnjxek.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gzatbeerc.sHtML

Ruby: Dir.children("dir")
来源：http://baike.hesvh.cn/Article/details/gmuvfrtzq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.hesvh.cn/Article/details/gmivmidog.sHtML

[F09] 获取文件大小
来源：http://wap.zdbjq.cn/Article/details/gackoleup.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.fehbvm.com/Article/details/gexndfcdh.sHtML

PHP:  filesize("a.txt");
来源：http://baike.fehbvm.com/Article/details/ghcziuyrf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gezjycush.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gdicokkno.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gdvjksqhw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.fehbvm.com/Article/details/gztpybebw.sHtML

Ruby: File.size("a.txt")
来源：http://baike.hesvh.cn/Article/details/gmjshvkvw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fehbvm.com/Article/details/gfvopcqck.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.zdbjq.cn/Article/details/gnbnfbayu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gdjlfqtaz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gsmimxaxp.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gjspowokc.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gabiokxhn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.fehbvm.com/Article/details/gpssyuqvd.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gfhtialou.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gzozvneyp.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/glfkwxnyp.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fehbvm.com/Article/details/gtcqyftzr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/grufwiwll.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.fehbvm.com/Article/details/gjlwlkxeq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gylpbepdq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gpcnpjaev.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.fehbvm.com/Article/details/gmdevbhai.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.hesvh.cn/Article/details/gpjoupgqv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gpuzmrlas.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.hesvh.cn/Article/details/gepcwkyux.sHtML

[F12] CSV 读写
来源：http://wap.zdbjq.cn/Article/details/ggjjtkojt.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.fehbvm.com/Article/details/gciwpzjvm.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.hesvh.cn/Article/details/gbrsycjvp.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fehbvm.com/Article/details/gnraooeoe.sHtML

TS:   // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/gvykunnbr.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.zdbjq.cn/Article/details/grxwxyuoe.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.hesvh.cn/Article/details/gihogeumw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.hesvh.cn/Article/details/gqrahvvvq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.zdbjq.cn/Article/details/gxbjkldkp.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/goorvfsfd.sHtML

G. 面向对象
来源：http://www.share.zdbjq.cn/Article/details/gbubrbzsm.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gjjwffxcr.sHtML

[G01] 定义类
来源：http://www.blog.fehbvm.com/Article/details/gavldlljc.sHtML

Py:   class User: pass
来源：http://www.blog.fehbvm.com/Article/details/garzksrhc.sHtML

PHP:  class User {}
来源：http://www.blog.fehbvm.com/Article/details/gzlmikhux.sHtML

JS:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gmqmwgwev.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.zdbjq.cn/Article/details/gtdugaovr.sHtML

Java: class User {}
来源：http://wap.fehbvm.com/Article/details/gvjvtuyag.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.fehbvm.com/Article/details/gwvjdgjww.sHtML

Ruby: class User; end
来源：http://www.blog.zdbjq.cn/Article/details/goehflaek.sHtML

C#:   class User {}
来源：http://wap.fehbvm.com/Article/details/gjsxrfypk.sHtML

[G02] 构造函数
来源：http://wap.zdbjq.cn/Article/details/gmxdmchxw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.zdbjq.cn/Article/details/grsxhemlo.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.zdbjq.cn/Article/details/gluashyzl.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gzzpsvsvq.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.hesvh.cn/Article/details/gupywxgux.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gouoajotg.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.zdbjq.cn/Article/details/gjlupeljb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fehbvm.com/Article/details/gputdguqg.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fehbvm.com/Article/details/gtgtwulxl.sHtML

[G03] 实例属性
来源：http://blog.fehbvm.com/Article/details/gsqicfzmf.sHtML

Py:   self.name = "x"
来源：http://wap.hesvh.cn/Article/details/gybdeiipx.sHtML

PHP:  public string $name = "x";
来源：http://m.share.hesvh.cn/Article/details/gazjgoxxb.sHtML

JS:   this.name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gpobqgaaa.sHtML

TS:   name: string = "x";
来源：http://mobile.zdbjq.cn/Article/details/guyxzlaix.sHtML

Java: private String name;
来源：http://www.m.share.hesvh.cn/Article/details/ghtojhgst.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.hesvh.cn/Article/details/gljizuqry.sHtML

Ruby: @name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gffpmtkva.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.zdbjq.cn/Article/details/gjvfgeehk.sHtML

[G04] 定义方法
来源：http://www.m.share.hesvh.cn/Article/details/gribhfayr.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gxatqjwnt.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gsnaoziij.sHtML

JS:   greet() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gvyxlluur.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/goozxptsh.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/goznrqgfm.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gkzhvkdnc.sHtML

Ruby: def greet; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gtwusshjn.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gzchgbyzb.sHtML

[G05] 继承
来源：http://www.blog.zdbjq.cn/Article/details/ggaophreu.sHtML

Py:   class Admin(User): pass
来源：http://www.share.hesvh.cn/Article/details/ghgyqbmsp.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gzzixlryu.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gfavojokt.sHtML

TS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gguyecojo.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghzblaadr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.zdbjq.cn/Article/details/gkyuuoxye.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/gfnpkcege.sHtML

C#:   class Admin : User {}
来源：http://3g.zdbjq.cn/Article/details/gnelowsni.sHtML

[G06] 重写方法
来源：http://m.share.hesvh.cn/Article/details/gjnzbcivz.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.zdbjq.cn/Article/details/gxrihmbri.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtentqohk.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gnfimjoaq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gutfugote.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gdvlpmjrc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fehbvm.com/Article/details/gajrrviav.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fehbvm.com/Article/details/gzuqxmzix.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.zdbjq.cn/Article/details/guacftpub.sHtML

[G07] 调用父类方法
来源：http://baike.fehbvm.com/Article/details/gzshpwndf.sHtML

Py:   super().greet()
来源：http://blog.zdbjq.cn/Article/details/gpfzbsmpm.sHtML

PHP:  parent::greet();
来源：http://mobile.zdbjq.cn/Article/details/gecszjkul.sHtML

JS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gpwnioutz.sHtML

TS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gcmycpncy.sHtML

Java: super.greet();
来源：http://wap.zdbjq.cn/Article/details/gdlknkfla.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.zdbjq.cn/Article/details/gvmcxmvcd.sHtML

Ruby: super
来源：http://www.blog.hesvh.cn/Article/details/gzyveuxsh.sHtML

C#:   base.Greet();
来源：http://3g.zdbjq.cn/Article/details/grrfkrdxn.sHtML

[G08] 静态方法与属性
来源：http://www.blog.zdbjq.cn/Article/details/gmlbxzcdd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.fehbvm.com/Article/details/gufzcmjow.sHtML

PHP:  public static function f() {}
来源：http://blog.zdbjq.cn/Article/details/gxmlvvlwi.sHtML

JS:   static f() {}
来源：http://baike.hesvh.cn/Article/details/gzghtwzml.sHtML

TS:   static f(): void {}
来源：http://baike.fehbvm.com/Article/details/gipltoajd.sHtML

Java: static void f() {}
来源：http://www.share.fehbvm.com/Article/details/ggmxhwnhf.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.zdbjq.cn/Article/details/gqvrwqeni.sHtML

Ruby: def self.f; end
来源：http://m.share.zdbjq.cn/Article/details/gufmzsofz.sHtML

C#:   public static void F() {}
来源：http://wap.fehbvm.com/Article/details/gfopeabgv.sHtML

[G09] 接口 / 抽象类
来源：http://3g.zdbjq.cn/Article/details/giqxjgopv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.zdbjq.cn/Article/details/gxzxrnmjb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.fehbvm.com/Article/details/glttqfpov.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.fehbvm.com/Article/details/ghcviqunn.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.hesvh.cn/Article/details/gnbuwquys.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.zdbjq.cn/Article/details/gsxfchemt.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.hesvh.cn/Article/details/gwfjvbouh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.hesvh.cn/Article/details/glwjkesmx.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.zdbjq.cn/Article/details/gghvbpzjy.sHtML

[G10] 访问控制
来源：http://www.m.share.hesvh.cn/Article/details/guzeeeska.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.hesvh.cn/Article/details/gzyxvvvfo.sHtML

PHP:  public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gkgukrxsh.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.zdbjq.cn/Article/details/gejmvaisv.sHtML

TS:   public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gklxbxdbu.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.hesvh.cn/Article/details/gzxoyxvtq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.zdbjq.cn/Article/details/gacgbimxi.sHtML

Ruby: public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gqmmprmff.sHtML


<!-- 参考信息 -->