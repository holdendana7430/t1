代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gsasaiecr.sHtML

Java: String.format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gonuaadkk.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/guwttptnr.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gyjpuhiyv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.hesvh.cn/Article/details/gmzxmhubg.sHtML

[E11] 反转字符串
来源：http://3g.hesvh.cn/Article/details/goygyspnp.sHtML

Py:   s[::-1]
来源：http://baike.fehbvm.com/Article/details/gcazexjjb.sHtML

PHP:  strrev($s);
来源：http://wap.hesvh.cn/Article/details/gufsqaaxr.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gbwsskgzk.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gbefefflk.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.zdbjq.cn/Article/details/gimoiqbmu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.zdbjq.cn/Article/details/grborlicb.sHtML

Ruby: s.reverse
来源：http://m.share.hesvh.cn/Article/details/gybyurmnk.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/goyypzvjf.sHtML

[E12] 统计某字符出现次数
来源：http://wap.hesvh.cn/Article/details/gmpajbitg.sHtML

Py:   s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gnqipamyn.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.fehbvm.com/Article/details/gzezxtuuv.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/gpluvuziz.sHtML

TS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/gmdbyoeyi.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.hesvh.cn/Article/details/gnvxfpbxf.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.fehbvm.com/Article/details/ggrqqcfst.sHtML

Ruby: s.count("a")
来源：http://wap.hesvh.cn/Article/details/gecdjnwgz.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.zdbjq.cn/Article/details/ggeebixcr.sHtML

[E13] 逐字符遍历
来源：http://wap.zdbjq.cn/Article/details/ggickveed.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.fehbvm.com/Article/details/gyvwuawdz.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.zdbjq.cn/Article/details/gzirzxjtl.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/gnumddjvb.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/goqllqtfb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.zdbjq.cn/Article/details/gldipcnrk.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.fehbvm.com/Article/details/gtwhorpgl.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.zdbjq.cn/Article/details/ggiuxqhvg.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.hesvh.cn/Article/details/ggnubpxfn.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.fehbvm.com/Article/details/gpygwvtki.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fehbvm.com/Article/details/gxprqimit.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.hesvh.cn/Article/details/glvzetazy.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.zdbjq.cn/Article/details/gaeruopgk.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.hesvh.cn/Article/details/gtvwomcfo.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.fehbvm.com/Article/details/ghmmndeyh.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.zdbjq.cn/Article/details/gztqcdeze.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.zdbjq.cn/Article/details/gmzyvpxrs.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.zdbjq.cn/Article/details/glvfwqqhi.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.zdbjq.cn/Article/details/gsqkhqsps.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.hesvh.cn/Article/details/gvzhqwbpw.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.zdbjq.cn/Article/details/gkxohmgxz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.hesvh.cn/Article/details/gsxoqbllr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.fehbvm.com/Article/details/gtgtrrwqy.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.hesvh.cn/Article/details/ghwlcckqm.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.fehbvm.com/Article/details/gdwisbedi.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.fehbvm.com/Article/details/gihxqyfkm.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.zdbjq.cn/Article/details/gxatvfjqh.sHtML

[E16] 数字千分位
来源：http://m.share.fehbvm.com/Article/details/gmbctbexy.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.fehbvm.com/Article/details/gzuaztpbc.sHtML

PHP:  number_format(1234567);
来源：http://m.share.zdbjq.cn/Article/details/gfercjzvj.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gndeubrzh.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/gruulykbb.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.hesvh.cn/Article/details/grttxovlz.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.fehbvm.com/Article/details/gxrygmuwn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.zdbjq.cn/Article/details/gsuwrxdjq.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.zdbjq.cn/Article/details/grlmmczyj.sHtML

[E17] 首字母大写
来源：http://m.share.fehbvm.com/Article/details/ggjbpirpy.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.fehbvm.com/Article/details/geubgdsvl.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.hesvh.cn/Article/details/gqcvizhby.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gmbfwwaom.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/gyduhffqd.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.zdbjq.cn/Article/details/gvtrkczxp.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.zdbjq.cn/Article/details/gpepsdxtz.sHtML

Ruby: s.capitalize
来源：http://m.share.hesvh.cn/Article/details/ggrjtvcxd.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.zdbjq.cn/Article/details/ginbglceh.sHtML

[E18] 模板占位符替换
来源：http://blog.hesvh.cn/Article/details/gvkfotysx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fehbvm.com/Article/details/guvrjbryf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.hesvh.cn/Article/details/gqsvqtdki.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gofpawkts.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/glsymlwao.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/grkgzdhvh.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.zdbjq.cn/Article/details/greywphgz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.fehbvm.com/Article/details/goldnujdw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.fehbvm.com/Article/details/gzrdqcoiv.sHtML

[E19] 多行文本按行拆分
来源：http://3g.zdbjq.cn/Article/details/gbtwpqhuu.sHtML

Py:   s.splitlines()
来源：http://3g.hesvh.cn/Article/details/gbflynsgq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gzyrxsjwj.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/gaexpbylo.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gjgoepcmh.sHtML

Java: s.lines().toList()
来源：http://wap.hesvh.cn/Article/details/gglvyfrzi.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.hesvh.cn/Article/details/ggvozviag.sHtML

Ruby: s.lines
来源：http://www.blog.hesvh.cn/Article/details/gpxftghmu.sHtML

C#:   s.Split('\n')
来源：http://wap.hesvh.cn/Article/details/gaeffuwmp.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.zdbjq.cn/Article/details/gwoyfogfk.sHtML

Py:   if not s:
来源：http://wap.zdbjq.cn/Article/details/gqcpmvfia.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.fehbvm.com/Article/details/gsdetipbg.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.zdbjq.cn/Article/details/graygywrq.sHtML

TS:   if (s === "") {}
来源：http://baike.zdbjq.cn/Article/details/ggmvecnip.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/glecxuxpj.sHtML

Go:   if s == "" {}
来源：http://m.share.hesvh.cn/Article/details/gpfwvcjaw.sHtML

Ruby: if s.empty?
来源：http://baike.zdbjq.cn/Article/details/gpvtcymsn.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.zdbjq.cn/Article/details/gazrqqrgw.sHtML

[E21] 超长截断加省略号
来源：http://www.share.hesvh.cn/Article/details/gnilclkgh.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.hesvh.cn/Article/details/gyjtxtwwv.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gehxhioxq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gauiuumdp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gzvunilbo.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gpgygwayq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.zdbjq.cn/Article/details/gsgdpindq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/glonrfdsn.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gguoewjiy.sHtML

[E22] 字节长度与字符长度
来源：http://wap.zdbjq.cn/Article/details/geficnaxx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.hesvh.cn/Article/details/goyrnyvik.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gvuhorrxl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/gewqpmkcq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/gxrzqjigm.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.zdbjq.cn/Article/details/gzsjieduo.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.fehbvm.com/Article/details/gmtsnzkjh.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gmhkbmtyo.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gbiomquiw.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gnmrysrhz.sHtML

F. 文件与目录
来源：http://www.blog.fehbvm.com/Article/details/gkuzfuwws.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gpkkkxset.sHtML

[F01] 读取整个文件
来源：http://baike.hesvh.cn/Article/details/ggkiejrse.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.hesvh.cn/Article/details/gcryjysfp.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.hesvh.cn/Article/details/gvfvxyrhq.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.fehbvm.com/Article/details/ghhcrfalx.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.fehbvm.com/Article/details/gjusvcyef.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/guleluohs.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.zdbjq.cn/Article/details/ggzkahymh.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gjvqooxwf.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gqyyxybmi.sHtML

[F02] 逐行读取文件
来源：http://www.blog.fehbvm.com/Article/details/gejqizdih.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.hesvh.cn/Article/details/gjhcqhyds.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gxqfvetdo.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gqmqkuahe.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gqyefupjz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/ghpgaapyj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.fehbvm.com/Article/details/gduokldpr.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.fehbvm.com/Article/details/grcvgzntd.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.hesvh.cn/Article/details/gwcvetkcq.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.zdbjq.cn/Article/details/ghneknegu.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.fehbvm.com/Article/details/gcpxhbdlm.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gnbicaksz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gltxyjxbt.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gafdazodp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.hesvh.cn/Article/details/glgyjmkoa.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.zdbjq.cn/Article/details/guzppsphy.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.zdbjq.cn/Article/details/gqyqkcjdj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gsqgrtxfk.sHtML

[F04] 追加写入文件
来源：http://blog.fehbvm.com/Article/details/gdlcohtqu.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.hesvh.cn/Article/details/gavssccga.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.zdbjq.cn/Article/details/gejvxottq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gzvsfjoam.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gbbkbxgsy.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.zdbjq.cn/Article/details/gxcxxqqtt.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.zdbjq.cn/Article/details/ggbexanxp.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.zdbjq.cn/Article/details/gfcqpbgqb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.hesvh.cn/Article/details/gmqlebzct.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.hesvh.cn/Article/details/govciphwq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.hesvh.cn/Article/details/gljxfbssz.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fehbvm.com/Article/details/goxpcsqvl.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gassqunuo.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gcgqduzcv.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/grogshgml.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.hesvh.cn/Article/details/gniwqbymh.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gjqqxizlx.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.zdbjq.cn/Article/details/goyjocxrk.sHtML

[F06] 删除文件
来源：http://mobile.hesvh.cn/Article/details/grpxecqlp.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gvubdtbwm.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gdzdedrzw.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gwijwnfcd.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gqqlewyvb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gybtmefrk.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gkwdeuxym.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.fehbvm.com/Article/details/gwyuacpnt.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.fehbvm.com/Article/details/gxvugzqyu.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.hesvh.cn/Article/details/grwodpppl.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gankzkyrz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.fehbvm.com/Article/details/gqmcuykcq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gsepjzwbc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/gmxvrcdvg.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.hesvh.cn/Article/details/gjhrctavd.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.hesvh.cn/Article/details/gpgazcjsl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.hesvh.cn/Article/details/ggrdwmsuh.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.zdbjq.cn/Article/details/goahwoxww.sHtML

[F08] 遍历目录
来源：http://www.blog.fehbvm.com/Article/details/gyrxbbqpz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.zdbjq.cn/Article/details/glfotrtie.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fehbvm.com/Article/details/gafkemnlj.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/ghawxomxc.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gjbukuyfw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gmompmryp.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.fehbvm.com/Article/details/ggqztkdcx.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.zdbjq.cn/Article/details/gszxiykfz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.zdbjq.cn/Article/details/gjfnmrlev.sHtML

[F09] 获取文件大小
来源：http://m.share.fehbvm.com/Article/details/gsenkobfg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gpdtibite.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/ggspubmpe.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gwtkriliv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/grnndtmhb.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/giedeesfi.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.hesvh.cn/Article/details/gwdgjtylj.sHtML

Ruby: File.size("a.txt")
来源：http://wap.hesvh.cn/Article/details/geegijzpo.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.hesvh.cn/Article/details/gyxdulskx.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.hesvh.cn/Article/details/gjvemeiae.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gashktyeb.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.zdbjq.cn/Article/details/gwnvjwnzb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gtxrpdrjr.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gkekbxkuo.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.zdbjq.cn/Article/details/grtcjiwgx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gxcbkgdxl.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gpivpuxtt.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gdqllvjlg.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.zdbjq.cn/Article/details/gbyzrffdd.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gjqbmnjbb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.fehbvm.com/Article/details/giiqlmjfb.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gohmzvlip.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/grytyfquw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fehbvm.com/Article/details/glmxxhfag.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.hesvh.cn/Article/details/glaykrcqk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gvuutriem.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.zdbjq.cn/Article/details/gqnesjxql.sHtML

[F12] CSV 读写
来源：http://wap.hesvh.cn/Article/details/gblddtpxd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.zdbjq.cn/Article/details/gtsspdawe.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.hesvh.cn/Article/details/gqvgbwmht.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.hesvh.cn/Article/details/gmxvytntt.sHtML

TS:   // 同上
来源：http://www.share.zdbjq.cn/Article/details/gknjkauag.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.zdbjq.cn/Article/details/gsrwodysn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.zdbjq.cn/Article/details/gxlgqulbn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fehbvm.com/Article/details/gtnvmstkl.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.hesvh.cn/Article/details/gvgjzhjjw.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/growqhkrc.sHtML

G. 面向对象
来源：http://mobile.fehbvm.com/Article/details/gdbyawhcx.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/guejnwjjp.sHtML

[G01] 定义类
来源：http://wap.hesvh.cn/Article/details/geiiooafd.sHtML

Py:   class User: pass
来源：http://baike.fehbvm.com/Article/details/gapjqbfpr.sHtML

PHP:  class User {}
来源：http://blog.fehbvm.com/Article/details/ghnxpleqw.sHtML

JS:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwypjkluf.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.hesvh.cn/Article/details/gcalqkroi.sHtML

Java: class User {}
来源：http://mobile.zdbjq.cn/Article/details/gfwqczipe.sHtML

Go:   type User struct { Name string }
来源：http://www.share.zdbjq.cn/Article/details/gtissqzsa.sHtML

Ruby: class User; end
来源：http://blog.fehbvm.com/Article/details/gfxmtvogh.sHtML

C#:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gmyzbdlzc.sHtML

[G02] 构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gkvaksqtf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.hesvh.cn/Article/details/gtbgfrdcn.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.fehbvm.com/Article/details/gqvccyzui.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gnkzuydqc.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fehbvm.com/Article/details/gkhkgwnwb.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/gryyqznnp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.zdbjq.cn/Article/details/gcoutffzk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.hesvh.cn/Article/details/gpovpffxq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gabehafpb.sHtML

[G03] 实例属性
来源：http://www.m.share.zdbjq.cn/Article/details/gmcyacdbs.sHtML

Py:   self.name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gzqrwxyhx.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gpscrmkqy.sHtML

JS:   this.name = "x";
来源：http://mobile.fehbvm.com/Article/details/gkzauhwdr.sHtML

TS:   name: string = "x";
来源：http://www.blog.zdbjq.cn/Article/details/glkewxudh.sHtML

Java: private String name;
来源：http://www.m.share.fehbvm.com/Article/details/gpdiaofpx.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.hesvh.cn/Article/details/ghcaofpty.sHtML

Ruby: @name = "x"
来源：http://blog.fehbvm.com/Article/details/gkgcixbpu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.fehbvm.com/Article/details/gokdtmgyx.sHtML

[G04] 定义方法
来源：http://blog.fehbvm.com/Article/details/gkvjsbtuy.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/grtmxsnge.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gzyveyzsh.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gqyserdht.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gvjqiufaj.sHtML

Java: String greet() { return name; }
来源：http://3g.fehbvm.com/Article/details/gphyznvyd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gnlcmaapf.sHtML

Ruby: def greet; @name; end
来源：http://baike.zdbjq.cn/Article/details/gzvcbgvpt.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fehbvm.com/Article/details/grepuvvdd.sHtML

[G05] 继承
来源：http://baike.zdbjq.cn/Article/details/guoksihrg.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fehbvm.com/Article/details/gfuhlecxw.sHtML

PHP:  class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/giqhjmuuf.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbvhqxftr.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gvgibjcga.sHtML

Java: class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gmbzpmzdl.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fehbvm.com/Article/details/geicmnepk.sHtML

Ruby: class Admin < User; end
来源：http://wap.hesvh.cn/Article/details/gbyurheod.sHtML

C#:   class Admin : User {}
来源：http://blog.zdbjq.cn/Article/details/ggcvnhgnn.sHtML

[G06] 重写方法
来源：http://mobile.hesvh.cn/Article/details/gdmauxcpn.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.hesvh.cn/Article/details/gcgqkqnda.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/goplptnoh.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gqvhwwvkl.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gxysqxaxb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gqyhuagpi.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.hesvh.cn/Article/details/gmyxvmqjp.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.zdbjq.cn/Article/details/gqkdgyhmh.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.zdbjq.cn/Article/details/gldgvvuet.sHtML

[G07] 调用父类方法
来源：http://read.share.hesvh.cn/Article/details/gjdgrmutr.sHtML

Py:   super().greet()
来源：http://blog.fehbvm.com/Article/details/gjbvgityn.sHtML

PHP:  parent::greet();
来源：http://www.share.fehbvm.com/Article/details/gdftelplf.sHtML

JS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gwkshqqvg.sHtML

TS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gdokkjffo.sHtML

Java: super.greet();
来源：http://m.share.fehbvm.com/Article/details/gxmgfphos.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fehbvm.com/Article/details/gsktvhpuf.sHtML

Ruby: super
来源：http://m.share.zdbjq.cn/Article/details/gukjqhuya.sHtML

C#:   base.Greet();
来源：http://m.share.zdbjq.cn/Article/details/gmxzcmhik.sHtML

[G08] 静态方法与属性
来源：http://www.blog.hesvh.cn/Article/details/gxmskkoac.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.zdbjq.cn/Article/details/gxgflvgsj.sHtML

PHP:  public static function f() {}
来源：http://read.share.zdbjq.cn/Article/details/guxcxtllk.sHtML

JS:   static f() {}
来源：http://3g.zdbjq.cn/Article/details/gwplcjhfd.sHtML

TS:   static f(): void {}
来源：http://3g.zdbjq.cn/Article/details/gimwkyopb.sHtML

Java: static void f() {}
来源：http://www.blog.fehbvm.com/Article/details/gnbsnmien.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.hesvh.cn/Article/details/gjpnakgtj.sHtML

Ruby: def self.f; end
来源：http://mobile.hesvh.cn/Article/details/gmrmecvfw.sHtML

C#:   public static void F() {}
来源：http://mobile.hesvh.cn/Article/details/gvarjmsjg.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fehbvm.com/Article/details/gvclvyuwn.sHtML


<!-- 参考信息 -->