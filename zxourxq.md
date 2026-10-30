代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.hesvh.cn/Article/details/gwftrqyxu.sHtML

[E11] 反转字符串
来源：http://baike.zdbjq.cn/Article/details/galmazccb.sHtML

Py:   s[::-1]
来源：http://m.share.hesvh.cn/Article/details/gkmmwyuej.sHtML

PHP:  strrev($s);
来源：http://baike.fehbvm.com/Article/details/gffyukwun.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gbrxchnis.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gwjdolxlt.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gptczjdyf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.zdbjq.cn/Article/details/gmznqtymj.sHtML

Ruby: s.reverse
来源：http://blog.fehbvm.com/Article/details/gvtlapzah.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gcuaaksjx.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.hesvh.cn/Article/details/gcwrpagfu.sHtML

Py:   s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gledxmpsj.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.hesvh.cn/Article/details/grkmqtiqt.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/gcozqsduq.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gnjswsdyp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.zdbjq.cn/Article/details/gkwtsyghd.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.hesvh.cn/Article/details/gzmvtzwgp.sHtML

Ruby: s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gkyzfploz.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.hesvh.cn/Article/details/gfhkdjbst.sHtML

[E13] 逐字符遍历
来源：http://m.share.hesvh.cn/Article/details/gfpaxhpqq.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.fehbvm.com/Article/details/gmkdfdxju.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.fehbvm.com/Article/details/gakrqilvc.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/ghxymqtbn.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/gqgjijczr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gpxqkpinp.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.fehbvm.com/Article/details/gmcgphrjo.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.hesvh.cn/Article/details/gdsdoywsw.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gbvxhquzl.sHtML

[E14] URL 编码与 Base64
来源：http://3g.fehbvm.com/Article/details/gaeqcvgir.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.fehbvm.com/Article/details/gkpcojcgu.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.hesvh.cn/Article/details/gmwltkpir.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.zdbjq.cn/Article/details/gduvgfieo.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.zdbjq.cn/Article/details/gdmesrjzv.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.zdbjq.cn/Article/details/guxscubsl.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.zdbjq.cn/Article/details/gynhpynml.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.zdbjq.cn/Article/details/gqfmhotpo.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.zdbjq.cn/Article/details/glzsbucju.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.hesvh.cn/Article/details/guetwrovb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.zdbjq.cn/Article/details/gkvajxvsi.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/ghlunnflq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.hesvh.cn/Article/details/gaefhvlpc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.hesvh.cn/Article/details/gjbfvlgmf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.fehbvm.com/Article/details/gpdesotwz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.zdbjq.cn/Article/details/gkxooulqy.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.fehbvm.com/Article/details/gqmusabjc.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.fehbvm.com/Article/details/gdcmfvgny.sHtML

[E16] 数字千分位
来源：http://www.m.share.zdbjq.cn/Article/details/gbqxmxobh.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.zdbjq.cn/Article/details/guvqveozl.sHtML

PHP:  number_format(1234567);
来源：http://3g.hesvh.cn/Article/details/gfiaxurxr.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gpattdsvt.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/gigmrwjam.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.fehbvm.com/Article/details/giflukabp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.fehbvm.com/Article/details/gxxbaxrzw.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.fehbvm.com/Article/details/ghgmrhbmh.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.fehbvm.com/Article/details/guxvkbpiq.sHtML

[E17] 首字母大写
来源：http://blog.zdbjq.cn/Article/details/gmiolzshv.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.zdbjq.cn/Article/details/gbhtvtbnm.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.fehbvm.com/Article/details/golpzvqkq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/gktfuqwga.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/ggghzrfiz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.fehbvm.com/Article/details/gykhysrbw.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.hesvh.cn/Article/details/gkifftwcn.sHtML

Ruby: s.capitalize
来源：http://wap.hesvh.cn/Article/details/gwrmdiawb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.zdbjq.cn/Article/details/gsbzodnao.sHtML

[E18] 模板占位符替换
来源：http://3g.fehbvm.com/Article/details/gipclisdd.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fehbvm.com/Article/details/gjvebvbku.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.zdbjq.cn/Article/details/gjcxhhwyo.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gwyakllra.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gqiwpuauz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gmbberdvl.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gcpxxvoiw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.zdbjq.cn/Article/details/gdfozyzhh.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.zdbjq.cn/Article/details/grnpwkqdw.sHtML

[E19] 多行文本按行拆分
来源：http://blog.zdbjq.cn/Article/details/gehlghxeb.sHtML

Py:   s.splitlines()
来源：http://www.share.zdbjq.cn/Article/details/grsqhdrjd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.hesvh.cn/Article/details/gggzrewuv.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/ginhtdyez.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/glopmciuq.sHtML

Java: s.lines().toList()
来源：http://3g.fehbvm.com/Article/details/gztyfythj.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.hesvh.cn/Article/details/gfmwkxpni.sHtML

Ruby: s.lines
来源：http://read.share.zdbjq.cn/Article/details/gshitcjvv.sHtML

C#:   s.Split('\n')
来源：http://wap.zdbjq.cn/Article/details/gmcwspycg.sHtML

[E20] 判断字符串是否为空
来源：http://baike.fehbvm.com/Article/details/gwamtkjgu.sHtML

Py:   if not s:
来源：http://m.share.fehbvm.com/Article/details/gpnoklgwm.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.fehbvm.com/Article/details/gjndcdlnk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.hesvh.cn/Article/details/gfvdkivzi.sHtML

TS:   if (s === "") {}
来源：http://read.share.hesvh.cn/Article/details/gppvdqegu.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gejhatdjj.sHtML

Go:   if s == "" {}
来源：http://m.share.fehbvm.com/Article/details/gkarwjodc.sHtML

Ruby: if s.empty?
来源：http://3g.hesvh.cn/Article/details/gohtseoqa.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.zdbjq.cn/Article/details/grnirdwni.sHtML

[E21] 超长截断加省略号
来源：http://baike.fehbvm.com/Article/details/gpkyvvrgy.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.zdbjq.cn/Article/details/gqtmjwyxe.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gzbjowhdr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gxjcrjfad.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gxhppgpjs.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/guvtooxmj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.zdbjq.cn/Article/details/gdrsruivc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/ghiyfmwrk.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gluqfrlyw.sHtML

[E22] 字节长度与字符长度
来源：http://wap.fehbvm.com/Article/details/ggbpjismz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.zdbjq.cn/Article/details/gdbfhmodq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gqbpwarbi.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gmkmwcdgi.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gkskehals.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.fehbvm.com/Article/details/gfqlfwcua.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.hesvh.cn/Article/details/gffmzqivr.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.hesvh.cn/Article/details/gmiaqggfb.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.fehbvm.com/Article/details/guqqpocpm.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gwuiyxveh.sHtML

F. 文件与目录
来源：http://3g.hesvh.cn/Article/details/gyzujlkyk.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gmzucpjov.sHtML

[F01] 读取整个文件
来源：http://www.m.share.hesvh.cn/Article/details/gjighxboo.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.fehbvm.com/Article/details/guqtresxc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.hesvh.cn/Article/details/gwpywokqx.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.fehbvm.com/Article/details/geoasdvqm.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gbaasbfwl.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gmljxdvri.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.hesvh.cn/Article/details/gwsgocvul.sHtML

Ruby: File.read("a.txt")
来源：http://wap.zdbjq.cn/Article/details/godtkyhnh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.fehbvm.com/Article/details/gnvinrhvn.sHtML

[F02] 逐行读取文件
来源：http://baike.zdbjq.cn/Article/details/gwbgnnitr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.zdbjq.cn/Article/details/gjmsozvpn.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.hesvh.cn/Article/details/gblfhcayz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/geinhstjc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gqoamlzqr.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gaaswhcbg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.zdbjq.cn/Article/details/grgcatyxw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.fehbvm.com/Article/details/gqdfjnldi.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.zdbjq.cn/Article/details/gcriryewe.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fehbvm.com/Article/details/gktedavmu.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.hesvh.cn/Article/details/gwuzhhskm.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gyweurtdo.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gndojaxxd.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gqgeimomg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.fehbvm.com/Article/details/gbpbnvfbg.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.fehbvm.com/Article/details/ggxwrajko.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.fehbvm.com/Article/details/glbgqivby.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/grvhpzqrj.sHtML

[F04] 追加写入文件
来源：http://wap.hesvh.cn/Article/details/gcauskxjl.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.fehbvm.com/Article/details/ghuxqqnah.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.hesvh.cn/Article/details/gxnbysfed.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/gflozjyts.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/goyqgtkws.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.hesvh.cn/Article/details/gmdpccxod.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.hesvh.cn/Article/details/gjtytspbf.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.zdbjq.cn/Article/details/giuwgfjqr.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.fehbvm.com/Article/details/gqtgpjrlv.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.zdbjq.cn/Article/details/gadmqtsuf.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.fehbvm.com/Article/details/gbtxzwuxl.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gpjmygywr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gvqbesbtw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gdimobylb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/goatiivdy.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.fehbvm.com/Article/details/gopcfkogg.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gynquwqrj.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/geahfijxf.sHtML

[F06] 删除文件
来源：http://www.share.fehbvm.com/Article/details/geffxxagk.sHtML

Py:   os.remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gahimvjit.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/ghvvcbruv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gisktviqg.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gkapvbuqj.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gwkcnchst.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gfltotcme.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.fehbvm.com/Article/details/gfzrauxky.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.fehbvm.com/Article/details/ggqyoccxl.sHtML

[F07] 创建目录（含多级）
来源：http://blog.hesvh.cn/Article/details/gdldyfzuu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gfblswzma.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.hesvh.cn/Article/details/gpwqenivk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gyjrdjagi.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gwcmurlxr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.zdbjq.cn/Article/details/gaszimehs.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.fehbvm.com/Article/details/ghyfgcouy.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.fehbvm.com/Article/details/gdiamifiq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fehbvm.com/Article/details/grlevmjcq.sHtML

[F08] 遍历目录
来源：http://www.share.fehbvm.com/Article/details/guaaizpnt.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.hesvh.cn/Article/details/gugjccfkh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fehbvm.com/Article/details/gyuwhhxuh.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gsgftdilt.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gopbfnyur.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gnzqrirja.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.hesvh.cn/Article/details/gfkejrhec.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gdhxhfsxm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.fehbvm.com/Article/details/gexrjcpln.sHtML

[F09] 获取文件大小
来源：http://3g.hesvh.cn/Article/details/gblrnhrvj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/glxrnkokt.sHtML

PHP:  filesize("a.txt");
来源：http://wap.hesvh.cn/Article/details/gxwrpizev.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gtxnorijx.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/gtarssbyi.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gkonctkxq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fehbvm.com/Article/details/gmdopxsbi.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gzzpqvyel.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.zdbjq.cn/Article/details/gyypbxmlp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.zdbjq.cn/Article/details/gistjiuaw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/ggfloofdg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gunhofroz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gxtjnwdmx.sHtML

TS:   path.extname("a.txt")
来源：http://3g.fehbvm.com/Article/details/gcmhfzeaj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.fehbvm.com/Article/details/guvfhdzri.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gfltydkpp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gvrvpqlqc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gbegsnlgo.sHtML

[F11] 复制与移动文件
来源：http://wap.zdbjq.cn/Article/details/gsfxbeyjx.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gmclsjjae.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.hesvh.cn/Article/details/glcrfulpc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/ghnfwafcy.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/ghordhdwk.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gfkygcviu.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.hesvh.cn/Article/details/gjhtxqxmp.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/glbzmqyan.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.zdbjq.cn/Article/details/gydunwodt.sHtML

[F12] CSV 读写
来源：http://read.share.hesvh.cn/Article/details/gsqkbdkny.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.zdbjq.cn/Article/details/gpgqvnoky.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fehbvm.com/Article/details/gbizxajkj.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.zdbjq.cn/Article/details/gkeytucii.sHtML

TS:   // 同上
来源：http://m.share.fehbvm.com/Article/details/geuudsqnb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.fehbvm.com/Article/details/gcnejuego.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.fehbvm.com/Article/details/gmyxlwmaf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.hesvh.cn/Article/details/gpaxgjezm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fehbvm.com/Article/details/ggdlvgvht.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbelszbhz.sHtML

G. 面向对象
来源：http://mobile.fehbvm.com/Article/details/gsbwsliff.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gskmrzaxc.sHtML

[G01] 定义类
来源：http://m.share.zdbjq.cn/Article/details/ggavjybis.sHtML

Py:   class User: pass
来源：http://baike.zdbjq.cn/Article/details/glqgfifyu.sHtML

PHP:  class User {}
来源：http://blog.zdbjq.cn/Article/details/gtfiziktu.sHtML

JS:   class User {}
来源：http://blog.hesvh.cn/Article/details/gvqnhsavq.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxuxmmwub.sHtML

Java: class User {}
来源：http://3g.zdbjq.cn/Article/details/gnmwgjgzb.sHtML

Go:   type User struct { Name string }
来源：http://m.share.fehbvm.com/Article/details/gngxufhzo.sHtML

Ruby: class User; end
来源：http://m.share.hesvh.cn/Article/details/gavhsclek.sHtML

C#:   class User {}
来源：http://www.share.fehbvm.com/Article/details/ggupsdkan.sHtML

[G02] 构造函数
来源：http://read.share.fehbvm.com/Article/details/gkmyjxzzp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/gspclypwi.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.hesvh.cn/Article/details/gbfbpredq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/ghkuakkwr.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.zdbjq.cn/Article/details/geyvsusig.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/ggbgskzkk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.hesvh.cn/Article/details/gknbzttqn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fehbvm.com/Article/details/grsmbvoio.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.zdbjq.cn/Article/details/ggizlwawc.sHtML

[G03] 实例属性
来源：http://wap.fehbvm.com/Article/details/gwyrsydwp.sHtML

Py:   self.name = "x"
来源：http://mobile.hesvh.cn/Article/details/gsoaopnlq.sHtML

PHP:  public string $name = "x";
来源：http://3g.fehbvm.com/Article/details/gyeuuudrm.sHtML

JS:   this.name = "x";
来源：http://baike.fehbvm.com/Article/details/ggapvqtij.sHtML

TS:   name: string = "x";
来源：http://www.blog.fehbvm.com/Article/details/gzoixjkxl.sHtML

Java: private String name;
来源：http://m.share.fehbvm.com/Article/details/glwtordvj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.hesvh.cn/Article/details/gvoncpkuf.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gynnzdtkk.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gbyygurfp.sHtML

[G04] 定义方法
来源：http://read.share.zdbjq.cn/Article/details/gtxurhjie.sHtML

Py:   def greet(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gsnrgisle.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gxxwbojlq.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gllhloxvg.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gqkcfoaze.sHtML

Java: String greet() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gftkupwqw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gvkzgapmb.sHtML

Ruby: def greet; @name; end
来源：http://wap.fehbvm.com/Article/details/gwitnccwh.sHtML

C#:   public string Greet() => Name;
来源：http://baike.fehbvm.com/Article/details/gmiehxrro.sHtML

[G05] 继承
来源：http://blog.hesvh.cn/Article/details/gwmnachcs.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.zdbjq.cn/Article/details/gsecsgdbg.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gspnsdbuh.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gcocfbaey.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gmxebsgva.sHtML

Java: class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gusggevgs.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fehbvm.com/Article/details/gunbvatzo.sHtML

Ruby: class Admin < User; end
来源：http://www.share.hesvh.cn/Article/details/ggfzybusu.sHtML

C#:   class Admin : User {}
来源：http://www.share.zdbjq.cn/Article/details/gipqunagu.sHtML

[G06] 重写方法
来源：http://m.share.zdbjq.cn/Article/details/goklfqozi.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.hesvh.cn/Article/details/gtdfswpvi.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gvanxgzev.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gqqjpobpi.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gxfjralyr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gecewonpw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fehbvm.com/Article/details/gdreqgpqp.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.zdbjq.cn/Article/details/gcohtumka.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.fehbvm.com/Article/details/gxhjlmrpl.sHtML

[G07] 调用父类方法
来源：http://3g.hesvh.cn/Article/details/gdsghfwfs.sHtML

Py:   super().greet()
来源：http://www.blog.hesvh.cn/Article/details/ggufzbmpt.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fehbvm.com/Article/details/gobleiqvb.sHtML

JS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gyeqkxinz.sHtML

TS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gchskrauj.sHtML

Java: super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gllhkfaaa.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.fehbvm.com/Article/details/goeooptbm.sHtML

Ruby: super
来源：http://www.share.hesvh.cn/Article/details/gswcdiwii.sHtML

C#:   base.Greet();
来源：http://www.m.share.hesvh.cn/Article/details/gxmsiviau.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.zdbjq.cn/Article/details/gifyxlufw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.zdbjq.cn/Article/details/gsikapbin.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fehbvm.com/Article/details/gqrlommqc.sHtML

JS:   static f() {}
来源：http://wap.fehbvm.com/Article/details/gkxhzhpoi.sHtML

TS:   static f(): void {}
来源：http://mobile.zdbjq.cn/Article/details/gaoxonhgk.sHtML

Java: static void f() {}
来源：http://www.blog.fehbvm.com/Article/details/gufmgebky.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.zdbjq.cn/Article/details/ghfhydkbd.sHtML

Ruby: def self.f; end
来源：http://www.blog.hesvh.cn/Article/details/gimsxodka.sHtML

C#:   public static void F() {}
来源：http://mobile.hesvh.cn/Article/details/gwksldrvn.sHtML

[G09] 接口 / 抽象类
来源：http://3g.hesvh.cn/Article/details/gctcehdvw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.zdbjq.cn/Article/details/gazyjtgdm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.fehbvm.com/Article/details/grgtbjwhi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.zdbjq.cn/Article/details/gycwsxlrr.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmiujayhq.sHtML


<!-- 参考信息 -->