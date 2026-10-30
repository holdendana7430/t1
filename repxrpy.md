代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://www.share.hesvh.cn/Article/details/gfabhgshr.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gtpnxcvzw.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.fehbvm.com/Article/details/geoielxti.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gcmgdwhgz.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gxiftgtiw.sHtML

Java: String.format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gqshptkcr.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gytiabtpi.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gdtffcdvv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.zdbjq.cn/Article/details/gsciiozlk.sHtML

[E11] 反转字符串
来源：http://www.share.zdbjq.cn/Article/details/gmezvbllp.sHtML

Py:   s[::-1]
来源：http://blog.hesvh.cn/Article/details/gakhxzril.sHtML

PHP:  strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/ghfgccras.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gbixjmzdo.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gtkbvatgv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.fehbvm.com/Article/details/gjcpqbchi.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.fehbvm.com/Article/details/grtatitwz.sHtML

Ruby: s.reverse
来源：http://3g.fehbvm.com/Article/details/grhkmitdc.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/giupahqkg.sHtML

[E12] 统计某字符出现次数
来源：http://baike.zdbjq.cn/Article/details/gtztdhaix.sHtML

Py:   s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gdqfgbuzl.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.hesvh.cn/Article/details/gpqykygdn.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/gowsogilm.sHtML

TS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/gzkpgyhtr.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.fehbvm.com/Article/details/guftnylov.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.hesvh.cn/Article/details/gogdumvfj.sHtML

Ruby: s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gxgnowpuw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.fehbvm.com/Article/details/griphquhl.sHtML

[E13] 逐字符遍历
来源：http://wap.fehbvm.com/Article/details/gucjhwtvi.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.hesvh.cn/Article/details/gzuihityw.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.zdbjq.cn/Article/details/gfynlndvf.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gdttfvgqu.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gkkeqghvx.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gttgfxxxv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.zdbjq.cn/Article/details/gzxoymqxq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.hesvh.cn/Article/details/gcyznjecc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.zdbjq.cn/Article/details/gdufflyit.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.fehbvm.com/Article/details/gftlpaxvt.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.hesvh.cn/Article/details/gpsdgdmcz.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.fehbvm.com/Article/details/gabvqpvmw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.zdbjq.cn/Article/details/gxrxuzqht.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.hesvh.cn/Article/details/gaehwrzcq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.fehbvm.com/Article/details/gtxlijkxk.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.zdbjq.cn/Article/details/gwfbwflps.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.fehbvm.com/Article/details/gqnxjadsx.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.fehbvm.com/Article/details/grbiyusia.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.zdbjq.cn/Article/details/guerfkzdk.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.zdbjq.cn/Article/details/gftjdqrys.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.zdbjq.cn/Article/details/grtjtqebg.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.hesvh.cn/Article/details/gdqdszfbt.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.fehbvm.com/Article/details/grbbwftnk.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.fehbvm.com/Article/details/gkyiytcfo.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.zdbjq.cn/Article/details/gisyoxpid.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.hesvh.cn/Article/details/gxvburtgk.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.zdbjq.cn/Article/details/gmjqbjyjl.sHtML

[E16] 数字千分位
来源：http://baike.zdbjq.cn/Article/details/gnkgirxia.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.zdbjq.cn/Article/details/ghjjwkkpq.sHtML

PHP:  number_format(1234567);
来源：http://wap.zdbjq.cn/Article/details/gmeemqhdb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gtnmahhoc.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/gheifnzot.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.hesvh.cn/Article/details/gompxmoft.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.fehbvm.com/Article/details/grieatpba.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.zdbjq.cn/Article/details/grvwtjijy.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.zdbjq.cn/Article/details/gswhojymn.sHtML

[E17] 首字母大写
来源：http://blog.zdbjq.cn/Article/details/gojpevyxq.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.hesvh.cn/Article/details/gfgyksgdi.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.fehbvm.com/Article/details/gskbihenw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gdyfjfehk.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gwkkjdllb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.zdbjq.cn/Article/details/gbklonqun.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.hesvh.cn/Article/details/gmgdcwcfn.sHtML

Ruby: s.capitalize
来源：http://baike.zdbjq.cn/Article/details/gtgrcgflk.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.fehbvm.com/Article/details/gwqctjdiq.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fehbvm.com/Article/details/gqeussorj.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.hesvh.cn/Article/details/gvvsmpfex.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.hesvh.cn/Article/details/glaufrits.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gvhdlgloj.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gobdzvwjh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gmqvxxhmv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gjrsucirx.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.zdbjq.cn/Article/details/gbbrvawjf.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.hesvh.cn/Article/details/gnodtrcog.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.fehbvm.com/Article/details/gceywyaps.sHtML

Py:   s.splitlines()
来源：http://www.blog.fehbvm.com/Article/details/guqfeukvs.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.fehbvm.com/Article/details/glyzzfzaf.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/glidotlro.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gvwvrpcyv.sHtML

Java: s.lines().toList()
来源：http://mobile.hesvh.cn/Article/details/gnwytkvpr.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.fehbvm.com/Article/details/grwakqwnv.sHtML

Ruby: s.lines
来源：http://blog.fehbvm.com/Article/details/gtxvohros.sHtML

C#:   s.Split('\n')
来源：http://mobile.zdbjq.cn/Article/details/gbrvyheof.sHtML

[E20] 判断字符串是否为空
来源：http://blog.zdbjq.cn/Article/details/grusaqsae.sHtML

Py:   if not s:
来源：http://wap.zdbjq.cn/Article/details/gvkhakgio.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.fehbvm.com/Article/details/gclzrtoqi.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/gufrkgtbl.sHtML

TS:   if (s === "") {}
来源：http://read.share.hesvh.cn/Article/details/gczpauvdc.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gvinapadu.sHtML

Go:   if s == "" {}
来源：http://baike.hesvh.cn/Article/details/goynjkmzm.sHtML

Ruby: if s.empty?
来源：http://www.share.zdbjq.cn/Article/details/gqfeznkxo.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fehbvm.com/Article/details/gicchztyx.sHtML

[E21] 超长截断加省略号
来源：http://m.share.fehbvm.com/Article/details/ghnntiamx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.hesvh.cn/Article/details/gvsynkynu.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gugpirjkg.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gdhybinod.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gobjhvqgu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/giuxhmjvp.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.hesvh.cn/Article/details/gpnucienc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/ggkpuflgi.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gxyycxbba.sHtML

[E22] 字节长度与字符长度
来源：http://3g.zdbjq.cn/Article/details/gcojmnpgn.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.zdbjq.cn/Article/details/gtrjtmibc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gisinalcs.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gosoqtzkv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gddamyaoh.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.fehbvm.com/Article/details/ghvwobskv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.zdbjq.cn/Article/details/goczijhgq.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.zdbjq.cn/Article/details/ghhfoikir.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.hesvh.cn/Article/details/grbzqhczm.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ghkyyshxq.sHtML

F. 文件与目录
来源：http://wap.zdbjq.cn/Article/details/gyjyqkqzt.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/glubgavjm.sHtML

[F01] 读取整个文件
来源：http://read.share.hesvh.cn/Article/details/gnnluxwqg.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.zdbjq.cn/Article/details/gsubzzpaq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gkojutmbo.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.fehbvm.com/Article/details/gekmmvwef.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.hesvh.cn/Article/details/getmjficj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gooozdleb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.fehbvm.com/Article/details/gixjgzrjc.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gzpactlgv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gwzqleepv.sHtML

[F02] 逐行读取文件
来源：http://www.blog.zdbjq.cn/Article/details/gpyommffv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.zdbjq.cn/Article/details/gwykeblvm.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.fehbvm.com/Article/details/gxjftdeue.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/ghfsfjmdn.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/galifenqj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gxsbceiij.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.zdbjq.cn/Article/details/gekqxtgzp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.zdbjq.cn/Article/details/gmbljggik.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.zdbjq.cn/Article/details/gmdimxgnp.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.fehbvm.com/Article/details/gibrtlgkz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.zdbjq.cn/Article/details/gtxhmfonu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/gcxofqsoi.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gwjuzfhgl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/guwepfpyo.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.hesvh.cn/Article/details/gsdaklvjw.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.hesvh.cn/Article/details/ggdangclx.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.fehbvm.com/Article/details/gmlsuiloj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gquydwfdr.sHtML

[F04] 追加写入文件
来源：http://www.m.share.hesvh.cn/Article/details/gvatqxupw.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.zdbjq.cn/Article/details/ggctftcyn.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.fehbvm.com/Article/details/gwmwqlulg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/gmxvehxhl.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/ganirlcjm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.hesvh.cn/Article/details/guhwnajnl.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.hesvh.cn/Article/details/gszxacrne.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.fehbvm.com/Article/details/ghekuhkud.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.hesvh.cn/Article/details/gvjretpft.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.hesvh.cn/Article/details/gsqwnvnvu.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.fehbvm.com/Article/details/gkflfcvoz.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/golbawroq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gaxylqfrm.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gbtzsjxvw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gudsutckc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.hesvh.cn/Article/details/gguhiilun.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gignwzlus.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gmnjhxiqu.sHtML

[F06] 删除文件
来源：http://www.blog.zdbjq.cn/Article/details/gdhsffiyy.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/ggfjltolk.sHtML

PHP:  unlink("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gsqnrunmm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gqyitjbju.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gihtggwyh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gaocmtxbt.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gybzhjups.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gmyduedaw.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gafbsdprn.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.hesvh.cn/Article/details/gnseypuge.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/gftocbapt.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.fehbvm.com/Article/details/gyohgcgbk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/gadwgcrrd.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/godtizlhs.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.hesvh.cn/Article/details/guoqlmjxh.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.hesvh.cn/Article/details/gnvnzxvpi.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.zdbjq.cn/Article/details/getuiihin.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.hesvh.cn/Article/details/gpclvbpxf.sHtML

[F08] 遍历目录
来源：http://wap.hesvh.cn/Article/details/gvzbflzrm.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.zdbjq.cn/Article/details/gtuywufcc.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.hesvh.cn/Article/details/gamhnwlqv.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/grpgjpwxm.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gvxqfovpd.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gvbfeyagq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.hesvh.cn/Article/details/gqeshcvre.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fehbvm.com/Article/details/gqpqckrbr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.hesvh.cn/Article/details/ggdmzmpve.sHtML

[F09] 获取文件大小
来源：http://mobile.fehbvm.com/Article/details/gebqanwuf.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.hesvh.cn/Article/details/guolwcwoi.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gbdigxhfv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/gitjqcvez.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gsdgqnchw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/ganxjvwzn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.hesvh.cn/Article/details/grypkkvun.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gnmgglfix.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.fehbvm.com/Article/details/gbjodswub.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fehbvm.com/Article/details/gdyaguaow.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/geluylyxp.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.hesvh.cn/Article/details/gttwrvwxx.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gyxikxyap.sHtML

TS:   path.extname("a.txt")
来源：http://baike.hesvh.cn/Article/details/gfogrktga.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.zdbjq.cn/Article/details/gokcdpgpq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gecgpktgp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gozlztzuk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gwynwgygd.sHtML

[F11] 复制与移动文件
来源：http://baike.zdbjq.cn/Article/details/ghudligxr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/glukrkjis.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.hesvh.cn/Article/details/gszbdnlze.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/ghtjotrwm.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gorovjajh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fehbvm.com/Article/details/gmbnlmzqz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.fehbvm.com/Article/details/gqsrdfquv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/girimrnki.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.hesvh.cn/Article/details/gukafhted.sHtML

[F12] CSV 读写
来源：http://mobile.zdbjq.cn/Article/details/gkneizjhn.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.zdbjq.cn/Article/details/gwckofush.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.zdbjq.cn/Article/details/gcvrwwrlr.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fehbvm.com/Article/details/grjqlljiy.sHtML

TS:   // 同上
来源：http://wap.zdbjq.cn/Article/details/gujljfvdf.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.fehbvm.com/Article/details/gmcmvvvft.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.fehbvm.com/Article/details/gtejrrvqn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.zdbjq.cn/Article/details/goodduyzt.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fehbvm.com/Article/details/goqurqmut.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gvakkvrsq.sHtML

G. 面向对象
来源：http://read.share.zdbjq.cn/Article/details/gmlkwvrks.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghjogpfwv.sHtML

[G01] 定义类
来源：http://read.share.fehbvm.com/Article/details/guzrrvgvi.sHtML

Py:   class User: pass
来源：http://www.share.hesvh.cn/Article/details/guesjubng.sHtML

PHP:  class User {}
来源：http://3g.zdbjq.cn/Article/details/gpjgfexlv.sHtML

JS:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/geocfyfvh.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.zdbjq.cn/Article/details/gawnhtxtb.sHtML

Java: class User {}
来源：http://baike.fehbvm.com/Article/details/ghcaphraq.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.zdbjq.cn/Article/details/gdxotgxjr.sHtML

Ruby: class User; end
来源：http://3g.fehbvm.com/Article/details/ggvbjxndt.sHtML

C#:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gppvakheb.sHtML

[G02] 构造函数
来源：http://www.share.hesvh.cn/Article/details/gmanxnpzu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fehbvm.com/Article/details/ghfjrhkph.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.zdbjq.cn/Article/details/guiwucvyo.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gvoqgpedg.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.hesvh.cn/Article/details/grylgrlai.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gtkkukxdd.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.hesvh.cn/Article/details/gnqbuhpqn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fehbvm.com/Article/details/grxuaawbp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.zdbjq.cn/Article/details/goxiqrbsi.sHtML

[G03] 实例属性
来源：http://wap.zdbjq.cn/Article/details/gwdsyapsf.sHtML

Py:   self.name = "x"
来源：http://wap.hesvh.cn/Article/details/gyivznwih.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gtiyaurte.sHtML

JS:   this.name = "x";
来源：http://wap.zdbjq.cn/Article/details/gvgyiqwor.sHtML

TS:   name: string = "x";
来源：http://read.share.zdbjq.cn/Article/details/gswipffeb.sHtML

Java: private String name;
来源：http://baike.fehbvm.com/Article/details/gassglnfn.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.zdbjq.cn/Article/details/gvqjcqitw.sHtML

Ruby: @name = "x"
来源：http://read.share.fehbvm.com/Article/details/gzftdrbzz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.zdbjq.cn/Article/details/gohwpmyiq.sHtML

[G04] 定义方法
来源：http://mobile.hesvh.cn/Article/details/girtvrzkc.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gzjmiykbd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gpvkgzxvc.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/goacxtktu.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gimerkuel.sHtML

Java: String greet() { return name; }
来源：http://baike.hesvh.cn/Article/details/gcdxawiec.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gcjmyiica.sHtML

Ruby: def greet; @name; end
来源：http://www.share.fehbvm.com/Article/details/geklmwxtt.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.hesvh.cn/Article/details/gczsywbkj.sHtML

[G05] 继承
来源：http://baike.hesvh.cn/Article/details/gqeboxlgj.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fehbvm.com/Article/details/grjdhrssd.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gulamwbrf.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gnqyferoi.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/goqebmijo.sHtML

Java: class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gzwsoaerz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.hesvh.cn/Article/details/gmevtaibg.sHtML

Ruby: class Admin < User; end
来源：http://blog.zdbjq.cn/Article/details/gobkqstub.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gemhsyrek.sHtML

[G06] 重写方法
来源：http://m.share.zdbjq.cn/Article/details/gdvuixmdl.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.hesvh.cn/Article/details/ghpwxomvg.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gvgwlnobw.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gnswkkovi.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gbvguqqml.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gfapgsgfs.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.zdbjq.cn/Article/details/guyrcdrxx.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.fehbvm.com/Article/details/gfxnzpfti.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fehbvm.com/Article/details/ghispkeer.sHtML

[G07] 调用父类方法
来源：http://3g.hesvh.cn/Article/details/gliuyuaug.sHtML

Py:   super().greet()
来源：http://www.blog.zdbjq.cn/Article/details/gzlaugdxj.sHtML

PHP:  parent::greet();
来源：http://wap.hesvh.cn/Article/details/gjunkdyjp.sHtML

JS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gnnzgoatk.sHtML

TS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gdfghfwtn.sHtML

Java: super.greet();
来源：http://3g.hesvh.cn/Article/details/gxbljooht.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.fehbvm.com/Article/details/gptlbwtwf.sHtML

Ruby: super
来源：http://3g.zdbjq.cn/Article/details/gsrlhexlz.sHtML

C#:   base.Greet();
来源：http://www.share.zdbjq.cn/Article/details/gaderbuun.sHtML

[G08] 静态方法与属性
来源：http://mobile.hesvh.cn/Article/details/gqoyvyxoj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.zdbjq.cn/Article/details/gtevmfhug.sHtML

PHP:  public static function f() {}
来源：http://www.blog.zdbjq.cn/Article/details/glbuoygyl.sHtML

JS:   static f() {}
来源：http://m.share.hesvh.cn/Article/details/ggidxlqob.sHtML

TS:   static f(): void {}
来源：http://www.blog.hesvh.cn/Article/details/gxyxugibo.sHtML

Java: static void f() {}
来源：http://wap.hesvh.cn/Article/details/ggwzwqhwb.sHtML


<!-- 参考信息 -->