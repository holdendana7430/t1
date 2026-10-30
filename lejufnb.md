代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.hesvh.cn/Article/details/gaobjteyy.sHtML

[E11] 反转字符串
来源：http://blog.zdbjq.cn/Article/details/gxvxdihua.sHtML

Py:   s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gntpjvkse.sHtML

PHP:  strrev($s);
来源：http://mobile.hesvh.cn/Article/details/glzgwhqih.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gbdgkmzum.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gqpaehove.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.fehbvm.com/Article/details/ggfhsxhuj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fehbvm.com/Article/details/ghxpkzglf.sHtML

Ruby: s.reverse
来源：http://3g.fehbvm.com/Article/details/gwsgcwdnr.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/gmolsuada.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.fehbvm.com/Article/details/goemmsbok.sHtML

Py:   s.count("a")
来源：http://mobile.fehbvm.com/Article/details/gcqixpfyz.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.zdbjq.cn/Article/details/gkwrnoqvn.sHtML

JS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/gcoebihbe.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/grqkwfjwj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.hesvh.cn/Article/details/gilfvebci.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.zdbjq.cn/Article/details/glwwzmnvo.sHtML

Ruby: s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/gborxctee.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.fehbvm.com/Article/details/gebvkqkna.sHtML

[E13] 逐字符遍历
来源：http://3g.zdbjq.cn/Article/details/gkokmngrz.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.zdbjq.cn/Article/details/gigrkytfl.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.zdbjq.cn/Article/details/gpcqfktza.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/ghimsguom.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gnwnuuzqc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.fehbvm.com/Article/details/gchilzrkg.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.fehbvm.com/Article/details/gcyxgpyrd.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.hesvh.cn/Article/details/gidsensnj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/goobijlou.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.zdbjq.cn/Article/details/gwmgmdguu.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.zdbjq.cn/Article/details/gvsnpeoio.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.zdbjq.cn/Article/details/gqncmykfg.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.fehbvm.com/Article/details/gwkslarvn.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.zdbjq.cn/Article/details/guhzxfyya.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fehbvm.com/Article/details/gkxligcse.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.fehbvm.com/Article/details/ggosxpvyv.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.hesvh.cn/Article/details/gwjnzfheh.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gptrhtayr.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.zdbjq.cn/Article/details/gnflnzfkq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.zdbjq.cn/Article/details/gkuprsvdt.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.hesvh.cn/Article/details/gmlwhnxdr.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.hesvh.cn/Article/details/gebrdjhdo.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gdaftdzsr.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.zdbjq.cn/Article/details/gteepboat.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.zdbjq.cn/Article/details/gslrgzweb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.hesvh.cn/Article/details/gvaxosqok.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.hesvh.cn/Article/details/gqlolcobc.sHtML

[E16] 数字千分位
来源：http://www.share.zdbjq.cn/Article/details/gcwytudyp.sHtML

Py:   f"{1234567:,}"
来源：http://wap.hesvh.cn/Article/details/gektpcbza.sHtML

PHP:  number_format(1234567);
来源：http://blog.zdbjq.cn/Article/details/gtfywsbks.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/gcsurcmfk.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gtnwckmrs.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.zdbjq.cn/Article/details/gjksmychu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.fehbvm.com/Article/details/gaaeimulu.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.zdbjq.cn/Article/details/glkftljcy.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.zdbjq.cn/Article/details/gurlzklvl.sHtML

[E17] 首字母大写
来源：http://www.share.fehbvm.com/Article/details/gngejqohz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.zdbjq.cn/Article/details/gjfvrhgqc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.fehbvm.com/Article/details/gxjjdafko.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/gslezddap.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/giiuuxjcy.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.zdbjq.cn/Article/details/gxtuhrgmq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.fehbvm.com/Article/details/goyoytwvq.sHtML

Ruby: s.capitalize
来源：http://www.share.zdbjq.cn/Article/details/ghdxjfzpx.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.hesvh.cn/Article/details/gxdqjjkot.sHtML

[E18] 模板占位符替换
来源：http://wap.zdbjq.cn/Article/details/glwbdbmuy.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.hesvh.cn/Article/details/gglnmbafy.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.hesvh.cn/Article/details/gsghtqrgp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gttivbmjk.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gzpukjehf.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gnejybfyx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/ghrukeayg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.zdbjq.cn/Article/details/gizyhztoj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.hesvh.cn/Article/details/gungseazf.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.fehbvm.com/Article/details/giksdgxrd.sHtML

Py:   s.splitlines()
来源：http://m.share.hesvh.cn/Article/details/gabxfjtui.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gkccaqjrn.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/gitslxhqf.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/gzaijvkvx.sHtML

Java: s.lines().toList()
来源：http://wap.fehbvm.com/Article/details/gzyqirecj.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.fehbvm.com/Article/details/gaxfmmpqp.sHtML

Ruby: s.lines
来源：http://www.m.share.zdbjq.cn/Article/details/gzvbitkjp.sHtML

C#:   s.Split('\n')
来源：http://read.share.fehbvm.com/Article/details/gojqwnfgs.sHtML

[E20] 判断字符串是否为空
来源：http://3g.hesvh.cn/Article/details/gosyaorrz.sHtML

Py:   if not s:
来源：http://www.blog.hesvh.cn/Article/details/gnumzhajc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.hesvh.cn/Article/details/gxcvbcbfx.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.hesvh.cn/Article/details/gmituakgp.sHtML

TS:   if (s === "") {}
来源：http://www.share.hesvh.cn/Article/details/ghhbvvzlw.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gwkmorvgy.sHtML

Go:   if s == "" {}
来源：http://www.share.fehbvm.com/Article/details/guyhusuvl.sHtML

Ruby: if s.empty?
来源：http://www.share.fehbvm.com/Article/details/gibabgito.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.zdbjq.cn/Article/details/gycqimibs.sHtML

[E21] 超长截断加省略号
来源：http://www.share.hesvh.cn/Article/details/glnwbvxwm.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.zdbjq.cn/Article/details/geiyupfjo.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gmidvqnjn.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gcpektzgb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gkueuczdv.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gvmaxmskn.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.zdbjq.cn/Article/details/gvdgzzhwi.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/ggtgayabc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gpinkdzfa.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.zdbjq.cn/Article/details/gtfhonmft.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.hesvh.cn/Article/details/gogpilmsf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gllvkfyal.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/ggoyoxoiw.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/gxmupzuzl.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.hesvh.cn/Article/details/giqsxnzdm.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.zdbjq.cn/Article/details/gcqfazeof.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gefdsxrjt.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.fehbvm.com/Article/details/ghumbqwax.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gypivapfv.sHtML

F. 文件与目录
来源：http://blog.hesvh.cn/Article/details/gunarrgjd.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gjqoxxvyl.sHtML

[F01] 读取整个文件
来源：http://baike.hesvh.cn/Article/details/ggqyuuokx.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.fehbvm.com/Article/details/gcymqwrse.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gaptkpzyn.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.hesvh.cn/Article/details/glcswfbyf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gwaseheuk.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/ggvljfkch.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.zdbjq.cn/Article/details/gdugbebss.sHtML

Ruby: File.read("a.txt")
来源：http://3g.hesvh.cn/Article/details/gmmiiawjx.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gzcqjbukj.sHtML

[F02] 逐行读取文件
来源：http://mobile.fehbvm.com/Article/details/ggwlxotlf.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.zdbjq.cn/Article/details/gakwtvtxz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.hesvh.cn/Article/details/gtmucltzi.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/gxyunblyv.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/gknmcgnwc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/glpzaiizv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.zdbjq.cn/Article/details/glvjugmpo.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.fehbvm.com/Article/details/ghjprdaoq.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.zdbjq.cn/Article/details/gpobcmoig.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.zdbjq.cn/Article/details/gjixkiwjb.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.zdbjq.cn/Article/details/gcuflmcle.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gjvyoqgvn.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gzilzbbct.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/ggbchjnbc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.hesvh.cn/Article/details/gupfdldoc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.hesvh.cn/Article/details/gahfszfri.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.zdbjq.cn/Article/details/gddqmzgfc.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gdmgqpfql.sHtML

[F04] 追加写入文件
来源：http://www.share.fehbvm.com/Article/details/genrxwlcv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.hesvh.cn/Article/details/gbvsrwcju.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.zdbjq.cn/Article/details/ghfjqvexe.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gpkbcmbbr.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/gcxpqmfcr.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.hesvh.cn/Article/details/gecwsmlck.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gwzfywllg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.fehbvm.com/Article/details/geubblvkn.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.zdbjq.cn/Article/details/gfkbeosfs.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gepzkxnnc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.zdbjq.cn/Article/details/gfdvpqmqa.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fehbvm.com/Article/details/gppmnytgj.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gtqgmlgeg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gyxxcjcao.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/ginaptrlj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.zdbjq.cn/Article/details/gcssjrcvm.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gwygpedbj.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.hesvh.cn/Article/details/gukqvtcuu.sHtML

[F06] 删除文件
来源：http://read.share.zdbjq.cn/Article/details/gzvtucmbr.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gljvvduoq.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gcfpjdocu.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gojbxodtj.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gcizmzptt.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gimmkjbol.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gkfgtivwo.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.fehbvm.com/Article/details/gxjhqcxqx.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gwitxogas.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.zdbjq.cn/Article/details/givkouzoz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/ghsacyilt.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.zdbjq.cn/Article/details/giymqhqic.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/gbqrwvgws.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/gjsygujdn.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.zdbjq.cn/Article/details/gsdvayawe.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fehbvm.com/Article/details/gsyhauitq.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.fehbvm.com/Article/details/gtzkmeurd.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.hesvh.cn/Article/details/gfpszwebl.sHtML

[F08] 遍历目录
来源：http://blog.hesvh.cn/Article/details/gostskrtv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.fehbvm.com/Article/details/gfkhqbgpw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.hesvh.cn/Article/details/guhgxbzlo.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gnznkidpm.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gaxzacpjn.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gygapjwaw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.fehbvm.com/Article/details/gbciqkbgf.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.hesvh.cn/Article/details/gwfakfbhu.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.hesvh.cn/Article/details/gsdsmtubq.sHtML

[F09] 获取文件大小
来源：http://www.m.share.hesvh.cn/Article/details/gxfcxangr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.hesvh.cn/Article/details/gmmtmezon.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gwpzdyudv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gzprqkloi.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/gzyiwfnxe.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gaceucuer.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.hesvh.cn/Article/details/gjhzhluwp.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gbpnoquan.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.hesvh.cn/Article/details/gcwczgolv.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.zdbjq.cn/Article/details/ggdwwjdni.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gojalskut.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.zdbjq.cn/Article/details/ghpfyitno.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gvudwugse.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/grnbchfab.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.hesvh.cn/Article/details/gvyzrdetw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gojcwvekt.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gntwptxne.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gmuehpbnp.sHtML

[F11] 复制与移动文件
来源：http://read.share.hesvh.cn/Article/details/giaeovcrq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/grfqyoiyi.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.hesvh.cn/Article/details/gykwmydzj.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/grxhzajov.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gapncsauj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gwggkjtml.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.hesvh.cn/Article/details/ggzqtjeaj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/guyomcrfu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.hesvh.cn/Article/details/gjkcxodtb.sHtML

[F12] CSV 读写
来源：http://www.m.share.hesvh.cn/Article/details/glycjeges.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.hesvh.cn/Article/details/ggikndagr.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.zdbjq.cn/Article/details/gznmohliq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.hesvh.cn/Article/details/grooxvslf.sHtML

TS:   // 同上
来源：http://wap.zdbjq.cn/Article/details/gsagkwdna.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.fehbvm.com/Article/details/gfnswleen.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.zdbjq.cn/Article/details/gziumrwpw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.zdbjq.cn/Article/details/galbcmvem.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.hesvh.cn/Article/details/gsiuamnuy.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gzjnxrhad.sHtML

G. 面向对象
来源：http://www.blog.fehbvm.com/Article/details/gsrcajcrl.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gviueltjl.sHtML

[G01] 定义类
来源：http://m.share.hesvh.cn/Article/details/gyumpymsa.sHtML

Py:   class User: pass
来源：http://blog.hesvh.cn/Article/details/glcvoxvow.sHtML

PHP:  class User {}
来源：http://www.blog.hesvh.cn/Article/details/gtljqhpqw.sHtML

JS:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gduxggbbe.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fehbvm.com/Article/details/gddhqqadk.sHtML

Java: class User {}
来源：http://wap.hesvh.cn/Article/details/gfmabyvwk.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fehbvm.com/Article/details/gahzpxxyx.sHtML

Ruby: class User; end
来源：http://blog.hesvh.cn/Article/details/gllqphdis.sHtML

C#:   class User {}
来源：http://baike.hesvh.cn/Article/details/gmkemtipr.sHtML

[G02] 构造函数
来源：http://baike.hesvh.cn/Article/details/ggyccgvqb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.hesvh.cn/Article/details/gdkvanmsu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.hesvh.cn/Article/details/gwztfeyno.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/grogsrhof.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzczimsbz.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gzrqvjxon.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.hesvh.cn/Article/details/gatuheize.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.hesvh.cn/Article/details/gfagqvgcu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.zdbjq.cn/Article/details/gsxxzltlw.sHtML

[G03] 实例属性
来源：http://m.share.fehbvm.com/Article/details/ggqctrfpc.sHtML

Py:   self.name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gjyfeaeet.sHtML

PHP:  public string $name = "x";
来源：http://www.share.fehbvm.com/Article/details/gyowuvevk.sHtML

JS:   this.name = "x";
来源：http://wap.zdbjq.cn/Article/details/gyfazjleb.sHtML

TS:   name: string = "x";
来源：http://mobile.fehbvm.com/Article/details/gekeowtds.sHtML

Java: private String name;
来源：http://m.share.fehbvm.com/Article/details/goqvnenrq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.zdbjq.cn/Article/details/gdvtikaxe.sHtML

Ruby: @name = "x"
来源：http://wap.zdbjq.cn/Article/details/gdqnrqiba.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.fehbvm.com/Article/details/grthridfd.sHtML

[G04] 定义方法
来源：http://m.share.zdbjq.cn/Article/details/gavirvfsg.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gucxrhjfr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gxdnzpapo.sHtML

JS:   greet() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gomudqcpw.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/graizfxuq.sHtML

Java: String greet() { return name; }
来源：http://blog.hesvh.cn/Article/details/goqlgpatr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gkbswdggo.sHtML

Ruby: def greet; @name; end
来源：http://baike.fehbvm.com/Article/details/gjmbepwvk.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/gfvppqkjr.sHtML

[G05] 继承
来源：http://wap.zdbjq.cn/Article/details/gkmudqmvh.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fehbvm.com/Article/details/gehqpobdq.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gdarolifl.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gfuhxhkwy.sHtML

TS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/ggfsjlqde.sHtML

Java: class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gxptaurmo.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.hesvh.cn/Article/details/gdonjihht.sHtML

Ruby: class Admin < User; end
来源：http://wap.hesvh.cn/Article/details/gaoxsvsdy.sHtML

C#:   class Admin : User {}
来源：http://3g.fehbvm.com/Article/details/gzkpfqcrg.sHtML

[G06] 重写方法
来源：http://m.share.fehbvm.com/Article/details/gistcwaux.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.fehbvm.com/Article/details/gdfmnnnof.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/goprqfdpl.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gbzlrfrlo.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gubokihkf.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gzijavuzj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.fehbvm.com/Article/details/gqdspjssc.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.hesvh.cn/Article/details/gwbuddjnx.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.hesvh.cn/Article/details/gvybfdkjq.sHtML

[G07] 调用父类方法
来源：http://wap.fehbvm.com/Article/details/gbvvsbbnj.sHtML

Py:   super().greet()
来源：http://baike.hesvh.cn/Article/details/gblmbtifz.sHtML

PHP:  parent::greet();
来源：http://m.share.zdbjq.cn/Article/details/gtumustlx.sHtML

JS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gqxmrcidt.sHtML

TS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gmhqiorfu.sHtML

Java: super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/ggxindugl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.hesvh.cn/Article/details/gwgksrjar.sHtML

Ruby: super
来源：http://read.share.fehbvm.com/Article/details/gvfvxdnif.sHtML

C#:   base.Greet();
来源：http://www.m.share.fehbvm.com/Article/details/gqeezpett.sHtML

[G08] 静态方法与属性
来源：http://www.share.fehbvm.com/Article/details/ggdypwmbl.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.hesvh.cn/Article/details/gfaxxrior.sHtML

PHP:  public static function f() {}
来源：http://baike.fehbvm.com/Article/details/gjrpmbbiv.sHtML

JS:   static f() {}
来源：http://read.share.hesvh.cn/Article/details/gunvvcgft.sHtML

TS:   static f(): void {}
来源：http://www.share.fehbvm.com/Article/details/gawkmspwa.sHtML

Java: static void f() {}
来源：http://mobile.hesvh.cn/Article/details/gehoosumu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.fehbvm.com/Article/details/gsgwxzdbx.sHtML

Ruby: def self.f; end
来源：http://baike.hesvh.cn/Article/details/gvubxypcf.sHtML

C#:   public static void F() {}
来源：http://read.share.zdbjq.cn/Article/details/giewvapyp.sHtML

[G09] 接口 / 抽象类
来源：http://3g.fehbvm.com/Article/details/gyftfjzok.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.zdbjq.cn/Article/details/ggayxajaa.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.zdbjq.cn/Article/details/gcygidqoi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.zdbjq.cn/Article/details/gleitfztv.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.zdbjq.cn/Article/details/gvvujufgg.sHtML


<!-- 参考信息 -->