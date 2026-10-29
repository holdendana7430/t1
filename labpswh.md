代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.fehbvm.com/Article/details/gwdgdxzzh.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.hesvh.cn/Article/details/gxcclfhnv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gkmlogydv.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gleryobzf.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.hesvh.cn/Article/details/gohyswshn.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.hesvh.cn/Article/details/gijggudbi.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.hesvh.cn/Article/details/girxlnwop.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.fehbvm.com/Article/details/gwzimaydp.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.hesvh.cn/Article/details/gtlofkplf.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/glwdcykmc.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fehbvm.com/Article/details/goiiwbkeg.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gknuyisgx.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gtefirvmr.sHtML

Java: String.format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gnmzuufuk.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gfqdknoym.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gtrzctqsn.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.fehbvm.com/Article/details/gzqrkxpsl.sHtML

[E11] 反转字符串
来源：http://read.share.zdbjq.cn/Article/details/grdjztlwo.sHtML

Py:   s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/gqcguurhy.sHtML

PHP:  strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gshpafyrt.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/giymeenzl.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gyidiogqi.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.hesvh.cn/Article/details/gonxgxbla.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.fehbvm.com/Article/details/gqkwxitia.sHtML

Ruby: s.reverse
来源：http://baike.fehbvm.com/Article/details/ghhesibnr.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gsjstnfsk.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.fehbvm.com/Article/details/gsqgsdbqq.sHtML

Py:   s.count("a")
来源：http://blog.fehbvm.com/Article/details/gpynkxeix.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.hesvh.cn/Article/details/gisgqegus.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gjuuipnss.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gomcodurc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.zdbjq.cn/Article/details/gbythflnt.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.fehbvm.com/Article/details/gtymbwonx.sHtML

Ruby: s.count("a")
来源：http://wap.fehbvm.com/Article/details/gksiqoqov.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.zdbjq.cn/Article/details/gjehmygkk.sHtML

[E13] 逐字符遍历
来源：http://www.share.zdbjq.cn/Article/details/gbntnwjnu.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.zdbjq.cn/Article/details/gutibvxwi.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.fehbvm.com/Article/details/gwcxmwzll.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/ghhwbvuli.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gjhxqhnhm.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gtxhlnmhp.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gcvfcxqny.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.fehbvm.com/Article/details/gxjvlwvyp.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.fehbvm.com/Article/details/ggsznhiwk.sHtML

[E14] URL 编码与 Base64
来源：http://blog.fehbvm.com/Article/details/gidttjebh.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.hesvh.cn/Article/details/gvrsdnnle.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.fehbvm.com/Article/details/gjbcbiidg.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.zdbjq.cn/Article/details/gwoxqflcz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.fehbvm.com/Article/details/ggfbnleys.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.hesvh.cn/Article/details/guxbicovm.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.fehbvm.com/Article/details/gljbezwfe.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.zdbjq.cn/Article/details/guwhjlvtl.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gdiwiwkum.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fehbvm.com/Article/details/gtydzpmvb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.hesvh.cn/Article/details/gsvwbaqix.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.zdbjq.cn/Article/details/gjglckavz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.fehbvm.com/Article/details/glwmpverh.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.fehbvm.com/Article/details/glhpznvem.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fehbvm.com/Article/details/gqhisufmq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.hesvh.cn/Article/details/gtiecfodi.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gxgmyopdh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.fehbvm.com/Article/details/ghnlglvga.sHtML

[E16] 数字千分位
来源：http://3g.zdbjq.cn/Article/details/gjkfpmewh.sHtML

Py:   f"{1234567:,}"
来源：http://3g.zdbjq.cn/Article/details/gjkjspecu.sHtML

PHP:  number_format(1234567);
来源：http://blog.hesvh.cn/Article/details/gzwuimgks.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gpeukidiw.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gyemucbwh.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.hesvh.cn/Article/details/gqrxtbjkx.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.zdbjq.cn/Article/details/gmgczqnqp.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.zdbjq.cn/Article/details/gaxjtbinc.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.zdbjq.cn/Article/details/gdaxqxauq.sHtML

[E17] 首字母大写
来源：http://www.share.fehbvm.com/Article/details/gzrqlnmlm.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.hesvh.cn/Article/details/glgyvkmsk.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.hesvh.cn/Article/details/gdxwyfebs.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/gffbpwqcr.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/geeygfgul.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fehbvm.com/Article/details/gwcwhqmhp.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.hesvh.cn/Article/details/gzbxdnydr.sHtML

Ruby: s.capitalize
来源：http://blog.zdbjq.cn/Article/details/gisyzoxek.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.hesvh.cn/Article/details/gjlawuafs.sHtML

[E18] 模板占位符替换
来源：http://3g.zdbjq.cn/Article/details/gycsqoegb.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.hesvh.cn/Article/details/gjcirsgqz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.zdbjq.cn/Article/details/glpekoxfj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gggehakqx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gmvcqksot.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/grkpdvqaf.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gbriaeeaj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.hesvh.cn/Article/details/gulgavbzz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.hesvh.cn/Article/details/gseayipyb.sHtML

[E19] 多行文本按行拆分
来源：http://3g.zdbjq.cn/Article/details/gidjaylui.sHtML

Py:   s.splitlines()
来源：http://read.share.hesvh.cn/Article/details/gcqwgpuki.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.hesvh.cn/Article/details/gnoeuyptw.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gwyutwrex.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gknaabrtk.sHtML

Java: s.lines().toList()
来源：http://3g.fehbvm.com/Article/details/gbyqkmzdo.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.hesvh.cn/Article/details/gmdjbtigr.sHtML

Ruby: s.lines
来源：http://www.m.share.zdbjq.cn/Article/details/gqrcxnwtp.sHtML

C#:   s.Split('\n')
来源：http://www.blog.zdbjq.cn/Article/details/gyuznanvm.sHtML

[E20] 判断字符串是否为空
来源：http://blog.hesvh.cn/Article/details/gktoxmtdq.sHtML

Py:   if not s:
来源：http://3g.hesvh.cn/Article/details/gptwsrwxl.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.zdbjq.cn/Article/details/gctmfpwoo.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.fehbvm.com/Article/details/geyvanoex.sHtML

TS:   if (s === "") {}
来源：http://baike.fehbvm.com/Article/details/gvszfophi.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/gscjubczf.sHtML

Go:   if s == "" {}
来源：http://www.blog.hesvh.cn/Article/details/gbgdhfmpj.sHtML

Ruby: if s.empty?
来源：http://read.share.hesvh.cn/Article/details/gybbguqqh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.zdbjq.cn/Article/details/givcwpunx.sHtML

[E21] 超长截断加省略号
来源：http://read.share.fehbvm.com/Article/details/gbdzhccat.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.zdbjq.cn/Article/details/gaztkeiyc.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gwbxofejr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gdfjruspt.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gybqwgvyj.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/glycxslqo.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fehbvm.com/Article/details/gknqqtmce.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gngujlxwi.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gvuiprses.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.zdbjq.cn/Article/details/gbpcmpwlm.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.hesvh.cn/Article/details/gpcqlmrnu.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gpfywqyho.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/gkkdtwmxu.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/ggfclxrqp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.hesvh.cn/Article/details/gdwocjanu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.zdbjq.cn/Article/details/gwysbvqot.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gnqmurrck.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.fehbvm.com/Article/details/gmwozenye.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmxcyesdx.sHtML

F. 文件与目录
来源：http://m.share.hesvh.cn/Article/details/gfjvrmjfw.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gzadaaclv.sHtML

[F01] 读取整个文件
来源：http://read.share.hesvh.cn/Article/details/gkujinwjw.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.fehbvm.com/Article/details/gbgdencoz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.fehbvm.com/Article/details/gmvvrzfiq.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.hesvh.cn/Article/details/gnlpxeuyj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/guafqvtis.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/glsoxpkst.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.zdbjq.cn/Article/details/gmxnpqbgy.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.hesvh.cn/Article/details/grjyezlrk.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gojhtjsug.sHtML

[F02] 逐行读取文件
来源：http://mobile.fehbvm.com/Article/details/gjkglhbtv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.fehbvm.com/Article/details/gaapoqaqu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.fehbvm.com/Article/details/gxrdsqdse.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gqaihkazd.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/gurlzybfg.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gzirkxonc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.zdbjq.cn/Article/details/grqjbzjjy.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.zdbjq.cn/Article/details/gpmefllea.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.fehbvm.com/Article/details/gfxkdzppd.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.hesvh.cn/Article/details/gyjmhquiu.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.hesvh.cn/Article/details/gpkbhmkep.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gyluehfwk.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/glywmubir.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gcydigeoa.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.hesvh.cn/Article/details/ghsjwhiee.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.zdbjq.cn/Article/details/gfjidqfvv.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gdacnflkb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/ghsarojhh.sHtML

[F04] 追加写入文件
来源：http://wap.fehbvm.com/Article/details/gmrvvdeie.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.hesvh.cn/Article/details/gjynejjko.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fehbvm.com/Article/details/gmduroofi.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gsmtzavaq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gibpajavj.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.fehbvm.com/Article/details/gfvkbjtbt.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.zdbjq.cn/Article/details/gcjktwjkw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.fehbvm.com/Article/details/gdqnsvhqr.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.zdbjq.cn/Article/details/ghedvaobi.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.zdbjq.cn/Article/details/goolhuxmm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.hesvh.cn/Article/details/glliavkiw.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/ggolidhnb.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gbdtwjbgi.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gjwmsqgoa.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gusfycuxh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.fehbvm.com/Article/details/ghrhosauq.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.fehbvm.com/Article/details/gzmjwuhbf.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gtjuuwpmo.sHtML

[F06] 删除文件
来源：http://3g.hesvh.cn/Article/details/gqkajujcb.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/ghhukpsdc.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/glektfetr.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gzzgmhhvg.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gcdjzyjvx.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gaumodmzw.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/godrhhncr.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gazzkkakr.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gewkzzywj.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.fehbvm.com/Article/details/gzmmaqhtq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gefkhhxlg.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.zdbjq.cn/Article/details/gskcorljn.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gysixuwyo.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/gpneaasjp.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.zdbjq.cn/Article/details/gwwfhcung.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fehbvm.com/Article/details/gbxlwehqu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.fehbvm.com/Article/details/gvkwtpwoc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.zdbjq.cn/Article/details/ghrxuvrdr.sHtML

[F08] 遍历目录
来源：http://www.blog.fehbvm.com/Article/details/gyyefgmxr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.zdbjq.cn/Article/details/gpvthrirf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.zdbjq.cn/Article/details/gvfemjpym.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gjqklmniz.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gvskegygu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/grwyhawek.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.hesvh.cn/Article/details/gosxylbpr.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fehbvm.com/Article/details/gkrmqmrxs.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fehbvm.com/Article/details/gqobducnw.sHtML

[F09] 获取文件大小
来源：http://read.share.fehbvm.com/Article/details/gqdutklwj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.fehbvm.com/Article/details/gskkecfpm.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gkgqgxnvn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/guvedidgq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gaoeujwjm.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/grntbvupv.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.zdbjq.cn/Article/details/gmmolckfp.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gtsfvyhjw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.hesvh.cn/Article/details/gmsevzgrl.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.hesvh.cn/Article/details/gwvjxhxsj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gakouvuvh.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.fehbvm.com/Article/details/giioogwvi.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gmotriocy.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gcwqvzyfu.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.zdbjq.cn/Article/details/gxhlihamk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/glvxlnifn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gyyxzaeet.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gejjhokdy.sHtML

[F11] 复制与移动文件
来源：http://m.share.hesvh.cn/Article/details/ghhzzdvyp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gqwqhulfw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.hesvh.cn/Article/details/gubaexyfy.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gouberbgj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/ghmeqwhkr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fehbvm.com/Article/details/ggqlgqkjs.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.hesvh.cn/Article/details/gibocemys.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gwigzybbb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.zdbjq.cn/Article/details/gaimszmuf.sHtML

[F12] CSV 读写
来源：http://baike.hesvh.cn/Article/details/gglaxrabz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.hesvh.cn/Article/details/glpwgqmej.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.hesvh.cn/Article/details/gfvlmoxto.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.zdbjq.cn/Article/details/giwresztv.sHtML

TS:   // 同上
来源：http://wap.zdbjq.cn/Article/details/gjvapfzus.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.hesvh.cn/Article/details/gwaimodee.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.zdbjq.cn/Article/details/glayydedz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.fehbvm.com/Article/details/gcseeuoaf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.hesvh.cn/Article/details/gqasahkbv.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzaowyufy.sHtML

G. 面向对象
来源：http://baike.hesvh.cn/Article/details/gdljhopgf.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/guwmrysth.sHtML

[G01] 定义类
来源：http://blog.fehbvm.com/Article/details/gbneeqksm.sHtML

Py:   class User: pass
来源：http://read.share.fehbvm.com/Article/details/gcsxtiudx.sHtML

PHP:  class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gyqssiabr.sHtML

JS:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gtdywsuer.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.fehbvm.com/Article/details/gkyjilqki.sHtML

Java: class User {}
来源：http://blog.hesvh.cn/Article/details/gwmyhzsga.sHtML

Go:   type User struct { Name string }
来源：http://read.share.zdbjq.cn/Article/details/gwndtvvhr.sHtML

Ruby: class User; end
来源：http://www.m.share.hesvh.cn/Article/details/gusakwfkl.sHtML

C#:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gdjusmvyt.sHtML

[G02] 构造函数
来源：http://m.share.fehbvm.com/Article/details/gvmqvjpxv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.zdbjq.cn/Article/details/gnozdvnvt.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.zdbjq.cn/Article/details/gjtndmhuw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gjctbjdxs.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.hesvh.cn/Article/details/gkmlozzyv.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gebqkwqut.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.fehbvm.com/Article/details/gykdestrl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fehbvm.com/Article/details/gbdkclhrk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.hesvh.cn/Article/details/gzvigkjew.sHtML

[G03] 实例属性
来源：http://mobile.zdbjq.cn/Article/details/gaqdypizm.sHtML

Py:   self.name = "x"
来源：http://blog.hesvh.cn/Article/details/gvtppmwic.sHtML

PHP:  public string $name = "x";
来源：http://www.share.hesvh.cn/Article/details/glpqrhkku.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/gjmebggjs.sHtML

TS:   name: string = "x";
来源：http://blog.hesvh.cn/Article/details/gnscmedge.sHtML

Java: private String name;
来源：http://m.share.zdbjq.cn/Article/details/glgjjlwmp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.zdbjq.cn/Article/details/gnebzkewa.sHtML

Ruby: @name = "x"
来源：http://3g.hesvh.cn/Article/details/gcthlmkej.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.zdbjq.cn/Article/details/gizfcbfwe.sHtML

[G04] 定义方法
来源：http://3g.zdbjq.cn/Article/details/gicaiqavy.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gduphwcua.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gdprvqfpr.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gfpbgdlws.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gmctzzkib.sHtML

Java: String greet() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gwzfwcfgq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gdrqnwlrm.sHtML

Ruby: def greet; @name; end
来源：http://baike.fehbvm.com/Article/details/gnbvanvzt.sHtML

C#:   public string Greet() => Name;
来源：http://blog.fehbvm.com/Article/details/gyqkzhcmy.sHtML

[G05] 继承
来源：http://m.share.hesvh.cn/Article/details/gjftqtuhz.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.hesvh.cn/Article/details/grvsuvmbt.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/ghfkfuwgj.sHtML

JS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gmhvimzuq.sHtML

TS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gicliuquc.sHtML

Java: class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gghkkqijw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.fehbvm.com/Article/details/gsdvtxxsg.sHtML

Ruby: class Admin < User; end
来源：http://blog.fehbvm.com/Article/details/gdupkqktp.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fehbvm.com/Article/details/gwaigrnbm.sHtML

[G06] 重写方法
来源：http://www.m.share.hesvh.cn/Article/details/gwzfsytos.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.zdbjq.cn/Article/details/grcuiemxi.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gzjuszdeb.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gvafiyiac.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gidirkkzb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gzgnoawvc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fehbvm.com/Article/details/gsfkqkeof.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.zdbjq.cn/Article/details/gxptgcedl.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.zdbjq.cn/Article/details/gpfeohwxu.sHtML

[G07] 调用父类方法
来源：http://read.share.hesvh.cn/Article/details/gwymckntb.sHtML

Py:   super().greet()
来源：http://www.share.zdbjq.cn/Article/details/geyygcxze.sHtML

PHP:  parent::greet();
来源：http://mobile.hesvh.cn/Article/details/gqfvcgztz.sHtML

JS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/ggjxoardl.sHtML

TS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gcnsabclf.sHtML

Java: super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gifphehji.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.zdbjq.cn/Article/details/gixuqgzuw.sHtML


<!-- 参考信息 -->