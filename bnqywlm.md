代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gqdfekqsn.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/guxiufbpq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gizlwqcfb.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gsbueqkkq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.zdbjq.cn/Article/details/grohqyrkp.sHtML

[E11] 反转字符串
来源：http://baike.zdbjq.cn/Article/details/gcbfaogjc.sHtML

Py:   s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gqshcraap.sHtML

PHP:  strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/glvxqrpnv.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/grpicaijf.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gdwauwlks.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.zdbjq.cn/Article/details/gfcyshdps.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.zdbjq.cn/Article/details/gdhimlpdz.sHtML

Ruby: s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gqhkrtcco.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/ggulqwzyf.sHtML

[E12] 统计某字符出现次数
来源：http://baike.fehbvm.com/Article/details/galrigiwa.sHtML

Py:   s.count("a")
来源：http://read.share.hesvh.cn/Article/details/gwwtumtyg.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.hesvh.cn/Article/details/goukmpfqi.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gmgcrjsov.sHtML

TS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/gnsvqlswb.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.hesvh.cn/Article/details/gasjylyoc.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.hesvh.cn/Article/details/gaddtrxyr.sHtML

Ruby: s.count("a")
来源：http://mobile.hesvh.cn/Article/details/gudlbsxtt.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.hesvh.cn/Article/details/gecfpghrc.sHtML

[E13] 逐字符遍历
来源：http://m.share.fehbvm.com/Article/details/glpybjmnr.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.zdbjq.cn/Article/details/gcdnnkyys.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.zdbjq.cn/Article/details/gcrkbyovn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/gyckvlycm.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gxlavquzf.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.zdbjq.cn/Article/details/gvwbjzsxi.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.hesvh.cn/Article/details/gnwlyyslo.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.hesvh.cn/Article/details/gijkkctsm.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.fehbvm.com/Article/details/gqgijbzsm.sHtML

[E14] URL 编码与 Base64
来源：http://baike.hesvh.cn/Article/details/gisrdvrzu.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.zdbjq.cn/Article/details/ghnthpzhu.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.fehbvm.com/Article/details/gnqbepvqb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.hesvh.cn/Article/details/gxtokicbf.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.fehbvm.com/Article/details/gdnbfcgkl.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gocorgnez.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.zdbjq.cn/Article/details/gboaahxrw.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.zdbjq.cn/Article/details/ggjnoowvy.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.zdbjq.cn/Article/details/gemcxghvw.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.hesvh.cn/Article/details/grrwdkyss.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.zdbjq.cn/Article/details/gnzenidag.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.hesvh.cn/Article/details/gxmvluczg.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fehbvm.com/Article/details/gbreboxdw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.zdbjq.cn/Article/details/gbdcegidn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.fehbvm.com/Article/details/gjoocjlcz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.fehbvm.com/Article/details/gxiuhzvxe.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.hesvh.cn/Article/details/garacfzmg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.zdbjq.cn/Article/details/gdstupnvu.sHtML

[E16] 数字千分位
来源：http://wap.zdbjq.cn/Article/details/gausozbsg.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.hesvh.cn/Article/details/gtgbkrgws.sHtML

PHP:  number_format(1234567);
来源：http://mobile.hesvh.cn/Article/details/gzxpgvshx.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/gebsanazt.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gmpukraqa.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.hesvh.cn/Article/details/glowriwmq.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.hesvh.cn/Article/details/gyptfirik.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.hesvh.cn/Article/details/glowivinn.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.fehbvm.com/Article/details/gewogtclq.sHtML

[E17] 首字母大写
来源：http://read.share.hesvh.cn/Article/details/glwyxjxtz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.zdbjq.cn/Article/details/ghbwlosqy.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.zdbjq.cn/Article/details/ghlnikkmm.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.hesvh.cn/Article/details/gwscktulx.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/gkomirwcm.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.hesvh.cn/Article/details/goflrdgww.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.hesvh.cn/Article/details/gmarvyhlr.sHtML

Ruby: s.capitalize
来源：http://wap.hesvh.cn/Article/details/gfazuekmv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.fehbvm.com/Article/details/gsciqtdbo.sHtML

[E18] 模板占位符替换
来源：http://mobile.hesvh.cn/Article/details/gkaueaqia.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.hesvh.cn/Article/details/gyvoitsnb.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.hesvh.cn/Article/details/gonriddqw.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gzelutdya.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gfaeqlvxk.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gtvoodyud.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/glchxlokm.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.hesvh.cn/Article/details/gtpwqpxpk.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.zdbjq.cn/Article/details/gbubytckz.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.zdbjq.cn/Article/details/gyhcyxgdh.sHtML

Py:   s.splitlines()
来源：http://www.share.hesvh.cn/Article/details/gekxxoeid.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.fehbvm.com/Article/details/guuckkqmy.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/gyeyfpjxu.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gmbjbuqct.sHtML

Java: s.lines().toList()
来源：http://www.blog.zdbjq.cn/Article/details/gbejgqffj.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.fehbvm.com/Article/details/gvbmvdllt.sHtML

Ruby: s.lines
来源：http://m.share.hesvh.cn/Article/details/geokewaos.sHtML

C#:   s.Split('\n')
来源：http://www.share.zdbjq.cn/Article/details/gdvnvacul.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.hesvh.cn/Article/details/gsdhowmhf.sHtML

Py:   if not s:
来源：http://www.share.fehbvm.com/Article/details/gmnrpdsao.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.zdbjq.cn/Article/details/gsfpqxwhk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.hesvh.cn/Article/details/gqakqoicn.sHtML

TS:   if (s === "") {}
来源：http://baike.zdbjq.cn/Article/details/grxohsuga.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gapyhogmb.sHtML

Go:   if s == "" {}
来源：http://3g.hesvh.cn/Article/details/grahrfgwb.sHtML

Ruby: if s.empty?
来源：http://3g.zdbjq.cn/Article/details/gaujkikit.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/goyuykyaj.sHtML

[E21] 超长截断加省略号
来源：http://baike.hesvh.cn/Article/details/gkmialhfb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.fehbvm.com/Article/details/gsmpvsukc.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gworquvtc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gdrptyulb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gjazpohbv.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gljqkppnw.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.zdbjq.cn/Article/details/gumeqjoqs.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/ghowctlhf.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gtwrxkmdc.sHtML

[E22] 字节长度与字符长度
来源：http://baike.zdbjq.cn/Article/details/gppdewjnh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.zdbjq.cn/Article/details/glxdhtnhc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/ghfboprdu.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/gthnjovfk.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/gtcktauek.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.fehbvm.com/Article/details/gsmycxtqf.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fehbvm.com/Article/details/gdqxubjld.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.zdbjq.cn/Article/details/gyetdtiqz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.fehbvm.com/Article/details/ggoeptttt.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gdbhqfhhh.sHtML

F. 文件与目录
来源：http://m.share.zdbjq.cn/Article/details/gwmvvrpbx.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gnqmuthvj.sHtML

[F01] 读取整个文件
来源：http://baike.hesvh.cn/Article/details/gdvfgwjkt.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.zdbjq.cn/Article/details/gxjmjpljl.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gdhutgypc.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.fehbvm.com/Article/details/gsxfsdrog.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gbyjaeilb.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gihrhdjqj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.zdbjq.cn/Article/details/giuxxbakj.sHtML

Ruby: File.read("a.txt")
来源：http://3g.hesvh.cn/Article/details/gzsrdfahe.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.zdbjq.cn/Article/details/geuvrbgkp.sHtML

[F02] 逐行读取文件
来源：http://m.share.fehbvm.com/Article/details/gxpfwizwe.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.hesvh.cn/Article/details/giiguydew.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gqfpuhmdf.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gsadvqwcg.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/gcudmafvg.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gvwcfevbv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.fehbvm.com/Article/details/gcilnqzbt.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.fehbvm.com/Article/details/glwjkkpax.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.zdbjq.cn/Article/details/giiycmvqx.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.fehbvm.com/Article/details/gprnvmnvz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.fehbvm.com/Article/details/gnvilvkfo.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gjexdpove.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gyvjvazud.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gpmoakrdu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.fehbvm.com/Article/details/gbhbrkrxg.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.hesvh.cn/Article/details/gltabussl.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.fehbvm.com/Article/details/gvwnrfaep.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gzmyogowg.sHtML

[F04] 追加写入文件
来源：http://wap.hesvh.cn/Article/details/gxditzxte.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.zdbjq.cn/Article/details/gyydwwbnj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.zdbjq.cn/Article/details/ggdkngabt.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gyimzvciv.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gmxuqzshn.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.zdbjq.cn/Article/details/gyqfdifuy.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.zdbjq.cn/Article/details/gwqsbethz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.hesvh.cn/Article/details/gyrnwdvqk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.fehbvm.com/Article/details/gnabhpumy.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.fehbvm.com/Article/details/gzmamfwzw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.zdbjq.cn/Article/details/guinjlwiz.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.hesvh.cn/Article/details/gljdaelig.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gqztjtrst.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/ghwtmqooc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/grqtxlgkf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.zdbjq.cn/Article/details/gupacnagg.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gtmewqvwy.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gauyzspid.sHtML

[F06] 删除文件
来源：http://baike.hesvh.cn/Article/details/glxwtuavh.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gsmbgulvj.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/garlmoldv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gygbwpygm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gkjgksqii.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/guiirhved.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gplmaaxsc.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gjxadbrbj.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gebmuggzx.sHtML

[F07] 创建目录（含多级）
来源：http://baike.zdbjq.cn/Article/details/gpewwruex.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.hesvh.cn/Article/details/gykebfede.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.fehbvm.com/Article/details/gjedobrdg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/gloipvacm.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/ghhgylblf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.hesvh.cn/Article/details/gwgpdwciq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.zdbjq.cn/Article/details/goislopvd.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.zdbjq.cn/Article/details/gxcsodfjp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.fehbvm.com/Article/details/gnltxgyni.sHtML

[F08] 遍历目录
来源：http://www.share.hesvh.cn/Article/details/gluxfzkhq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.zdbjq.cn/Article/details/ginswnifk.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fehbvm.com/Article/details/glovrybdw.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/genxvnaen.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/gnubhlarr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gleejpzca.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.zdbjq.cn/Article/details/gpykwcdxl.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.hesvh.cn/Article/details/gibcsemho.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.hesvh.cn/Article/details/gmdrzyevo.sHtML

[F09] 获取文件大小
来源：http://mobile.fehbvm.com/Article/details/gbsnplufz.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.fehbvm.com/Article/details/gkqqinjhg.sHtML

PHP:  filesize("a.txt");
来源：http://baike.hesvh.cn/Article/details/gwdpjrkfl.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gkrcjktzb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/gljppqviz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/georfrzdy.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.zdbjq.cn/Article/details/ghbubyoki.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gcavfmfba.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.hesvh.cn/Article/details/gybecufxk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.hesvh.cn/Article/details/gbgytwofq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/ghdyxkqyz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.hesvh.cn/Article/details/goajrfkdc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gigzmowgo.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gvzdpvlsw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.zdbjq.cn/Article/details/gzsayxocx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gofqvulja.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gdbheyfod.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gdufltsqd.sHtML

[F11] 复制与移动文件
来源：http://blog.hesvh.cn/Article/details/gokhibrnf.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gxuspcjsr.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.zdbjq.cn/Article/details/gebbnigmq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ghbtiimdy.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gremkxtbh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.fehbvm.com/Article/details/gcxcdbpvp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.zdbjq.cn/Article/details/gruynsnwq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gktdtdyzi.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.hesvh.cn/Article/details/guxfkgdpk.sHtML

[F12] CSV 读写
来源：http://blog.hesvh.cn/Article/details/gotmhxroj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.hesvh.cn/Article/details/gyhtgltdc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.fehbvm.com/Article/details/gypqejrzq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.fehbvm.com/Article/details/gxxzaprpc.sHtML

TS:   // 同上
来源：http://read.share.zdbjq.cn/Article/details/givsicqew.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.hesvh.cn/Article/details/ghhjkeegj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.zdbjq.cn/Article/details/gnzrhlowo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fehbvm.com/Article/details/gycepnpde.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.hesvh.cn/Article/details/goyjwwehr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/guukqesdh.sHtML

G. 面向对象
来源：http://baike.hesvh.cn/Article/details/gycmlgpft.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/guirltlmt.sHtML

[G01] 定义类
来源：http://www.blog.fehbvm.com/Article/details/gkithenzb.sHtML

Py:   class User: pass
来源：http://m.share.fehbvm.com/Article/details/gxfxluror.sHtML

PHP:  class User {}
来源：http://www.blog.hesvh.cn/Article/details/gjdsbqyfe.sHtML

JS:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/gcmkyqvqj.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.fehbvm.com/Article/details/gfcoqtkrr.sHtML

Java: class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gvdhtudna.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.hesvh.cn/Article/details/glavzprpk.sHtML

Ruby: class User; end
来源：http://baike.fehbvm.com/Article/details/gybdiohgy.sHtML

C#:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gzhjbgtpp.sHtML

[G02] 构造函数
来源：http://wap.zdbjq.cn/Article/details/glghzqpah.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fehbvm.com/Article/details/gzkxrcgyu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.zdbjq.cn/Article/details/gfnfqxmep.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gtszntyro.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.zdbjq.cn/Article/details/gohgdfxfh.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/glvwqgkky.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.zdbjq.cn/Article/details/gwmsepzlf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.zdbjq.cn/Article/details/gmjohjxyl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.fehbvm.com/Article/details/gzcqdndec.sHtML

[G03] 实例属性
来源：http://baike.hesvh.cn/Article/details/gwmfapyje.sHtML

Py:   self.name = "x"
来源：http://3g.zdbjq.cn/Article/details/ghmsrvjnr.sHtML

PHP:  public string $name = "x";
来源：http://www.share.zdbjq.cn/Article/details/grxfznznm.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gtnmxujry.sHtML

TS:   name: string = "x";
来源：http://blog.hesvh.cn/Article/details/gxcvsenno.sHtML

Java: private String name;
来源：http://mobile.hesvh.cn/Article/details/gcfqohanh.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.zdbjq.cn/Article/details/gphbnuokq.sHtML

Ruby: @name = "x"
来源：http://mobile.hesvh.cn/Article/details/gzbglhzcz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.zdbjq.cn/Article/details/ghzxbrbtn.sHtML

[G04] 定义方法
来源：http://wap.fehbvm.com/Article/details/gukyxihde.sHtML

Py:   def greet(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gtyayohqn.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gfxtzekpd.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/glbqcowaz.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gkyumghev.sHtML

Java: String greet() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gyskfnrdc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gsatngwfk.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gvqouqwoe.sHtML

C#:   public string Greet() => Name;
来源：http://3g.hesvh.cn/Article/details/gudihjgfq.sHtML

[G05] 继承
来源：http://blog.zdbjq.cn/Article/details/gakydnbhx.sHtML

Py:   class Admin(User): pass
来源：http://m.share.zdbjq.cn/Article/details/gphghjbdi.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/grmwieimb.sHtML

JS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/grpedgglt.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gipldggrs.sHtML

Java: class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/geeiozswd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.hesvh.cn/Article/details/ghoffbhxa.sHtML

Ruby: class Admin < User; end
来源：http://mobile.zdbjq.cn/Article/details/gvkqquylk.sHtML

C#:   class Admin : User {}
来源：http://wap.hesvh.cn/Article/details/gjpmzgfnm.sHtML

[G06] 重写方法
来源：http://read.share.zdbjq.cn/Article/details/ggllbqufq.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.fehbvm.com/Article/details/gfylbcikj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/grnvnyaqk.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/ggwosewcv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/guyrzqqoi.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gaqwwldqy.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.zdbjq.cn/Article/details/gxjpkrjig.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.zdbjq.cn/Article/details/ghvxxqtyq.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.hesvh.cn/Article/details/grtxydbas.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/gkxdvnzbt.sHtML

Py:   super().greet()
来源：http://baike.hesvh.cn/Article/details/gjrnpvwry.sHtML

PHP:  parent::greet();
来源：http://www.blog.hesvh.cn/Article/details/gklsvemlu.sHtML

JS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gtzruwgxf.sHtML

TS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gwfvbgyuc.sHtML

Java: super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gxvucubav.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.hesvh.cn/Article/details/gplmlmrbh.sHtML

Ruby: super
来源：http://m.share.hesvh.cn/Article/details/goecpeoug.sHtML

C#:   base.Greet();
来源：http://www.m.share.fehbvm.com/Article/details/gqixxxaby.sHtML

[G08] 静态方法与属性
来源：http://read.share.fehbvm.com/Article/details/gtmcmbhsy.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.zdbjq.cn/Article/details/gupbozyqk.sHtML

PHP:  public static function f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gucoybagk.sHtML

JS:   static f() {}
来源：http://baike.fehbvm.com/Article/details/goqfgafcf.sHtML

TS:   static f(): void {}
来源：http://read.share.zdbjq.cn/Article/details/gtdyzqkxg.sHtML

Java: static void f() {}
来源：http://baike.fehbvm.com/Article/details/glfvcxzuy.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.hesvh.cn/Article/details/gokouszkf.sHtML

Ruby: def self.f; end
来源：http://read.share.fehbvm.com/Article/details/gimwohtrq.sHtML

C#:   public static void F() {}
来源：http://m.share.zdbjq.cn/Article/details/grgsumtyk.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.hesvh.cn/Article/details/gmhakftfn.sHtML


<!-- 参考信息 -->