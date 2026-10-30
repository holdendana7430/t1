代发 wailian999

PHP:  substr_count($s, "a");
来源：http://wap.fanxiaobao.xyz/Article/details/grdfdgyzc.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gagczdbaw.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzpcsjmw.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.fanxiaobao.xyz/Article/details/gilsjauya.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.fanxiaobao.xyz/Article/details/gqprqqelu.sHtML

Ruby: s.count("a")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gekaxeisx.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.fanxiaobao.xyz/Article/details/gmyeclwkf.sHtML

[E13] 逐字符遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gthrjtmvh.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyefyaxad.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzzgtstc.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbwbpljym.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fanxiaobao.xyz/Article/details/gpqguzgdd.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.fanxiaobao.xyz/Article/details/guvwzallp.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.fanxiaobao.xyz/Article/details/ggghgystl.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyymcyrl.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxinwkpfj.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.fanxiaobao.xyz/Article/details/gqsmdwfqo.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.fanxiaobao.xyz/Article/details/giademzex.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.fanxiaobao.xyz/Article/details/getemsjip.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.fanxiaobao.xyz/Article/details/grihmelpu.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gewyuspzk.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.fanxiaobao.xyz/Article/details/gehipywaa.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.fanxiaobao.xyz/Article/details/gmciavhgb.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.fanxiaobao.xyz/Article/details/gppykegkd.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpoivlxbg.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghielatey.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gcymzgwga.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fanxiaobao.xyz/Article/details/gfoimivfc.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gxleioyse.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.fanxiaobao.xyz/Article/details/goccboppb.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.fanxiaobao.xyz/Article/details/gxwyljlwc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjpdwqpa.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdseynqea.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjvtkojy.sHtML

[E16] 数字千分位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacuspipy.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gejsdabqb.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gusehzkri.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxstkyxdj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.fanxiaobao.xyz/Article/details/gmsrlqswq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.fanxiaobao.xyz/Article/details/gjrffcvqr.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gisfydlyx.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.fanxiaobao.xyz/Article/details/gdjwshbkz.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fanxiaobao.xyz/Article/details/graswofck.sHtML

[E17] 首字母大写
来源：http://baike.fanxiaobao.xyz/Article/details/gwldbhiye.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.fanxiaobao.xyz/Article/details/gziutygal.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.fanxiaobao.xyz/Article/details/gwtraojxh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbewcrli.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gfxggjjuc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gouxkzkbs.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtesszqem.sHtML

Ruby: s.capitalize
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfsknmyyo.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqkyiytz.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsilkiphp.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.fanxiaobao.xyz/Article/details/gacrbhouc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmarrgkqp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfbqjgum.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.fanxiaobao.xyz/Article/details/gkapodvpj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsihtxjho.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.fanxiaobao.xyz/Article/details/grolpdetw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gqaosxwiq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpuhlqfip.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fanxiaobao.xyz/Article/details/gebpizqdj.sHtML

Py:   s.splitlines()
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdxdioat.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrhlqtat.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfhznjuu.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grlsqubui.sHtML

Java: s.lines().toList()
来源：http://mobile.fanxiaobao.xyz/Article/details/grcdgdhes.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.fanxiaobao.xyz/Article/details/grktmytpi.sHtML

Ruby: s.lines
来源：http://mobile.fanxiaobao.xyz/Article/details/goydtqtyg.sHtML

C#:   s.Split('\n')
来源：http://www.share.fanxiaobao.xyz/Article/details/gucfvuzhn.sHtML

[E20] 判断字符串是否为空
来源：http://baike.fanxiaobao.xyz/Article/details/glhfjviex.sHtML

Py:   if not s:
来源：http://baike.fanxiaobao.xyz/Article/details/gmoaosjue.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.fanxiaobao.xyz/Article/details/grdleaccm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/ghvuqtuze.sHtML

TS:   if (s === "") {}
来源：http://3g.fanxiaobao.xyz/Article/details/gphkowcpu.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gjqikybiw.sHtML

Go:   if s == "" {}
来源：http://blog.fanxiaobao.xyz/Article/details/gfhouqcut.sHtML

Ruby: if s.empty?
来源：http://baike.fanxiaobao.xyz/Article/details/gcnnpvqwh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gkpbekdnt.sHtML

[E21] 超长截断加省略号
来源：http://blog.fanxiaobao.xyz/Article/details/gkhcuioqj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlvfhbpy.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfqhznev.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fanxiaobao.xyz/Article/details/gjeepvlhq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fanxiaobao.xyz/Article/details/gxgtwekzy.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.fanxiaobao.xyz/Article/details/gmeakkcgc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.fanxiaobao.xyz/Article/details/gkupspjzs.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fanxiaobao.xyz/Article/details/gifufnemx.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.fanxiaobao.xyz/Article/details/gqtovkokd.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjoloqzz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gyyogehct.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fanxiaobao.xyz/Article/details/gbthpfpin.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fanxiaobao.xyz/Article/details/gmvisggwg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fanxiaobao.xyz/Article/details/ggqucxjun.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.fanxiaobao.xyz/Article/details/guprvbdjz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.fanxiaobao.xyz/Article/details/gnodtjqpt.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrmcigld.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthfmtcur.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gblyrdrhv.sHtML

F. 文件与目录
来源：http://wap.fanxiaobao.xyz/Article/details/gtvfszahr.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gtcylljev.sHtML

[F01] 读取整个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/glxpgfbds.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtjijtldj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/gsieawcta.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxlihhjqp.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvidmpjn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.fanxiaobao.xyz/Article/details/grrvvfnsu.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.fanxiaobao.xyz/Article/details/gpumozcga.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtrdwyhv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.fanxiaobao.xyz/Article/details/glxlzhkxk.sHtML

[F02] 逐行读取文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gttrnlhhp.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.fanxiaobao.xyz/Article/details/gjwkswzhv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.fanxiaobao.xyz/Article/details/gnmcmndqo.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giblbftwt.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gojsnkkeg.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdhdsjxl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmkcdutx.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.fanxiaobao.xyz/Article/details/glppigtqx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fanxiaobao.xyz/Article/details/gestoymtq.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fanxiaobao.xyz/Article/details/goydpxsfx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqpjwyfo.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/ggxulmfrz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvqadqrk.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fanxiaobao.xyz/Article/details/gmoojxibm.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwkccjjd.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjdkschw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzropjta.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyrzpptnh.sHtML

[F04] 追加写入文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtcahxtv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fanxiaobao.xyz/Article/details/gwrrzhtvy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggcybkvds.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fanxiaobao.xyz/Article/details/gwyorjxzu.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgdedfvz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.fanxiaobao.xyz/Article/details/gavwhuxbp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grczwrvnq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjjdyltw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.fanxiaobao.xyz/Article/details/ggnbhaxot.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gyukgzcls.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwutlhjr.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjuiiaxv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gjwtwtmsy.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbhuepgq.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkleklvm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.fanxiaobao.xyz/Article/details/gqgjihbjb.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gbnhdtcfq.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpabxvlr.sHtML

[F06] 删除文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxloycbkp.sHtML

Py:   os.remove("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/glwrmneys.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fanxiaobao.xyz/Article/details/gtltrefil.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gibyhllex.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/grtgojweb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqyftblsv.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gamytgqsn.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gyyjgvlnu.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.fanxiaobao.xyz/Article/details/gbgmqmqob.sHtML

[F07] 创建目录（含多级）
来源：http://blog.fanxiaobao.xyz/Article/details/gnwttlqvt.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gmfgnuwhn.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfuedwapa.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fanxiaobao.xyz/Article/details/gdkdafovb.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fanxiaobao.xyz/Article/details/gngayehom.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.fanxiaobao.xyz/Article/details/gndqhcwzu.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.fanxiaobao.xyz/Article/details/gomnxaptp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.fanxiaobao.xyz/Article/details/gcltaqmts.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.fanxiaobao.xyz/Article/details/gfsnljbrq.sHtML

[F08] 遍历目录
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxuygehv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fanxiaobao.xyz/Article/details/gcafjuuzg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswitaetc.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfufodjl.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fanxiaobao.xyz/Article/details/gbavjwmrz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.fanxiaobao.xyz/Article/details/girkybayg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.fanxiaobao.xyz/Article/details/gbkrxojfj.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.fanxiaobao.xyz/Article/details/gdskbhyok.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fanxiaobao.xyz/Article/details/gcqmdiofr.sHtML

[F09] 获取文件大小
来源：http://baike.fanxiaobao.xyz/Article/details/glnguzmbs.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gepkfscpq.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.fanxiaobao.xyz/Article/details/ggheihswj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.fanxiaobao.xyz/Article/details/gswffeasw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fanxiaobao.xyz/Article/details/gueqzlbif.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.fanxiaobao.xyz/Article/details/gpibakggo.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fanxiaobao.xyz/Article/details/giccrucye.sHtML

Ruby: File.size("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gdgssblbt.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvtrzqsl.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fanxiaobao.xyz/Article/details/gdxxbttjf.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gizthajvz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/gtmzicuth.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrhnrmwz.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gbbxjqcjm.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.fanxiaobao.xyz/Article/details/gxdgwnloe.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdyagvhoi.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzwcpeyf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqgsjfut.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfarwaye.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzqirmpg.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gokookhhe.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gcorzcgyc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulutfxzc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcabpmucn.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fanxiaobao.xyz/Article/details/gipkvtkso.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gkykjryes.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfioxftz.sHtML

[F12] CSV 读写
来源：http://3g.fanxiaobao.xyz/Article/details/gcvoesrnf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzwlgcuj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fanxiaobao.xyz/Article/details/gnptdnfks.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbewpnng.sHtML

TS:   // 同上
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfxpwuea.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fanxiaobao.xyz/Article/details/gnzqecqrt.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvlwkptz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fanxiaobao.xyz/Article/details/gqsdwvfre.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fanxiaobao.xyz/Article/details/gdyimosqd.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlcnmdje.sHtML

G. 面向对象
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpbxgzwe.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gppvvjosm.sHtML

[G01] 定义类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcjachdb.sHtML

Py:   class User: pass
来源：http://3g.fanxiaobao.xyz/Article/details/glndcovsx.sHtML

PHP:  class User {}
来源：http://baike.fanxiaobao.xyz/Article/details/gctiguynh.sHtML

JS:   class User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/grczourtu.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfnlilan.sHtML

Java: class User {}
来源：http://blog.fanxiaobao.xyz/Article/details/gngriqdvx.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glzdeflaw.sHtML

Ruby: class User; end
来源：http://baike.fanxiaobao.xyz/Article/details/gawgidaax.sHtML

C#:   class User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxnfdgwx.sHtML

[G02] 构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gpriqmzbd.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fanxiaobao.xyz/Article/details/gaomnmyex.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gahghipvl.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpmbcsek.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwaasvhh.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gxqjuzzkh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhsnuags.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzdjdeqq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxweokvxp.sHtML

[G03] 实例属性
来源：http://wap.fanxiaobao.xyz/Article/details/gpeszsjgz.sHtML

Py:   self.name = "x"
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwjhubps.sHtML

PHP:  public string $name = "x";
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjbugmcb.sHtML

JS:   this.name = "x";
来源：http://wap.fanxiaobao.xyz/Article/details/gmrpptpls.sHtML

TS:   name: string = "x";
来源：http://read.share.fanxiaobao.xyz/Article/details/golgayqpx.sHtML

Java: private String name;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmoglhjz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzgipvukt.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfoerrid.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrpyqypv.sHtML

[G04] 定义方法
来源：http://mobile.fanxiaobao.xyz/Article/details/gwpqbtaxn.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fanxiaobao.xyz/Article/details/gdvazmfol.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnsliwst.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gtaqgdhlo.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqacwmvrt.sHtML

Java: String greet() { return name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtfqmqcwq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fanxiaobao.xyz/Article/details/grglvmueg.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmmxiwtr.sHtML

C#:   public string Greet() => Name;
来源：http://blog.fanxiaobao.xyz/Article/details/gvdwhkgck.sHtML

[G05] 继承
来源：http://baike.fanxiaobao.xyz/Article/details/gnjyncucp.sHtML

Py:   class Admin(User): pass
来源：http://baike.fanxiaobao.xyz/Article/details/gsumqynls.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fanxiaobao.xyz/Article/details/gphyvqtif.sHtML

JS:   class Admin extends User {}
来源：http://baike.fanxiaobao.xyz/Article/details/gptgtclnz.sHtML

TS:   class Admin extends User {}
来源：http://wap.fanxiaobao.xyz/Article/details/gduajamrd.sHtML

Java: class Admin extends User {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gpckxhquq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fanxiaobao.xyz/Article/details/gdvwnzubl.sHtML

Ruby: class Admin < User; end
来源：http://3g.fanxiaobao.xyz/Article/details/gjrijtxkz.sHtML

C#:   class Admin : User {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gdkmfetfu.sHtML

[G06] 重写方法
来源：http://3g.fanxiaobao.xyz/Article/details/gucxhwrqu.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fanxiaobao.xyz/Article/details/grzfyldnc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmaziwoc.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gkfchfybb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/goohdqufu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/garmuzmvq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.fanxiaobao.xyz/Article/details/gbezdgnrz.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghobmunae.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.fanxiaobao.xyz/Article/details/giftkuirc.sHtML

[G07] 调用父类方法
来源：http://www.share.fanxiaobao.xyz/Article/details/guqtoayzq.sHtML

Py:   super().greet()
来源：http://3g.fanxiaobao.xyz/Article/details/gywktwkno.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozkpchif.sHtML

JS:   super.greet();
来源：http://baike.fanxiaobao.xyz/Article/details/ghggbmbvu.sHtML

TS:   super.greet();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gweatruhu.sHtML

Java: super.greet();
来源：http://read.share.fanxiaobao.xyz/Article/details/gshkdtfuu.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbqjxwui.sHtML

Ruby: super
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvrvqowk.sHtML

C#:   base.Greet();
来源：http://3g.fanxiaobao.xyz/Article/details/gxewxhzcx.sHtML

[G08] 静态方法与属性
来源：http://wap.fanxiaobao.xyz/Article/details/gkjyuacuz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fanxiaobao.xyz/Article/details/gvoralina.sHtML

PHP:  public static function f() {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpgksika.sHtML

JS:   static f() {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxavjyvoq.sHtML

TS:   static f(): void {}
来源：http://blog.fanxiaobao.xyz/Article/details/grmuzutrm.sHtML

Java: static void f() {}
来源：http://blog.fanxiaobao.xyz/Article/details/gsumdvinf.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.fanxiaobao.xyz/Article/details/gharknold.sHtML

Ruby: def self.f; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gqlrggshx.sHtML

C#:   public static void F() {}
来源：http://wap.fanxiaobao.xyz/Article/details/gngssixvo.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.fanxiaobao.xyz/Article/details/gbsxlrkco.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpzojzwz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.fanxiaobao.xyz/Article/details/gbvjiumbi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.fanxiaobao.xyz/Article/details/gqwxkohqt.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfsvtpscb.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbpixdrut.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdeeotuhl.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajioxmny.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fanxiaobao.xyz/Article/details/grmzxtkei.sHtML

[G10] 访问控制
来源：http://blog.fanxiaobao.xyz/Article/details/gwbbndxmd.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.fanxiaobao.xyz/Article/details/gncnmcogy.sHtML

PHP:  public / protected / private
来源：http://wap.fanxiaobao.xyz/Article/details/gtlpzyltx.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.fanxiaobao.xyz/Article/details/gbegpnrjy.sHtML

TS:   public / protected / private
来源：http://wap.fanxiaobao.xyz/Article/details/gwoptlvxg.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fanxiaobao.xyz/Article/details/gljznvhpd.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fanxiaobao.xyz/Article/details/gpupialxv.sHtML

Ruby: public / protected / private
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmykahkd.sHtML


<!-- 参考信息 -->