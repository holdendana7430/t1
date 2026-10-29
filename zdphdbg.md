代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.fehbvm.com/Article/details/gyeoyrhpx.sHtML

[E11] 反转字符串
来源：http://www.blog.fehbvm.com/Article/details/gyxcvkhze.sHtML

Py:   s[::-1]
来源：http://wap.hesvh.cn/Article/details/gmgotytoe.sHtML

PHP:  strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/gkvqebyix.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gyljyxrgc.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gugthwbre.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.fehbvm.com/Article/details/gdxjjiqnu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.fehbvm.com/Article/details/gzcfzdhtb.sHtML

Ruby: s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gqvoywosf.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/gnhbdsghw.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.fehbvm.com/Article/details/gorgdptec.sHtML

Py:   s.count("a")
来源：http://blog.fehbvm.com/Article/details/gappilyvc.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.zdbjq.cn/Article/details/gahgwrdtz.sHtML

JS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/gmjkfrmua.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gdmtxgtlh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.fehbvm.com/Article/details/gwlnbpnuv.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.fehbvm.com/Article/details/gzsxsrqxb.sHtML

Ruby: s.count("a")
来源：http://3g.hesvh.cn/Article/details/gjixmabco.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.hesvh.cn/Article/details/gqgjoxqvb.sHtML

[E13] 逐字符遍历
来源：http://mobile.hesvh.cn/Article/details/gcyomcrwe.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.fehbvm.com/Article/details/gdkpmayse.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.fehbvm.com/Article/details/gfrrjtmdp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gnfrvuovx.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/ghgijzwhn.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.hesvh.cn/Article/details/gvymqrzvy.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.zdbjq.cn/Article/details/gxywwiphg.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.zdbjq.cn/Article/details/gwrsbtdqc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.zdbjq.cn/Article/details/ghpbjozzu.sHtML

[E14] URL 编码与 Base64
来源：http://baike.zdbjq.cn/Article/details/gevmbkjrv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.fehbvm.com/Article/details/gwzmxpkkx.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.hesvh.cn/Article/details/gnztnyocp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.fehbvm.com/Article/details/gqfxslvph.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.hesvh.cn/Article/details/gxcgfawus.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.hesvh.cn/Article/details/gbyghousr.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.fehbvm.com/Article/details/guqofrpwi.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.fehbvm.com/Article/details/gqgfbjmtm.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.fehbvm.com/Article/details/gzoddnmwq.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.fehbvm.com/Article/details/gzhnswxlo.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.hesvh.cn/Article/details/gtwjmqmlc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gyokohtzw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.zdbjq.cn/Article/details/ggwihjuyb.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.hesvh.cn/Article/details/geijhhmwc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.hesvh.cn/Article/details/gerpklzpp.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.fehbvm.com/Article/details/gjltxukkv.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.zdbjq.cn/Article/details/gxwagtqam.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.hesvh.cn/Article/details/gpxubjtih.sHtML

[E16] 数字千分位
来源：http://www.share.zdbjq.cn/Article/details/gjxqkknef.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.hesvh.cn/Article/details/gtodxnecr.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.hesvh.cn/Article/details/gohrxjumx.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/gzeorxgwf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/godigpubf.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.fehbvm.com/Article/details/gxptpxsqa.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.zdbjq.cn/Article/details/gccqnnxky.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.zdbjq.cn/Article/details/gperxfqik.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.fehbvm.com/Article/details/gbscvkwva.sHtML

[E17] 首字母大写
来源：http://wap.hesvh.cn/Article/details/gmpjtpxmz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.fehbvm.com/Article/details/goiygbnke.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.zdbjq.cn/Article/details/gyzprsnrq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/gzebwglxx.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.hesvh.cn/Article/details/gfxvltgki.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.fehbvm.com/Article/details/gsnwdiwky.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gjuizwyuo.sHtML

Ruby: s.capitalize
来源：http://www.m.share.fehbvm.com/Article/details/giylllqdb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.zdbjq.cn/Article/details/glrmifenm.sHtML

[E18] 模板占位符替换
来源：http://read.share.fehbvm.com/Article/details/gwumzjvdi.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.fehbvm.com/Article/details/gzjeuyqqb.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.hesvh.cn/Article/details/gfgcdbjum.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gohtdjzlq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gnselfyrd.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gsdrzirez.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gjyaqxrgd.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.hesvh.cn/Article/details/gsmscyvwk.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.zdbjq.cn/Article/details/gknfnlbma.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.hesvh.cn/Article/details/giutfptih.sHtML

Py:   s.splitlines()
来源：http://mobile.hesvh.cn/Article/details/giesmglxd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gloeumymn.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/girgopkeb.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gkzpblwfh.sHtML

Java: s.lines().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gtahnqbyu.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.fehbvm.com/Article/details/goijcrhjq.sHtML

Ruby: s.lines
来源：http://blog.zdbjq.cn/Article/details/gmklhqmzu.sHtML

C#:   s.Split('\n')
来源：http://www.share.fehbvm.com/Article/details/gzqvcpzri.sHtML

[E20] 判断字符串是否为空
来源：http://3g.zdbjq.cn/Article/details/gxnfpprfd.sHtML

Py:   if not s:
来源：http://www.share.hesvh.cn/Article/details/greudygvy.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.zdbjq.cn/Article/details/gjppuhtdi.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.fehbvm.com/Article/details/gwcggwvsu.sHtML

TS:   if (s === "") {}
来源：http://m.share.fehbvm.com/Article/details/gkyhtambl.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gxzkiiaio.sHtML

Go:   if s == "" {}
来源：http://wap.zdbjq.cn/Article/details/gztqchadg.sHtML

Ruby: if s.empty?
来源：http://www.share.zdbjq.cn/Article/details/gwaoxutkh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.hesvh.cn/Article/details/gkgkwouja.sHtML

[E21] 超长截断加省略号
来源：http://wap.zdbjq.cn/Article/details/gbqhazbxv.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.hesvh.cn/Article/details/gcvazsvkj.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gegjikfln.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gslqmnqkz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gemzkpiid.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/ggvnhotmf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.zdbjq.cn/Article/details/gtzxtscxk.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/gcdvtykab.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gdgddrcpg.sHtML

[E22] 字节长度与字符长度
来源：http://blog.hesvh.cn/Article/details/gvsahpdnv.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.zdbjq.cn/Article/details/gtyeqnmsj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gayachjdz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/ggrksjwgw.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gtnsbbqzn.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gebjvqnwt.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.hesvh.cn/Article/details/gkkngvjmw.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gjtcrytrv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gwbkwkkum.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gusihbbjh.sHtML

F. 文件与目录
来源：http://wap.zdbjq.cn/Article/details/gjeowiple.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gkxxajsji.sHtML

[F01] 读取整个文件
来源：http://www.share.hesvh.cn/Article/details/gbjcbfhmz.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.zdbjq.cn/Article/details/ggvnrruuu.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.fehbvm.com/Article/details/gknbhvvoo.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.hesvh.cn/Article/details/gfsbkypix.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gwtoutpjl.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gwqyicqrn.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.zdbjq.cn/Article/details/gcpprurob.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gkfkvzqww.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gteftbpxr.sHtML

[F02] 逐行读取文件
来源：http://3g.fehbvm.com/Article/details/gpzdlnenk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.zdbjq.cn/Article/details/gfceexkud.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.hesvh.cn/Article/details/gtyfbagys.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gpaspeiaq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/gjjomklwk.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gvvaxohhd.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.zdbjq.cn/Article/details/gilpwgknu.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.fehbvm.com/Article/details/gmnkwisae.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.hesvh.cn/Article/details/ggvpmbynm.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.hesvh.cn/Article/details/guwrcxivv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.hesvh.cn/Article/details/gdbewbvib.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gfssvgfap.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/ggrqatpsh.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gvgyamevx.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.fehbvm.com/Article/details/gutjlsiac.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fehbvm.com/Article/details/gamjexkmh.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.fehbvm.com/Article/details/ghnehuqml.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gwxkmfpki.sHtML

[F04] 追加写入文件
来源：http://www.m.share.fehbvm.com/Article/details/gjemdwfhp.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gpidliwqw.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.zdbjq.cn/Article/details/gcowdocat.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gbjfjnsmw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gutngvpok.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.fehbvm.com/Article/details/gaedjiwot.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.hesvh.cn/Article/details/gdatokurp.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.hesvh.cn/Article/details/guerbglln.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.zdbjq.cn/Article/details/gfaxhrnuc.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.zdbjq.cn/Article/details/gvyifqwsh.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.zdbjq.cn/Article/details/gnmkywseo.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.fehbvm.com/Article/details/gyfjhvqaw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gfocdvqnv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gwiynozec.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gnwduufvw.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.fehbvm.com/Article/details/gzqqcbhnx.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gvbovcuys.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gwnqahdmd.sHtML

[F06] 删除文件
来源：http://www.blog.fehbvm.com/Article/details/gvrtniznm.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gnmbntmay.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gbnangtyr.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gsundbxdt.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gznunubnm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gnqzqvgul.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gqhwtemab.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.fehbvm.com/Article/details/gkzxvbwyi.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gcldunshe.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.fehbvm.com/Article/details/gzmuwvpqg.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/gzqctitdj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.fehbvm.com/Article/details/gtxymzoce.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gmbbzjjar.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/gceucvdru.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.zdbjq.cn/Article/details/gqjozvpmc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fehbvm.com/Article/details/gosfvdlkr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.hesvh.cn/Article/details/gixqlqfdd.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.fehbvm.com/Article/details/gchgjxene.sHtML

[F08] 遍历目录
来源：http://blog.fehbvm.com/Article/details/grabpwbip.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.zdbjq.cn/Article/details/gnwxmptzk.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.fehbvm.com/Article/details/gjbdpjswz.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/gsjyfgyog.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/gsllqlhrz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gwcjwdsge.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.hesvh.cn/Article/details/grpkbbwcb.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gbzgtepyz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.zdbjq.cn/Article/details/gyselbpin.sHtML

[F09] 获取文件大小
来源：http://www.m.share.hesvh.cn/Article/details/gkvrfxpch.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gbbtujpbv.sHtML

PHP:  filesize("a.txt");
来源：http://blog.hesvh.cn/Article/details/ghtompzlc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/ggxpefwce.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gquguhamj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gfdetvbgu.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.zdbjq.cn/Article/details/gyxuznexc.sHtML

Ruby: File.size("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gkfhxephu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.zdbjq.cn/Article/details/gayohltcn.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.hesvh.cn/Article/details/ggerpiwbf.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/ghfnulmyb.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.zdbjq.cn/Article/details/gtlwhrhal.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gicnhwjjt.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gxccriedk.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.zdbjq.cn/Article/details/gyyrgwney.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gdibeetgn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/ghjrnrphy.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/geamshlwq.sHtML

[F11] 复制与移动文件
来源：http://blog.zdbjq.cn/Article/details/gwujecdet.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gjotwuzkd.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.hesvh.cn/Article/details/gixmgvwdj.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gudncfiay.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gtvlduplj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.hesvh.cn/Article/details/gkvyumsfn.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.hesvh.cn/Article/details/gftphagme.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gfibyqaoh.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.fehbvm.com/Article/details/gpbznkznc.sHtML

[F12] CSV 读写
来源：http://www.m.share.fehbvm.com/Article/details/gfoelxtqz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.fehbvm.com/Article/details/glfdxvlgv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fehbvm.com/Article/details/gblmslzja.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.hesvh.cn/Article/details/gdaqclhlk.sHtML

TS:   // 同上
来源：http://www.share.zdbjq.cn/Article/details/grkdtmnxt.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.hesvh.cn/Article/details/gmdydqcmx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.zdbjq.cn/Article/details/gkihqqvox.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.hesvh.cn/Article/details/ghrxzllrg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.hesvh.cn/Article/details/grrsirsca.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gkbeizoat.sHtML

G. 面向对象
来源：http://www.m.share.zdbjq.cn/Article/details/ghknzdsdb.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gobxrzave.sHtML

[G01] 定义类
来源：http://www.share.fehbvm.com/Article/details/gybamjmsn.sHtML

Py:   class User: pass
来源：http://mobile.hesvh.cn/Article/details/gdqeepksq.sHtML

PHP:  class User {}
来源：http://www.share.zdbjq.cn/Article/details/gaykdzurn.sHtML

JS:   class User {}
来源：http://blog.hesvh.cn/Article/details/gkjyaeehf.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.hesvh.cn/Article/details/ghaumygcy.sHtML

Java: class User {}
来源：http://m.share.hesvh.cn/Article/details/goharyvga.sHtML

Go:   type User struct { Name string }
来源：http://read.share.fehbvm.com/Article/details/gncqbycqu.sHtML

Ruby: class User; end
来源：http://www.share.fehbvm.com/Article/details/gatucnqlt.sHtML

C#:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gofwmkjad.sHtML

[G02] 构造函数
来源：http://baike.hesvh.cn/Article/details/gohfonveq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fehbvm.com/Article/details/gnpeaznek.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gopfauzkq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gpprqyhft.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.zdbjq.cn/Article/details/gsiulydbo.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gdgbrqhxj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.zdbjq.cn/Article/details/goltuvqfl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.zdbjq.cn/Article/details/gawtitibu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/grfaenpzj.sHtML

[G03] 实例属性
来源：http://wap.zdbjq.cn/Article/details/grlxzvaks.sHtML

Py:   self.name = "x"
来源：http://m.share.fehbvm.com/Article/details/getkoutdp.sHtML

PHP:  public string $name = "x";
来源：http://blog.hesvh.cn/Article/details/gvrkgsjjn.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gshycwnjc.sHtML

TS:   name: string = "x";
来源：http://mobile.fehbvm.com/Article/details/gldwcggwr.sHtML

Java: private String name;
来源：http://www.blog.zdbjq.cn/Article/details/gwlkzszhk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.fehbvm.com/Article/details/gtnzmucuc.sHtML

Ruby: @name = "x"
来源：http://3g.hesvh.cn/Article/details/ghabcxvpw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.hesvh.cn/Article/details/gaeccpxmj.sHtML

[G04] 定义方法
来源：http://baike.fehbvm.com/Article/details/gtdhodcym.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gxpwuswri.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gjjnrinzd.sHtML

JS:   greet() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/grzugdvly.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gcdjibdpt.sHtML

Java: String greet() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gqdbyjhgy.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/geudqbjup.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gdpxctmub.sHtML

C#:   public string Greet() => Name;
来源：http://baike.fehbvm.com/Article/details/grphmaqkt.sHtML

[G05] 继承
来源：http://www.blog.fehbvm.com/Article/details/gnitbqwjn.sHtML

Py:   class Admin(User): pass
来源：http://3g.hesvh.cn/Article/details/grsunrsvt.sHtML

PHP:  class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gdwjagiqi.sHtML

JS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gaahzkwvr.sHtML

TS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gufxjrmwp.sHtML

Java: class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gckurrptp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.zdbjq.cn/Article/details/gxvjcbqvv.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.fehbvm.com/Article/details/gaeecezsh.sHtML

C#:   class Admin : User {}
来源：http://blog.fehbvm.com/Article/details/gjxlziftr.sHtML

[G06] 重写方法
来源：http://www.blog.hesvh.cn/Article/details/gilpnycmb.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.fehbvm.com/Article/details/gwgicnhah.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gcjkfdldr.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gegiszsel.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gjtczaqsc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gvfadppft.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.zdbjq.cn/Article/details/gvffbqjje.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.zdbjq.cn/Article/details/gmvkrzfnd.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.zdbjq.cn/Article/details/gclkdvezi.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fehbvm.com/Article/details/guuvprmug.sHtML

Py:   super().greet()
来源：http://wap.hesvh.cn/Article/details/gzlarrkky.sHtML

PHP:  parent::greet();
来源：http://wap.hesvh.cn/Article/details/grtlujnhd.sHtML

JS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gojjiuayn.sHtML

TS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gryhynytp.sHtML

Java: super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gylgrisaj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.hesvh.cn/Article/details/gfvwbylrx.sHtML

Ruby: super
来源：http://blog.fehbvm.com/Article/details/gkbodjaop.sHtML

C#:   base.Greet();
来源：http://baike.zdbjq.cn/Article/details/gimjbugoq.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.hesvh.cn/Article/details/guhygqegf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.hesvh.cn/Article/details/gymytmfiv.sHtML

PHP:  public static function f() {}
来源：http://3g.fehbvm.com/Article/details/gvhfucagp.sHtML

JS:   static f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gbzfzzpqr.sHtML

TS:   static f(): void {}
来源：http://mobile.hesvh.cn/Article/details/grlfucgwj.sHtML

Java: static void f() {}
来源：http://mobile.fehbvm.com/Article/details/gchzupggf.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.fehbvm.com/Article/details/gihtirfhf.sHtML

Ruby: def self.f; end
来源：http://3g.fehbvm.com/Article/details/gfljybkcu.sHtML

C#:   public static void F() {}
来源：http://www.share.hesvh.cn/Article/details/gjvlannvf.sHtML

[G09] 接口 / 抽象类
来源：http://blog.hesvh.cn/Article/details/ghzcoabaz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.fehbvm.com/Article/details/gwqbbjjuf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.hesvh.cn/Article/details/gvrswkdbr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.zdbjq.cn/Article/details/gbhtjzcpr.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.fehbvm.com/Article/details/gevnvrpks.sHtML


<!-- 参考信息 -->