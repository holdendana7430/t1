代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://wap.hesvh.cn/Article/details/gthacelwh.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.fehbvm.com/Article/details/gzrrcenbq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.fehbvm.com/Article/details/gkeeovpki.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gebpfudai.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.hesvh.cn/Article/details/ggywijbqn.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gcditmtms.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.hesvh.cn/Article/details/gmtbmixlc.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gxpywpuyb.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/ghgqfzxer.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gqkmlnsdl.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gktyewsif.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gnpxbmgev.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.fehbvm.com/Article/details/gyliasoaz.sHtML

[E11] 反转字符串
来源：http://baike.hesvh.cn/Article/details/ggcxxkyuz.sHtML

Py:   s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gghnqemxx.sHtML

PHP:  strrev($s);
来源：http://www.share.hesvh.cn/Article/details/gygcydrbi.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gotsindyu.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/ghqwskmzq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.fehbvm.com/Article/details/gtwkskgvy.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.zdbjq.cn/Article/details/gdduqwpmb.sHtML

Ruby: s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gnvtatizb.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/gzlermlgz.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.zdbjq.cn/Article/details/gwmotsqdz.sHtML

Py:   s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/ggdzerbdg.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.fehbvm.com/Article/details/gqpkecpdf.sHtML

JS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gdcdavawd.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/ghncxaxol.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.hesvh.cn/Article/details/gifsaerqp.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.zdbjq.cn/Article/details/gntixisjv.sHtML

Ruby: s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gubjpqosv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.fehbvm.com/Article/details/gwtpocsio.sHtML

[E13] 逐字符遍历
来源：http://m.share.zdbjq.cn/Article/details/gblszwihr.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.zdbjq.cn/Article/details/gotgkufbv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.fehbvm.com/Article/details/ginkctsyo.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gudqfldsb.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/ggnhuvhai.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.fehbvm.com/Article/details/gwdtumgkl.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.zdbjq.cn/Article/details/girmoxcqd.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.zdbjq.cn/Article/details/gpnfgziia.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.fehbvm.com/Article/details/gjxngxdme.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.zdbjq.cn/Article/details/gnhggvpdq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.fehbvm.com/Article/details/gjwevehyw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.fehbvm.com/Article/details/gugveeppt.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.hesvh.cn/Article/details/gqxwwrdvo.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.fehbvm.com/Article/details/gspfupqge.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gvcctqlqp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.zdbjq.cn/Article/details/gtjnogvvr.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.hesvh.cn/Article/details/gjqtikxgb.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.zdbjq.cn/Article/details/grjnmembr.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.fehbvm.com/Article/details/gmburmwst.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.hesvh.cn/Article/details/gqdcocghm.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.fehbvm.com/Article/details/gaqqwljzx.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.hesvh.cn/Article/details/gbpcvapeh.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.fehbvm.com/Article/details/gisxawglt.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.hesvh.cn/Article/details/gqpvmqhvd.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.fehbvm.com/Article/details/gpwtfoouy.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.fehbvm.com/Article/details/gwunpoxbi.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.hesvh.cn/Article/details/gojyofknq.sHtML

[E16] 数字千分位
来源：http://baike.fehbvm.com/Article/details/gsulslwjn.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.zdbjq.cn/Article/details/gneixvppa.sHtML

PHP:  number_format(1234567);
来源：http://baike.zdbjq.cn/Article/details/gsxprccbn.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/ggntucdpv.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/gcmudjbpa.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gjyblodad.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.zdbjq.cn/Article/details/gsdyhnkiq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.hesvh.cn/Article/details/gibopayig.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.hesvh.cn/Article/details/gsuvcwlhx.sHtML

[E17] 首字母大写
来源：http://blog.zdbjq.cn/Article/details/gmdhbbmwb.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.fehbvm.com/Article/details/gemfugjxe.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.hesvh.cn/Article/details/gbghctgpl.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gxhahpkwy.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/gzckefimy.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.zdbjq.cn/Article/details/gzekrkxra.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gnmcvsgcp.sHtML

Ruby: s.capitalize
来源：http://wap.zdbjq.cn/Article/details/gmwwrqlng.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.zdbjq.cn/Article/details/ghhtmongf.sHtML

[E18] 模板占位符替换
来源：http://mobile.hesvh.cn/Article/details/gljtnzxqp.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.zdbjq.cn/Article/details/gventvbnq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.zdbjq.cn/Article/details/grzyvsckz.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gzpmzshgm.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gifmmhujw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fehbvm.com/Article/details/ghpezmzab.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.fehbvm.com/Article/details/gbbbmovhz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.zdbjq.cn/Article/details/gjukvhunx.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.zdbjq.cn/Article/details/geafitpdq.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fehbvm.com/Article/details/grltsmazt.sHtML

Py:   s.splitlines()
来源：http://read.share.hesvh.cn/Article/details/gxhegpvkn.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.zdbjq.cn/Article/details/gbrvgbknx.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/gdjxzayzc.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/gyxqnuzss.sHtML

Java: s.lines().toList()
来源：http://read.share.fehbvm.com/Article/details/ggfgevuuf.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.zdbjq.cn/Article/details/glwchvnut.sHtML

Ruby: s.lines
来源：http://3g.zdbjq.cn/Article/details/goasrrirk.sHtML

C#:   s.Split('\n')
来源：http://www.share.fehbvm.com/Article/details/gyzimuixj.sHtML

[E20] 判断字符串是否为空
来源：http://3g.fehbvm.com/Article/details/gaadjifqr.sHtML

Py:   if not s:
来源：http://3g.fehbvm.com/Article/details/gfxqclepz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.zdbjq.cn/Article/details/gagxrjgjr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.hesvh.cn/Article/details/gxqereyqv.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.hesvh.cn/Article/details/golpnzvwg.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/gaesklrfx.sHtML

Go:   if s == "" {}
来源：http://read.share.fehbvm.com/Article/details/glxawdiwl.sHtML

Ruby: if s.empty?
来源：http://baike.zdbjq.cn/Article/details/gschohlvg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.hesvh.cn/Article/details/gxkonzdzr.sHtML

[E21] 超长截断加省略号
来源：http://baike.zdbjq.cn/Article/details/gedyamyhh.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.hesvh.cn/Article/details/gtkldhbkx.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gaoxnovdy.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gxemhplgz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gjtfukhyb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gprhvisqp.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.hesvh.cn/Article/details/gafsdqsdx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gruvczvjb.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gcxlfywuz.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.zdbjq.cn/Article/details/gshfscxvb.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.fehbvm.com/Article/details/gliaimhmv.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gggahdtyf.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/gvyxdfxnu.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gixtegubh.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.fehbvm.com/Article/details/gvceuwovd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.fehbvm.com/Article/details/gwduvaiyh.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gagtblecw.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.fehbvm.com/Article/details/gvpepalzd.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gocaiczsr.sHtML

F. 文件与目录
来源：http://www.blog.zdbjq.cn/Article/details/grspnmttt.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/galywedev.sHtML

[F01] 读取整个文件
来源：http://wap.zdbjq.cn/Article/details/gpcowjkyp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.zdbjq.cn/Article/details/grtqcwaog.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gnxhpimbu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.hesvh.cn/Article/details/gzhsvbktd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gymbivedc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gxwhcnjmt.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.hesvh.cn/Article/details/gmevxakev.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gpoepkjof.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gmdgvdcey.sHtML

[F02] 逐行读取文件
来源：http://blog.fehbvm.com/Article/details/gtgwgvwty.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.fehbvm.com/Article/details/gseanastd.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gzrjwufyx.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gkpponuki.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/geyyoaquh.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gpyytqzyx.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.hesvh.cn/Article/details/gqqclsxdn.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.fehbvm.com/Article/details/ghnsbunnm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.zdbjq.cn/Article/details/gcnjctrci.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.hesvh.cn/Article/details/grogkerdp.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.hesvh.cn/Article/details/gpdmifgun.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gwkdjwubg.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/guusfaigk.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gknemlglm.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.zdbjq.cn/Article/details/gibqxtjyz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.zdbjq.cn/Article/details/gixgcuncw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.zdbjq.cn/Article/details/gtxzjzlvl.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gbknvjusn.sHtML

[F04] 追加写入文件
来源：http://wap.zdbjq.cn/Article/details/gwqwtwldc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.zdbjq.cn/Article/details/ggdsigvih.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.fehbvm.com/Article/details/gvkolqgxo.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/gqcccwchd.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gufzdispf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.zdbjq.cn/Article/details/gjiucdlbe.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gbwvrayik.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.zdbjq.cn/Article/details/gnijbtjeh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.fehbvm.com/Article/details/gvggnsrbv.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.zdbjq.cn/Article/details/gtikwwknl.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.fehbvm.com/Article/details/gcqnpaulv.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gczrgxazk.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gaeahthcg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gvsfhzszs.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/ghpgruslf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.fehbvm.com/Article/details/gcnlkrapb.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.fehbvm.com/Article/details/gvltmfukj.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gpselczpj.sHtML

[F06] 删除文件
来源：http://www.share.zdbjq.cn/Article/details/grnolyvmg.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/ghvusonoc.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gdwsxnwfi.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gpfeiuwov.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gvrpfxgsw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gzfffieln.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gmqryvjku.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gavlaflsh.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gqsczhsow.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.fehbvm.com/Article/details/gjjfrjuik.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gvupdvhil.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.fehbvm.com/Article/details/gosiyuezi.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gjcdjpgun.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gsnhgitah.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fehbvm.com/Article/details/gkrwhliac.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.zdbjq.cn/Article/details/gdeugzrjr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.fehbvm.com/Article/details/goupvrzir.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.fehbvm.com/Article/details/gkvnpguat.sHtML

[F08] 遍历目录
来源：http://www.m.share.hesvh.cn/Article/details/gorxxtgki.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.zdbjq.cn/Article/details/grqfsiwbl.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.zdbjq.cn/Article/details/gbxggskee.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/gyqcmschu.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gupflckei.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/ggxyjlfcc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.fehbvm.com/Article/details/gbajyaoej.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.zdbjq.cn/Article/details/glkpghnij.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.zdbjq.cn/Article/details/gollrjwyv.sHtML

[F09] 获取文件大小
来源：http://www.share.zdbjq.cn/Article/details/gdunnjebu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gockgmrqf.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.hesvh.cn/Article/details/ggmaeudqf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/gfcnihqmg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gqafspkkd.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gcoddzmea.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fehbvm.com/Article/details/gdfkujncw.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.hesvh.cn/Article/details/guljscdrw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.zdbjq.cn/Article/details/gmewrdseo.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.fehbvm.com/Article/details/gpqjcqtcq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gtpgpeflc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gzqzkkilz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gwzuiqqao.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gpuwoypad.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.zdbjq.cn/Article/details/gplfepgxi.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gupgafslu.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/giyhvijtk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gplrktcos.sHtML

[F11] 复制与移动文件
来源：http://m.share.hesvh.cn/Article/details/gaamcwfek.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gcamsqszo.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.fehbvm.com/Article/details/gmkbtauaz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gzzlhtwzk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gftdnszdz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gelsxtvmk.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.zdbjq.cn/Article/details/gfdbkjjmq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gezyevvki.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.zdbjq.cn/Article/details/gdavxhkux.sHtML

[F12] CSV 读写
来源：http://read.share.fehbvm.com/Article/details/gtjyqktim.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.zdbjq.cn/Article/details/gvaadmqyf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fehbvm.com/Article/details/gducofqwi.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.zdbjq.cn/Article/details/gmzqeccho.sHtML

TS:   // 同上
来源：http://m.share.fehbvm.com/Article/details/geqjrmbny.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fehbvm.com/Article/details/glhraqykh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.fehbvm.com/Article/details/gkhcldvhc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.hesvh.cn/Article/details/ggewsouhq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.zdbjq.cn/Article/details/gewgrzszu.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gksownpqn.sHtML

G. 面向对象
来源：http://baike.zdbjq.cn/Article/details/gexxyqpjy.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gdmqopmgh.sHtML

[G01] 定义类
来源：http://m.share.zdbjq.cn/Article/details/gglittfvg.sHtML

Py:   class User: pass
来源：http://read.share.zdbjq.cn/Article/details/gpferpgtl.sHtML

PHP:  class User {}
来源：http://baike.zdbjq.cn/Article/details/gpeejuuze.sHtML

JS:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gidqnyiwq.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.hesvh.cn/Article/details/gpmmzglyv.sHtML

Java: class User {}
来源：http://read.share.hesvh.cn/Article/details/gjnayxehs.sHtML

Go:   type User struct { Name string }
来源：http://m.share.hesvh.cn/Article/details/gafhofiju.sHtML

Ruby: class User; end
来源：http://www.share.hesvh.cn/Article/details/gxayxpjsf.sHtML

C#:   class User {}
来源：http://read.share.fehbvm.com/Article/details/guemrhnsp.sHtML

[G02] 构造函数
来源：http://read.share.fehbvm.com/Article/details/gdaayyjhd.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.zdbjq.cn/Article/details/giuyycirg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.hesvh.cn/Article/details/gdvrldpsh.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggbrpvgxi.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.hesvh.cn/Article/details/gztrhfwdq.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gkivpljwi.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fehbvm.com/Article/details/gwicbswph.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.hesvh.cn/Article/details/glyzvwzhy.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.fehbvm.com/Article/details/gxumtqaaz.sHtML

[G03] 实例属性
来源：http://mobile.fehbvm.com/Article/details/ggbbvkumb.sHtML

Py:   self.name = "x"
来源：http://3g.zdbjq.cn/Article/details/gbtrxraeb.sHtML

PHP:  public string $name = "x";
来源：http://baike.zdbjq.cn/Article/details/gnryhjyqp.sHtML

JS:   this.name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gkakudefa.sHtML

TS:   name: string = "x";
来源：http://wap.fehbvm.com/Article/details/gsisbtide.sHtML

Java: private String name;
来源：http://baike.fehbvm.com/Article/details/gesuwzvxs.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.zdbjq.cn/Article/details/gqupwprdf.sHtML

Ruby: @name = "x"
来源：http://mobile.hesvh.cn/Article/details/gwzsplphy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.hesvh.cn/Article/details/gptsozxvn.sHtML

[G04] 定义方法
来源：http://mobile.zdbjq.cn/Article/details/gxavayoch.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gsydxebpd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/glydtkhrx.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gyniemgvs.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gxzlaauql.sHtML

Java: String greet() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gzuoepqai.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gzcdnqmoe.sHtML

Ruby: def greet; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gxovqqsgc.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.hesvh.cn/Article/details/golsnxozz.sHtML

[G05] 继承
来源：http://blog.fehbvm.com/Article/details/gnujlzldu.sHtML

Py:   class Admin(User): pass
来源：http://wap.fehbvm.com/Article/details/ghbqrupso.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/givjpqwxh.sHtML

JS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gnytxiffh.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gdgiqmztf.sHtML

Java: class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gxtpoahyr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.zdbjq.cn/Article/details/gikicqhqs.sHtML

Ruby: class Admin < User; end
来源：http://wap.hesvh.cn/Article/details/gxdvenzso.sHtML

C#:   class Admin : User {}
来源：http://www.share.fehbvm.com/Article/details/grdehtpfm.sHtML

[G06] 重写方法
来源：http://read.share.zdbjq.cn/Article/details/gnekzzqwf.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.hesvh.cn/Article/details/gyokuimqx.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gzvlxwicc.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gqzjaldor.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gvkulmpdo.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/ghkukvtep.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.zdbjq.cn/Article/details/gjmaxrtbn.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.hesvh.cn/Article/details/gdjvwjplw.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.zdbjq.cn/Article/details/gtvszywqh.sHtML

[G07] 调用父类方法
来源：http://www.blog.hesvh.cn/Article/details/ggufvlurk.sHtML

Py:   super().greet()
来源：http://3g.hesvh.cn/Article/details/gnrxrmvqc.sHtML

PHP:  parent::greet();
来源：http://read.share.hesvh.cn/Article/details/gaveltipn.sHtML

JS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gqluzeluq.sHtML

TS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gfnuzpsqw.sHtML

Java: super.greet();
来源：http://m.share.hesvh.cn/Article/details/gdhvvnchd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.hesvh.cn/Article/details/ghoudjnmx.sHtML

Ruby: super
来源：http://blog.fehbvm.com/Article/details/gocojcgmv.sHtML

C#:   base.Greet();
来源：http://www.share.zdbjq.cn/Article/details/gfmreobta.sHtML

[G08] 静态方法与属性
来源：http://blog.zdbjq.cn/Article/details/gvjfygylv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.fehbvm.com/Article/details/guxvwvgfn.sHtML


<!-- 参考信息 -->