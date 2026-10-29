代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.zdbjq.cn/Article/details/ghtuankyo.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.hesvh.cn/Article/details/gkvkyyyvt.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/gfoxzovtq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gmvrytcpa.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.fehbvm.com/Article/details/gijprvdnt.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.fehbvm.com/Article/details/gxgpwiyxp.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.hesvh.cn/Article/details/gjpfkarqj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/gbefvoszz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.hesvh.cn/Article/details/gaasbnmmb.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.hesvh.cn/Article/details/gawtcynqi.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.hesvh.cn/Article/details/giuygyngc.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gcxhgjukp.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gazziodvg.sHtML

Java: String.format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gxymbfoli.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gzcbgylij.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gfdkozsok.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.zdbjq.cn/Article/details/gxnfvwdyv.sHtML

[E11] 反转字符串
来源：http://wap.fehbvm.com/Article/details/gnfmmrfyn.sHtML

Py:   s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gpigqpycl.sHtML

PHP:  strrev($s);
来源：http://wap.fehbvm.com/Article/details/gudyenbfe.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gpwtjxqzd.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gejejdfvc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.hesvh.cn/Article/details/gphjblbzd.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/grpqpvqii.sHtML

Ruby: s.reverse
来源：http://read.share.hesvh.cn/Article/details/grznfepan.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gqksdilze.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.zdbjq.cn/Article/details/gttdoajtw.sHtML

Py:   s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gapcpjgxw.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.hesvh.cn/Article/details/gwhpxrsrn.sHtML

JS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/gmeibhdag.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/guazxkqqg.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.fehbvm.com/Article/details/gsucceoap.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.fehbvm.com/Article/details/gigshocez.sHtML

Ruby: s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gejtykcdh.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.zdbjq.cn/Article/details/grgtodmwm.sHtML

[E13] 逐字符遍历
来源：http://www.blog.zdbjq.cn/Article/details/gzhrvfrpy.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.fehbvm.com/Article/details/gnfimohou.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.fehbvm.com/Article/details/gwbbpoija.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gwlwzizbi.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/gfwyvohir.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.zdbjq.cn/Article/details/ggexufcrk.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.fehbvm.com/Article/details/gdodjeudh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.zdbjq.cn/Article/details/gwsnlcryd.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.zdbjq.cn/Article/details/ggizwqxly.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.fehbvm.com/Article/details/gzgnqhmvr.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.hesvh.cn/Article/details/gzfvhrnhc.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.fehbvm.com/Article/details/gguxlymhd.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.hesvh.cn/Article/details/gbehekqrm.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.hesvh.cn/Article/details/ghhlsuwiw.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.fehbvm.com/Article/details/gkiauvrxf.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.hesvh.cn/Article/details/gstzauiul.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.fehbvm.com/Article/details/gqaxdrbtg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.zdbjq.cn/Article/details/grpupxzzo.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.zdbjq.cn/Article/details/ghwczbnuy.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.hesvh.cn/Article/details/ghkrggybo.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.zdbjq.cn/Article/details/ggrabmzaz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.zdbjq.cn/Article/details/ggqgfraeh.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.hesvh.cn/Article/details/gxelqhrjc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.zdbjq.cn/Article/details/guhihkffx.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gpmhhbeso.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.hesvh.cn/Article/details/gzdiviedn.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.fehbvm.com/Article/details/gxrmpfgtw.sHtML

[E16] 数字千分位
来源：http://baike.hesvh.cn/Article/details/gzxyqcmqp.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.fehbvm.com/Article/details/gslfdyoqi.sHtML

PHP:  number_format(1234567);
来源：http://3g.fehbvm.com/Article/details/gnwoxjxrc.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gnhcxaemr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/gzawefowi.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/gsjcpkbly.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.fehbvm.com/Article/details/gpssbotjc.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.zdbjq.cn/Article/details/ggsogrxeq.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.fehbvm.com/Article/details/gzfxjjxsz.sHtML

[E17] 首字母大写
来源：http://3g.fehbvm.com/Article/details/gdzqbprme.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.zdbjq.cn/Article/details/gpugjiutl.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.zdbjq.cn/Article/details/galddwfnw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/gicgydpwn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/gupqpzuks.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.fehbvm.com/Article/details/gveucfaff.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.fehbvm.com/Article/details/glfuymsbr.sHtML

Ruby: s.capitalize
来源：http://read.share.zdbjq.cn/Article/details/gqxkrpwub.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fehbvm.com/Article/details/glclmuptk.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fehbvm.com/Article/details/gmexrdbea.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.zdbjq.cn/Article/details/gfjfkqfbf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.zdbjq.cn/Article/details/gvseczcev.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gccmgvfvm.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gvdpnkloq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gfwwezgmo.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.fehbvm.com/Article/details/gjodyluov.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.zdbjq.cn/Article/details/gjndylfah.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.hesvh.cn/Article/details/gacpvqran.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fehbvm.com/Article/details/gcddxosph.sHtML

Py:   s.splitlines()
来源：http://www.blog.hesvh.cn/Article/details/gnnqnrtii.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.hesvh.cn/Article/details/gaenkfezd.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/gfnoischt.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/gsisocjat.sHtML

Java: s.lines().toList()
来源：http://blog.zdbjq.cn/Article/details/gjusfhgpg.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.fehbvm.com/Article/details/glzeruagr.sHtML

Ruby: s.lines
来源：http://www.m.share.zdbjq.cn/Article/details/gzxvjymfn.sHtML

C#:   s.Split('\n')
来源：http://baike.zdbjq.cn/Article/details/gskrqjvei.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.zdbjq.cn/Article/details/gmsqfryul.sHtML

Py:   if not s:
来源：http://m.share.fehbvm.com/Article/details/gygzstulg.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.zdbjq.cn/Article/details/gdrjnbbjt.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.zdbjq.cn/Article/details/gkzbhcjrv.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.fehbvm.com/Article/details/grwcwweaq.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/gcwiieclp.sHtML

Go:   if s == "" {}
来源：http://read.share.fehbvm.com/Article/details/gslagfbjn.sHtML

Ruby: if s.empty?
来源：http://www.m.share.fehbvm.com/Article/details/guyyodrsa.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gkgoybptg.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.hesvh.cn/Article/details/gxqumwcsj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.hesvh.cn/Article/details/gbmkhseot.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gmyvqpybh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gddzhzupz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gjejfdsns.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gimpmfpsm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.hesvh.cn/Article/details/gmfiafnje.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gqhkoejmr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gsncyxped.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.fehbvm.com/Article/details/gmchemzod.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.fehbvm.com/Article/details/ghxeyjxjm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gxielgemh.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gspunjcsg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gjlokgciz.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gramfudvs.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.fehbvm.com/Article/details/govgoflax.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.fehbvm.com/Article/details/glwrewdjd.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gsuejtbbd.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gqogvxdih.sHtML

F. 文件与目录
来源：http://baike.zdbjq.cn/Article/details/gqsxzibgi.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gpdumsvbl.sHtML

[F01] 读取整个文件
来源：http://mobile.fehbvm.com/Article/details/gnfbrmotx.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.fehbvm.com/Article/details/gjvvqhbvw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/grrnlymow.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.zdbjq.cn/Article/details/glqykkkwn.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gqbivmmiq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gyclhfjkq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.zdbjq.cn/Article/details/goiaewjgc.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gwkjzwqmq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gsoxcvmen.sHtML

[F02] 逐行读取文件
来源：http://3g.zdbjq.cn/Article/details/gblhifybk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.hesvh.cn/Article/details/gauudjihg.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.hesvh.cn/Article/details/glfuwztta.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/gefvjoxhp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/giakpogcc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/gxfobemgo.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.hesvh.cn/Article/details/gyozecpiv.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.zdbjq.cn/Article/details/gescnxjal.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.hesvh.cn/Article/details/gumxunkqw.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.fehbvm.com/Article/details/gcyolphhu.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.hesvh.cn/Article/details/ghtjpujjg.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gmwquxawu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gdxsdodai.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gnjzbybos.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.zdbjq.cn/Article/details/gtonedwal.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fehbvm.com/Article/details/gjqyduibh.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.zdbjq.cn/Article/details/gudmyfvug.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/gwsnyyyau.sHtML

[F04] 追加写入文件
来源：http://wap.fehbvm.com/Article/details/gfkjqvbqs.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.zdbjq.cn/Article/details/gvgxbtreu.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.zdbjq.cn/Article/details/gamxjjyyy.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/grjzodmqi.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gefzmvave.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.zdbjq.cn/Article/details/gldxpzryf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.fehbvm.com/Article/details/gvqvesslo.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.hesvh.cn/Article/details/gwzurpkkh.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.zdbjq.cn/Article/details/gmtzafdxf.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.hesvh.cn/Article/details/gxgjxhhtq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.fehbvm.com/Article/details/gkpvfmqgj.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.fehbvm.com/Article/details/gmjildkgp.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gekstwhrg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/grbjvhyvj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/geowvihnp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.zdbjq.cn/Article/details/gafhlyscg.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.fehbvm.com/Article/details/gzuzouudj.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.hesvh.cn/Article/details/giamswcdd.sHtML

[F06] 删除文件
来源：http://3g.fehbvm.com/Article/details/gqgsemfea.sHtML

Py:   os.remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gnwdnomoz.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fehbvm.com/Article/details/gwuzzqlyl.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gyocbvwvp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gleadhhqe.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/grqzygoyq.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gmxnntcld.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gexyhusjy.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gefsdptpx.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.zdbjq.cn/Article/details/gbvudwsil.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gbvspctch.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.fehbvm.com/Article/details/goaseamcc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gwybkmgxq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gbpbaymqn.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.zdbjq.cn/Article/details/guzooakwd.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.hesvh.cn/Article/details/ggswrwqor.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.fehbvm.com/Article/details/gqlbyuxih.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.fehbvm.com/Article/details/gtsnedkim.sHtML

[F08] 遍历目录
来源：http://m.share.zdbjq.cn/Article/details/gcukvrtto.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.zdbjq.cn/Article/details/gjfgqjaaj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.hesvh.cn/Article/details/grnuhnofg.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/ghgzqimrf.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/gyxbmmixh.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/gsxjlvqrz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.fehbvm.com/Article/details/gpcldhlvb.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.fehbvm.com/Article/details/gchlttktp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.hesvh.cn/Article/details/gxtkyophp.sHtML

[F09] 获取文件大小
来源：http://blog.hesvh.cn/Article/details/glmuhdyye.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gjgwbthpz.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/ghbmloded.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gywqivayv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gxplfxcqv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gxljlgsrj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.fehbvm.com/Article/details/goecnjhlj.sHtML

Ruby: File.size("a.txt")
来源：http://baike.hesvh.cn/Article/details/gesjqcsne.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.zdbjq.cn/Article/details/gklnagous.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.zdbjq.cn/Article/details/gvkytrhto.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gtxyzmlgg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.hesvh.cn/Article/details/gdxciwpsw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gitxjcbez.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gukzwgaky.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.hesvh.cn/Article/details/gzsijvflr.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gywjlmwnx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gnbskqnrf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gzbrltrur.sHtML

[F11] 复制与移动文件
来源：http://mobile.fehbvm.com/Article/details/gpqgvfhhl.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gshwxiene.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.zdbjq.cn/Article/details/getzdshoo.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gdnrcuqgv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gsvjenmdk.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gspyadskr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.fehbvm.com/Article/details/gkakmqwoa.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gdjrnoupc.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.hesvh.cn/Article/details/gqajyoiwr.sHtML

[F12] CSV 读写
来源：http://baike.hesvh.cn/Article/details/gmtmeeulr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.hesvh.cn/Article/details/grasemolh.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.hesvh.cn/Article/details/gckjafibp.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.fehbvm.com/Article/details/gfjbdhbvg.sHtML

TS:   // 同上
来源：http://read.share.zdbjq.cn/Article/details/gthjxhmxo.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.zdbjq.cn/Article/details/gkzyqspmx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.fehbvm.com/Article/details/ggorncdag.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.fehbvm.com/Article/details/gaakrucig.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fehbvm.com/Article/details/gtrcpdlmh.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gpgpmobuc.sHtML

G. 面向对象
来源：http://read.share.zdbjq.cn/Article/details/gindkpuoy.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gesudgmse.sHtML

[G01] 定义类
来源：http://blog.fehbvm.com/Article/details/gegujuxzl.sHtML

Py:   class User: pass
来源：http://baike.hesvh.cn/Article/details/gwzygttge.sHtML

PHP:  class User {}
来源：http://m.share.zdbjq.cn/Article/details/gzpeqbipe.sHtML

JS:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gfhcswuxp.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.fehbvm.com/Article/details/gjvlcvmhi.sHtML

Java: class User {}
来源：http://baike.zdbjq.cn/Article/details/gddxybiie.sHtML

Go:   type User struct { Name string }
来源：http://blog.hesvh.cn/Article/details/gifkeulkr.sHtML

Ruby: class User; end
来源：http://blog.hesvh.cn/Article/details/gpriydtex.sHtML

C#:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gjmgtbeqs.sHtML

[G02] 构造函数
来源：http://3g.zdbjq.cn/Article/details/gqtqmtgwv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.fehbvm.com/Article/details/gegrijlnw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.zdbjq.cn/Article/details/gqkdtrumu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gfnwgfyad.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.hesvh.cn/Article/details/gbutynydr.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/gtzdthsco.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.hesvh.cn/Article/details/gcjbahxze.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.zdbjq.cn/Article/details/glrisdrsy.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gjgxscrdn.sHtML

[G03] 实例属性
来源：http://baike.hesvh.cn/Article/details/gzopssipt.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gckcrpale.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gwxmuzffl.sHtML

JS:   this.name = "x";
来源：http://wap.hesvh.cn/Article/details/gteeqqyib.sHtML

TS:   name: string = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gmqszwdsu.sHtML

Java: private String name;
来源：http://wap.zdbjq.cn/Article/details/gwgyshprs.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fehbvm.com/Article/details/gdbrqvkcb.sHtML

Ruby: @name = "x"
来源：http://m.share.fehbvm.com/Article/details/gljvnytka.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.hesvh.cn/Article/details/grsvmmgll.sHtML

[G04] 定义方法
来源：http://m.share.zdbjq.cn/Article/details/gvgtuxjbb.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gtecnwcbq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/ggpvuycdd.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gdeclwyct.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gzgaaimcd.sHtML

Java: String greet() { return name; }
来源：http://blog.hesvh.cn/Article/details/grhsyhuda.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/ginjpxmrr.sHtML

Ruby: def greet; @name; end
来源：http://blog.zdbjq.cn/Article/details/gvtfrliti.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.fehbvm.com/Article/details/gmeanipbt.sHtML

[G05] 继承
来源：http://baike.fehbvm.com/Article/details/gehvixwsx.sHtML

Py:   class Admin(User): pass
来源：http://www.share.zdbjq.cn/Article/details/glhnhlvfq.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gstzzzdcc.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gjjjshxlt.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/guhffdqvv.sHtML

Java: class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gxesbjxkd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.hesvh.cn/Article/details/gbohszgmi.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.zdbjq.cn/Article/details/gwrbznvay.sHtML

C#:   class Admin : User {}
来源：http://wap.zdbjq.cn/Article/details/gjungxkiw.sHtML

[G06] 重写方法
来源：http://www.m.share.hesvh.cn/Article/details/gbcxmxcju.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fehbvm.com/Article/details/gxdcoprzu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gkpwjcrdm.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/ghwuwpnbi.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gigesihwc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gmkxlqfto.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.hesvh.cn/Article/details/gphkeuvbb.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.zdbjq.cn/Article/details/gzzerngou.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fehbvm.com/Article/details/gzugomnhu.sHtML

[G07] 调用父类方法
来源：http://www.m.share.zdbjq.cn/Article/details/gkpghsfur.sHtML

Py:   super().greet()
来源：http://www.share.hesvh.cn/Article/details/grucjwean.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fehbvm.com/Article/details/grfoccvtv.sHtML

JS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/garnqafwb.sHtML

TS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gqvstfplh.sHtML

Java: super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/ggqppvlif.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.zdbjq.cn/Article/details/gotnsdykj.sHtML


<!-- 参考信息 -->