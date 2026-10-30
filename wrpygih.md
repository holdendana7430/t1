代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubbjgvww.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.fanxiaobao.xyz/Article/details/gujyjfkkx.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.fanxiaobao.xyz/Article/details/gcimvjpnq.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.fanxiaobao.xyz/Article/details/gbvmlixtz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocbrqvwi.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.fanxiaobao.xyz/Article/details/gnyjibxlx.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.fanxiaobao.xyz/Article/details/gnrrldion.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.fanxiaobao.xyz/Article/details/ggrvxiign.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdytpnwa.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.fanxiaobao.xyz/Article/details/grvyltmte.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwxfgszbg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjntvxbh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmcdgwsq.sHtML

[E11] 反转字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gnvfxlcni.sHtML

Py:   s[::-1]
来源：http://m.share.fanxiaobao.xyz/Article/details/gffnvcmtr.sHtML

PHP:  strrev($s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvegijpp.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.fanxiaobao.xyz/Article/details/guckkwwkq.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.fanxiaobao.xyz/Article/details/gdobeogav.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.fanxiaobao.xyz/Article/details/giylzjmwr.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fanxiaobao.xyz/Article/details/gjufgzudx.sHtML

Ruby: s.reverse
来源：http://baike.fanxiaobao.xyz/Article/details/gorlzeljw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.fanxiaobao.xyz/Article/details/gwtfvtzzp.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdrctabl.sHtML

Py:   s.count("a")
来源：http://3g.fanxiaobao.xyz/Article/details/gsfocnghz.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.fanxiaobao.xyz/Article/details/gmcvqatyu.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzungiwea.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gkudkqyyl.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvqhhqjf.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.fanxiaobao.xyz/Article/details/gjyzlsvpj.sHtML

Ruby: s.count("a")
来源：http://wap.fanxiaobao.xyz/Article/details/gicfndbmg.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.fanxiaobao.xyz/Article/details/gnzqgbait.sHtML

[E13] 逐字符遍历
来源：http://baike.fanxiaobao.xyz/Article/details/goxbznqsf.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnlwagzc.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.fanxiaobao.xyz/Article/details/gkiafjhef.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fanxiaobao.xyz/Article/details/gfthrvxrq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfepiyyw.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.fanxiaobao.xyz/Article/details/gwavwhqgf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gbyzbtuqi.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.fanxiaobao.xyz/Article/details/gzsusjqgp.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.fanxiaobao.xyz/Article/details/gymsswkmr.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geuyeqlax.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.fanxiaobao.xyz/Article/details/gcfxqjxbm.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdqddlqs.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.fanxiaobao.xyz/Article/details/ghmczeddi.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbblgingy.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.fanxiaobao.xyz/Article/details/gydqucdma.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.fanxiaobao.xyz/Article/details/gkcqrpnee.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtiqvulqb.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.fanxiaobao.xyz/Article/details/gpvmorjyp.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdljgyezj.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gqotglvmw.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.fanxiaobao.xyz/Article/details/gfgeiwmxx.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geimgqudi.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gdzosomsg.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.fanxiaobao.xyz/Article/details/gwjjdlrmh.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrehjvpx.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxmulpbpy.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggqzvylme.sHtML

[E16] 数字千分位
来源：http://baike.fanxiaobao.xyz/Article/details/gkpfzqgtm.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gnxzzlrrt.sHtML

PHP:  number_format(1234567);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwphejio.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnaxulye.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnyvjwxst.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.fanxiaobao.xyz/Article/details/geipddznj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.fanxiaobao.xyz/Article/details/greacqfqh.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.fanxiaobao.xyz/Article/details/gitwfvefy.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxwscejs.sHtML

[E17] 首字母大写
来源：http://m.share.fanxiaobao.xyz/Article/details/gasdeaaxw.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnegotopo.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnjhaoqu.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/guwpdvfwu.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fanxiaobao.xyz/Article/details/gyrbfjhjz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.fanxiaobao.xyz/Article/details/ghvedelme.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.fanxiaobao.xyz/Article/details/gypbojvpb.sHtML

Ruby: s.capitalize
来源：http://baike.fanxiaobao.xyz/Article/details/gtzzzwcdf.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.fanxiaobao.xyz/Article/details/gohpwgdks.sHtML

[E18] 模板占位符替换
来源：http://baike.fanxiaobao.xyz/Article/details/glpuwicbq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.fanxiaobao.xyz/Article/details/ghpmnuanf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcinkpuhy.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.fanxiaobao.xyz/Article/details/ghuewadba.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtyynlcxw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.fanxiaobao.xyz/Article/details/glvsswdtx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.fanxiaobao.xyz/Article/details/grrjegxxu.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gmpjquzud.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.fanxiaobao.xyz/Article/details/gmmbzwwbv.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.fanxiaobao.xyz/Article/details/ggihejcqn.sHtML

Py:   s.splitlines()
来源：http://mobile.fanxiaobao.xyz/Article/details/gyguniyre.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.fanxiaobao.xyz/Article/details/godzpfbtq.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkimvyexc.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcnwtfwap.sHtML

Java: s.lines().toList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkbcpphi.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbuuyoyz.sHtML

Ruby: s.lines
来源：http://wap.fanxiaobao.xyz/Article/details/gjdujcebd.sHtML

C#:   s.Split('\n')
来源：http://baike.fanxiaobao.xyz/Article/details/gfvmwcuqg.sHtML

[E20] 判断字符串是否为空
来源：http://baike.fanxiaobao.xyz/Article/details/gxspeewsf.sHtML

Py:   if not s:
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkgcoxyi.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.fanxiaobao.xyz/Article/details/guwcvvils.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjvzliqz.sHtML

TS:   if (s === "") {}
来源：http://blog.fanxiaobao.xyz/Article/details/ghdwvdohv.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fanxiaobao.xyz/Article/details/govfnmpjx.sHtML

Go:   if s == "" {}
来源：http://wap.fanxiaobao.xyz/Article/details/gonnwwigb.sHtML

Ruby: if s.empty?
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndpmpnyb.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwgjjbxg.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpygwhavv.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fanxiaobao.xyz/Article/details/gepbimyqc.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.fanxiaobao.xyz/Article/details/gubqvuwix.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gthsudxvc.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fanxiaobao.xyz/Article/details/gonekyphi.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.fanxiaobao.xyz/Article/details/grqqphogx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fanxiaobao.xyz/Article/details/glmgsdqmv.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.fanxiaobao.xyz/Article/details/gqlqyekfc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.fanxiaobao.xyz/Article/details/gmoeeeomh.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gkpvjrtca.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmwitovem.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fanxiaobao.xyz/Article/details/gurkrxtcw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glamlwucr.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxigfhtf.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaugptwge.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.fanxiaobao.xyz/Article/details/gcqgqurqf.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fanxiaobao.xyz/Article/details/gvqjfrkxr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.fanxiaobao.xyz/Article/details/gbrtzbsed.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnuyelri.sHtML

F. 文件与目录
来源：http://mobile.fanxiaobao.xyz/Article/details/gnibcppuq.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gfucngfeo.sHtML

[F01] 读取整个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gtjpenenb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.fanxiaobao.xyz/Article/details/gzskmbkzy.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gwmtmvcxb.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.fanxiaobao.xyz/Article/details/giwxjhxsx.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.fanxiaobao.xyz/Article/details/gujcirqki.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdaebhxvy.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxwjgxky.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxfecfhq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.fanxiaobao.xyz/Article/details/gbvrkizuo.sHtML

[F02] 逐行读取文件
来源：http://baike.fanxiaobao.xyz/Article/details/gzcpvngqo.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.fanxiaobao.xyz/Article/details/gwymosker.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gswaulkjv.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gixxcwprs.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gzuwolcth.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsrujljuy.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.fanxiaobao.xyz/Article/details/gttitrqss.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.fanxiaobao.xyz/Article/details/goywrjpmy.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.fanxiaobao.xyz/Article/details/grwccytsd.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gickwlvmy.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrufehkt.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gkiymlfkg.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fanxiaobao.xyz/Article/details/glpuabkot.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fanxiaobao.xyz/Article/details/gkozfwoil.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnejpigu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.fanxiaobao.xyz/Article/details/ggiwchdyd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.fanxiaobao.xyz/Article/details/gdkeroxfs.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsauogdco.sHtML

[F04] 追加写入文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geaqdzdwm.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.fanxiaobao.xyz/Article/details/gdfpalprr.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmayovffc.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fanxiaobao.xyz/Article/details/gigbfnqpv.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fanxiaobao.xyz/Article/details/ginuiylca.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.fanxiaobao.xyz/Article/details/gjtrdbewu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goacmlczf.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvsvbbobf.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.fanxiaobao.xyz/Article/details/gwffwfyiv.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gocfiuqdt.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwnqkdyq.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grcidmxii.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/grmlblxgl.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/giupreayz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gplkmaiex.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtxguqve.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbswhtpg.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrlnbtik.sHtML

[F06] 删除文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkrtmnrp.sHtML

Py:   os.remove("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gadvqkqok.sHtML

PHP:  unlink("a.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/gloxsybpd.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gnxfblucu.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gbrjjsbqw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmaokhbfr.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gnfphckqv.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gqksyxglk.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/gxduagtzl.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.fanxiaobao.xyz/Article/details/gixggjvhd.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpogkpkuf.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghknyrzcq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjxfqvbh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fanxiaobao.xyz/Article/details/gsuemofin.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.fanxiaobao.xyz/Article/details/ggnllzwkk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdtqhzfql.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjhuyrxr.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.fanxiaobao.xyz/Article/details/gmjyugapc.sHtML

[F08] 遍历目录
来源：http://baike.fanxiaobao.xyz/Article/details/gyimqlsex.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.fanxiaobao.xyz/Article/details/gjfiktuoo.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fanxiaobao.xyz/Article/details/grcacnylg.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkttnnvj.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.fanxiaobao.xyz/Article/details/ghlznoqpy.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtuaynkrk.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzpvlfuj.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fanxiaobao.xyz/Article/details/galakeyyx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.fanxiaobao.xyz/Article/details/grrkkofuc.sHtML

[F09] 获取文件大小
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvxfsfuq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grsjncndh.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzfdokob.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fanxiaobao.xyz/Article/details/gzoqbixkp.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fanxiaobao.xyz/Article/details/gbihlmfyn.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.fanxiaobao.xyz/Article/details/gujhaqojo.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.fanxiaobao.xyz/Article/details/gatpspmhy.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gsmsieonb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.fanxiaobao.xyz/Article/details/gnhtuivzt.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.fanxiaobao.xyz/Article/details/ghyqgozuv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gjefqtodq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/goeqlnmpv.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gnlltzwjf.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/guxtuzrmz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.fanxiaobao.xyz/Article/details/gvoupmeam.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gxksobjak.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/grluathcn.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gjciuauzk.sHtML

[F11] 复制与移动文件
来源：http://wap.fanxiaobao.xyz/Article/details/gnplcupov.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gzveweqqc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gontnguxy.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gpkitiyzh.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/glwliyffy.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.fanxiaobao.xyz/Article/details/grmndaqso.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmgczxqr.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwqnakda.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghneqmdyz.sHtML

[F12] CSV 读写
来源：http://blog.fanxiaobao.xyz/Article/details/gecywcadf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fanxiaobao.xyz/Article/details/gejjathlb.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwuwqxodf.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.fanxiaobao.xyz/Article/details/goaigqflk.sHtML

TS:   // 同上
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyuflegxm.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fanxiaobao.xyz/Article/details/guneaxoxh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.fanxiaobao.xyz/Article/details/gpznsucnt.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfxtvqph.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fanxiaobao.xyz/Article/details/gdhjdevgd.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/grxdszvno.sHtML

G. 面向对象
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwrezncv.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtreahqn.sHtML

[G01] 定义类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geetdocyx.sHtML

Py:   class User: pass
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpmgmzdk.sHtML

PHP:  class User {}
来源：http://blog.fanxiaobao.xyz/Article/details/gtsefitkh.sHtML

JS:   class User {}
来源：http://mobile.fanxiaobao.xyz/Article/details/geyxvjrow.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fanxiaobao.xyz/Article/details/gaxktqwxy.sHtML

Java: class User {}
来源：http://baike.fanxiaobao.xyz/Article/details/gxixybthh.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxumskwh.sHtML

Ruby: class User; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvyeaezf.sHtML

C#:   class User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gjwalhksy.sHtML

[G02] 构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gpynfnwpc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.fanxiaobao.xyz/Article/details/gcnrkrvra.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gboqpfvit.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnuijmboa.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gcgritack.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fanxiaobao.xyz/Article/details/glwvviybf.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fanxiaobao.xyz/Article/details/gudhhtuvk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glberwsjr.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbkpcfumi.sHtML

[G03] 实例属性
来源：http://blog.fanxiaobao.xyz/Article/details/gzkvgxdeo.sHtML

Py:   self.name = "x"
来源：http://www.share.fanxiaobao.xyz/Article/details/gqmldjwta.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fanxiaobao.xyz/Article/details/gemicodct.sHtML

JS:   this.name = "x";
来源：http://baike.fanxiaobao.xyz/Article/details/gxpekcqqo.sHtML

TS:   name: string = "x";
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvclfxsp.sHtML

Java: private String name;
来源：http://wap.fanxiaobao.xyz/Article/details/gaiwbxjjg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fanxiaobao.xyz/Article/details/gykxoarxt.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gagavigeg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.fanxiaobao.xyz/Article/details/gybzpzqnm.sHtML

[G04] 定义方法
来源：http://m.share.fanxiaobao.xyz/Article/details/gsidcvinq.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fanxiaobao.xyz/Article/details/gcfdffwsc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gkjouuovv.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/glpowztpe.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkhqeeja.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavfzccqs.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.fanxiaobao.xyz/Article/details/gbcpxdazt.sHtML

Ruby: def greet; @name; end
来源：http://wap.fanxiaobao.xyz/Article/details/gpqhbpkcr.sHtML

C#:   public string Greet() => Name;
来源：http://blog.fanxiaobao.xyz/Article/details/gdznsuuoe.sHtML

[G05] 继承
来源：http://blog.fanxiaobao.xyz/Article/details/gdovocyxu.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fanxiaobao.xyz/Article/details/gndpjxfog.sHtML

PHP:  class Admin extends User {}
来源：http://blog.fanxiaobao.xyz/Article/details/ghffzuyqy.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhfgubwd.sHtML

TS:   class Admin extends User {}
来源：http://3g.fanxiaobao.xyz/Article/details/gfxnskdvv.sHtML

Java: class Admin extends User {}
来源：http://3g.fanxiaobao.xyz/Article/details/gnfmdgfgl.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fanxiaobao.xyz/Article/details/gafwyrtyi.sHtML

Ruby: class Admin < User; end
来源：http://blog.fanxiaobao.xyz/Article/details/gzlklyibt.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsczlixpy.sHtML

[G06] 重写方法
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqwcclau.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.fanxiaobao.xyz/Article/details/gqiksuvgk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkreurqfy.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gspexysyj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrlaavch.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gbkoqjqfx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpktpfxvj.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtwzinsq.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.fanxiaobao.xyz/Article/details/gdlvhtctb.sHtML

[G07] 调用父类方法
来源：http://mobile.fanxiaobao.xyz/Article/details/gpnwlyqqk.sHtML

Py:   super().greet()
来源：http://baike.fanxiaobao.xyz/Article/details/grmyxposx.sHtML

PHP:  parent::greet();
来源：http://baike.fanxiaobao.xyz/Article/details/grzntrtgd.sHtML

JS:   super.greet();
来源：http://blog.fanxiaobao.xyz/Article/details/gfephbsrl.sHtML

TS:   super.greet();
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkkoukmm.sHtML

Java: super.greet();
来源：http://3g.fanxiaobao.xyz/Article/details/gporrkfyy.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.fanxiaobao.xyz/Article/details/gufqmdlty.sHtML

Ruby: super
来源：http://blog.fanxiaobao.xyz/Article/details/gjncpztgo.sHtML

C#:   base.Greet();
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtthjkri.sHtML

[G08] 静态方法与属性
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjqbxtml.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprhbgesq.sHtML


<!-- 参考信息 -->