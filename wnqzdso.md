代发 wailian999

PHP:  substr_count($s, "a");
来源：http://mobile.fanxiaobao.xyz/Article/details/gdixbyvyt.sHtML

JS:   s.split("a").length - 1
来源：http://wap.fanxiaobao.xyz/Article/details/giqgkchvu.sHtML

TS:   s.split("a").length - 1
来源：http://baike.fanxiaobao.xyz/Article/details/gydjtycvl.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.fanxiaobao.xyz/Article/details/gtigbfuvw.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.fanxiaobao.xyz/Article/details/guhxajvxc.sHtML

Ruby: s.count("a")
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrxtpmit.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.fanxiaobao.xyz/Article/details/gsrvlhrfy.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjreyqvq.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwczwyvu.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxkdpngfr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fanxiaobao.xyz/Article/details/gtfgdanah.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fanxiaobao.xyz/Article/details/gepqtinej.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.fanxiaobao.xyz/Article/details/gytzgqpkq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gaflvwojj.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmgduxxtq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gaumaptjz.sHtML

[E14] URL 编码与 Base64
来源：http://baike.fanxiaobao.xyz/Article/details/gmpbpfesy.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbddbjkj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.fanxiaobao.xyz/Article/details/gddeoiyqx.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fanxiaobao.xyz/Article/details/gblgsezwf.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gljmzutxu.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmmxufzr.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.fanxiaobao.xyz/Article/details/gsyqoircm.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.fanxiaobao.xyz/Article/details/gmhglkkdq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.fanxiaobao.xyz/Article/details/gxlqiyyst.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrnezroc.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxnkdinl.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyesembgv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gjipdoxuj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gumcbcnch.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvxjaovn.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gmvjcjrkq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbmojhpyw.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gccwfrrbl.sHtML

[E16] 数字千分位
来源：http://read.share.fanxiaobao.xyz/Article/details/grqphajpy.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gpnbfszjs.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fanxiaobao.xyz/Article/details/gcisdbsbm.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxonyqxlx.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.fanxiaobao.xyz/Article/details/glfatsbvq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.fanxiaobao.xyz/Article/details/ghpfybyzf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gummxybtj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumvftiie.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkxgojau.sHtML

[E17] 首字母大写
来源：http://m.share.fanxiaobao.xyz/Article/details/gdozwsxrg.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzknpfoz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.fanxiaobao.xyz/Article/details/gicbsrobw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gpajdjylq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gideifwyc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gvckclxcy.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.fanxiaobao.xyz/Article/details/grmcfeweg.sHtML

Ruby: s.capitalize
来源：http://baike.fanxiaobao.xyz/Article/details/ggwnhvrvc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fanxiaobao.xyz/Article/details/geqjwgtde.sHtML

[E18] 模板占位符替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gwonitnhk.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fanxiaobao.xyz/Article/details/gdbuuuluj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzfchpfu.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.fanxiaobao.xyz/Article/details/gcoofcuty.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwevgrzz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.fanxiaobao.xyz/Article/details/gijkhdfdz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxgpxzcq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.fanxiaobao.xyz/Article/details/gefgjelix.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.fanxiaobao.xyz/Article/details/gmzalefry.sHtML

[E19] 多行文本按行拆分
来源：http://baike.fanxiaobao.xyz/Article/details/gfaolqkwg.sHtML

Py:   s.splitlines()
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqmgliyy.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghogqxlyv.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.fanxiaobao.xyz/Article/details/gxnnpbugy.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcxmfabe.sHtML

Java: s.lines().toList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gonhuiocp.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.fanxiaobao.xyz/Article/details/gqggiorjk.sHtML

Ruby: s.lines
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giswizzzi.sHtML

C#:   s.Split('\n')
来源：http://blog.fanxiaobao.xyz/Article/details/ggxdiwdyj.sHtML

[E20] 判断字符串是否为空
来源：http://3g.fanxiaobao.xyz/Article/details/gwfrtqyix.sHtML

Py:   if not s:
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcthbizg.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.fanxiaobao.xyz/Article/details/griocwjky.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gzyfbiuwu.sHtML

TS:   if (s === "") {}
来源：http://wap.fanxiaobao.xyz/Article/details/gzuhfjtno.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gxckljwzh.sHtML

Go:   if s == "" {}
来源：http://m.share.fanxiaobao.xyz/Article/details/guyflaybt.sHtML

Ruby: if s.empty?
来源：http://read.share.fanxiaobao.xyz/Article/details/gsloqknge.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gnimykyxj.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttwwpczy.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fanxiaobao.xyz/Article/details/gsgxmkvjp.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdntbnnk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fanxiaobao.xyz/Article/details/gzvkcweup.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbhrysmq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.fanxiaobao.xyz/Article/details/ggaivvdkm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.fanxiaobao.xyz/Article/details/gwauugizl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.fanxiaobao.xyz/Article/details/grigmrrkx.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.fanxiaobao.xyz/Article/details/gifulofji.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.fanxiaobao.xyz/Article/details/glbmydmkm.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnxijbpq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fanxiaobao.xyz/Article/details/guwbhkrfb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcqkxysf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmnyfmvq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.fanxiaobao.xyz/Article/details/gwpgmzrab.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.fanxiaobao.xyz/Article/details/gjavrvzbh.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fanxiaobao.xyz/Article/details/guvawqexa.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjtboyaae.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gjoozjijn.sHtML

F. 文件与目录
来源：http://blog.fanxiaobao.xyz/Article/details/gyljcruri.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzqljnue.sHtML

[F01] 读取整个文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflbqsfiw.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.fanxiaobao.xyz/Article/details/gwmktayoi.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkiwcghpv.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijdyqtxe.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.fanxiaobao.xyz/Article/details/gnjiadkcj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.fanxiaobao.xyz/Article/details/ghajpvtcc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.fanxiaobao.xyz/Article/details/gffigobok.sHtML

Ruby: File.read("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gihdenxtk.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/gdtbtuscy.sHtML

[F02] 逐行读取文件
来源：http://3g.fanxiaobao.xyz/Article/details/gcsypkcta.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.fanxiaobao.xyz/Article/details/gxidcrthe.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.fanxiaobao.xyz/Article/details/gyotofakd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbuwxhrf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbcbegra.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.fanxiaobao.xyz/Article/details/gilyolinr.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.fanxiaobao.xyz/Article/details/gzwwxlpxa.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.fanxiaobao.xyz/Article/details/gxlhrhldw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.fanxiaobao.xyz/Article/details/gvjjyfsib.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fanxiaobao.xyz/Article/details/gkczsmbwx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.fanxiaobao.xyz/Article/details/gltbkzkxk.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gyejkvzuy.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqsntwfm.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgwihmvb.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.fanxiaobao.xyz/Article/details/gbnbpxnuc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fanxiaobao.xyz/Article/details/gthastufy.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggihwjwaz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gnuuwvvby.sHtML

[F04] 追加写入文件
来源：http://mobile.fanxiaobao.xyz/Article/details/geqbhitoc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.fanxiaobao.xyz/Article/details/gwzaiszri.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.fanxiaobao.xyz/Article/details/gevgpytbe.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxpvxrzko.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fanxiaobao.xyz/Article/details/gbcwcocqm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gunprntxl.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fanxiaobao.xyz/Article/details/gnodnjfon.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.fanxiaobao.xyz/Article/details/gsloutbkd.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.fanxiaobao.xyz/Article/details/gkpynrncd.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/ggttkgifv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqbzkqrp.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/gnffgmxnz.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gceaeqxft.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gdknschtm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.fanxiaobao.xyz/Article/details/gcyciwvke.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.fanxiaobao.xyz/Article/details/gajknehxx.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdwptimv.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpwpsruc.sHtML

[F06] 删除文件
来源：http://baike.fanxiaobao.xyz/Article/details/gzopmvxur.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxsbmarh.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvzrgkum.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gihbecngx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gwqqwmqee.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.fanxiaobao.xyz/Article/details/geexonuix.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkcbccbu.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gsiftggsx.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gheinhgrx.sHtML

[F07] 创建目录（含多级）
来源：http://baike.fanxiaobao.xyz/Article/details/gwuftngan.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gorraaxof.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.fanxiaobao.xyz/Article/details/gxioprwiu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgjrrxfk.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fanxiaobao.xyz/Article/details/gghygudve.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbzngrwmq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.fanxiaobao.xyz/Article/details/gtypkeihc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdjngnpg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fanxiaobao.xyz/Article/details/ggdrittja.sHtML

[F08] 遍历目录
来源：http://baike.fanxiaobao.xyz/Article/details/gtnhbptgm.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.fanxiaobao.xyz/Article/details/gidzkilqd.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqcdhvsma.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.fanxiaobao.xyz/Article/details/gglszmbjl.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fanxiaobao.xyz/Article/details/gdoioauci.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhqfjhob.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfpusvtf.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gklnwqkrf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fanxiaobao.xyz/Article/details/gonjrbpfd.sHtML

[F09] 获取文件大小
来源：http://www.share.fanxiaobao.xyz/Article/details/gpxlzatet.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gpikpbpbd.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhokdhgp.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fanxiaobao.xyz/Article/details/gdusmkldr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmcobtuj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fanxiaobao.xyz/Article/details/gzdqhhqra.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.fanxiaobao.xyz/Article/details/guzdiaqkz.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gpjhcpfko.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.fanxiaobao.xyz/Article/details/gtpnmnmoe.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fanxiaobao.xyz/Article/details/glugeyqgu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgjzgaaj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.fanxiaobao.xyz/Article/details/gtxrieewg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/goxosubud.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gezuxbspq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrugbhdl.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gqsfbyctm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpqqivuc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gqujofupm.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdxcrask.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/grmtqlkek.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gwdojzfyo.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtyttylc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/grhnkjpnv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.fanxiaobao.xyz/Article/details/gfiguqxup.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fanxiaobao.xyz/Article/details/gbroxisjf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gxpltifzp.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fanxiaobao.xyz/Article/details/gatitasni.sHtML

[F12] CSV 读写
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjcvxajw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbeyqrqo.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.fanxiaobao.xyz/Article/details/gkqajuque.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.fanxiaobao.xyz/Article/details/ghkjmkzaf.sHtML

TS:   // 同上
来源：http://mobile.fanxiaobao.xyz/Article/details/gflapdify.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwqdixxq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.fanxiaobao.xyz/Article/details/gfmjvyemm.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfkmmyba.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fanxiaobao.xyz/Article/details/gzggogddj.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdslbyah.sHtML

G. 面向对象
来源：http://baike.fanxiaobao.xyz/Article/details/gucpzizja.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxudzkas.sHtML

[G01] 定义类
来源：http://wap.fanxiaobao.xyz/Article/details/guhaziauo.sHtML

Py:   class User: pass
来源：http://wap.fanxiaobao.xyz/Article/details/gswodytyd.sHtML

PHP:  class User {}
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdbmrssk.sHtML

JS:   class User {}
来源：http://blog.fanxiaobao.xyz/Article/details/gnprzsmot.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzklghie.sHtML

Java: class User {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gcsjcarvw.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnnwwipe.sHtML

Ruby: class User; end
来源：http://wap.fanxiaobao.xyz/Article/details/gvmhbpiob.sHtML

C#:   class User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxggvcic.sHtML

[G02] 构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/ghgqmpuus.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fanxiaobao.xyz/Article/details/gqiwcjujd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gnhishegv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fanxiaobao.xyz/Article/details/garnwqjop.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gbfavlgza.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/golrlbmxu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwgmfmaqm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.fanxiaobao.xyz/Article/details/gifxrpocy.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvlnwszh.sHtML

[G03] 实例属性
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzvkwyfj.sHtML

Py:   self.name = "x"
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdoekbri.sHtML

PHP:  public string $name = "x";
来源：http://3g.fanxiaobao.xyz/Article/details/gqlocsijm.sHtML

JS:   this.name = "x";
来源：http://baike.fanxiaobao.xyz/Article/details/gglueixqc.sHtML

TS:   name: string = "x";
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvjlpire.sHtML

Java: private String name;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvjsrmlj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gapgyhdxt.sHtML

Ruby: @name = "x"
来源：http://3g.fanxiaobao.xyz/Article/details/gifsekeuj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.fanxiaobao.xyz/Article/details/gjckketag.sHtML

[G04] 定义方法
来源：http://www.blog.fanxiaobao.xyz/Article/details/golqrnijq.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fanxiaobao.xyz/Article/details/goyynpzqv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvpvmlft.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcybzqery.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdgqezpr.sHtML

Java: String greet() { return name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gvjlradwi.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fanxiaobao.xyz/Article/details/gocawwmmf.sHtML

Ruby: def greet; @name; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gihpsielv.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhhlcmti.sHtML

[G05] 继承
来源：http://blog.fanxiaobao.xyz/Article/details/gbfumgqbc.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fanxiaobao.xyz/Article/details/gywadtwnh.sHtML

PHP:  class Admin extends User {}
来源：http://baike.fanxiaobao.xyz/Article/details/gvdfkwgbq.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fanxiaobao.xyz/Article/details/geptxtkyb.sHtML

TS:   class Admin extends User {}
来源：http://blog.fanxiaobao.xyz/Article/details/gkxqbwyqy.sHtML

Java: class Admin extends User {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqnpktne.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fanxiaobao.xyz/Article/details/ggoaythyg.sHtML

Ruby: class Admin < User; end
来源：http://3g.fanxiaobao.xyz/Article/details/grxyagxiw.sHtML

C#:   class Admin : User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwjbqofp.sHtML

[G06] 重写方法
来源：http://m.share.fanxiaobao.xyz/Article/details/gropffbqq.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fanxiaobao.xyz/Article/details/gxkhgfipd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbiuivsug.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gknigwggl.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goultaxzb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gmsurbkad.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.fanxiaobao.xyz/Article/details/goqkjrbkk.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fanxiaobao.xyz/Article/details/glltytpgt.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fanxiaobao.xyz/Article/details/gaofcrvgj.sHtML

[G07] 调用父类方法
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcgusunug.sHtML

Py:   super().greet()
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxedofpn.sHtML

PHP:  parent::greet();
来源：http://wap.fanxiaobao.xyz/Article/details/gasraggil.sHtML

JS:   super.greet();
来源：http://www.share.fanxiaobao.xyz/Article/details/gtlxgqdrr.sHtML

TS:   super.greet();
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfwroqzc.sHtML

Java: super.greet();
来源：http://read.share.fanxiaobao.xyz/Article/details/gcsudhplv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedsswswm.sHtML

Ruby: super
来源：http://baike.fanxiaobao.xyz/Article/details/gclpiytqk.sHtML

C#:   base.Greet();
来源：http://mobile.fanxiaobao.xyz/Article/details/ggpqtncnv.sHtML

[G08] 静态方法与属性
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvrnbplx.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.fanxiaobao.xyz/Article/details/gufeqilgj.sHtML

PHP:  public static function f() {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gilsjoykl.sHtML

JS:   static f() {}
来源：http://read.share.fanxiaobao.xyz/Article/details/goyzhqwzu.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefnylldg.sHtML

Java: static void f() {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gmseiyxhu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.fanxiaobao.xyz/Article/details/gaafadpup.sHtML

Ruby: def self.f; end
来源：http://blog.fanxiaobao.xyz/Article/details/gmouoenbm.sHtML

C#:   public static void F() {}
来源：http://mobile.fanxiaobao.xyz/Article/details/genxwxbrz.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.fanxiaobao.xyz/Article/details/ggezacmkr.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fanxiaobao.xyz/Article/details/gcflqcdqo.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakirbqxu.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobphysfh.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjnyigrbg.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcklzyupl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gigptgjac.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gftnowjnk.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gyrdnmkbv.sHtML

[G10] 访问控制
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdxhtcby.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.fanxiaobao.xyz/Article/details/gxwcktmdi.sHtML

PHP:  public / protected / private
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkylvdfas.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gelhdcjdp.sHtML

TS:   public / protected / private
来源：http://blog.fanxiaobao.xyz/Article/details/githkembc.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjltojmzb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fanxiaobao.xyz/Article/details/gocwmtdps.sHtML

Ruby: public / protected / private
来源：http://3g.fanxiaobao.xyz/Article/details/gbrmiwfbb.sHtML


<!-- 参考信息 -->