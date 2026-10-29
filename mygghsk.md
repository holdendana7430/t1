代发 wailian999

Go:   strings.Join(items, ",")
来源：http://wap.hesvh.cn/Article/details/gjwncwkbf.sHtML

Ruby: items.join(",")
来源：http://3g.hesvh.cn/Article/details/gvwiozemj.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/glnuqpgmp.sHtML

[E09] 去除所有空白字符
来源：http://mobile.fehbvm.com/Article/details/gwkzitpqv.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.hesvh.cn/Article/details/genmmsrsn.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fehbvm.com/Article/details/gljkgvvlq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/grhhgkpkr.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/gzbmlzitw.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.hesvh.cn/Article/details/gjiikyqve.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.zdbjq.cn/Article/details/gronzztkm.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.zdbjq.cn/Article/details/geclmrsoo.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.hesvh.cn/Article/details/gchdwuzvh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.hesvh.cn/Article/details/gkajpxexk.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gogosmxhx.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fehbvm.com/Article/details/gkxkqqjqs.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gppkvqorj.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gvyvgxryw.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gylnxjsml.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gzswcrkkr.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/grqltvcit.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.hesvh.cn/Article/details/gbwlxhtyq.sHtML

[E11] 反转字符串
来源：http://www.m.share.hesvh.cn/Article/details/ghztfoveo.sHtML

Py:   s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/gkapjcjws.sHtML

PHP:  strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/gcugbnmyc.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gdtsmbkpu.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/grfwfovpa.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.hesvh.cn/Article/details/gwiwtazil.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.fehbvm.com/Article/details/gmawctugu.sHtML

Ruby: s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gqxgclxkb.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gxdmyeimo.sHtML

[E12] 统计某字符出现次数
来源：http://blog.fehbvm.com/Article/details/gdvhvnqxr.sHtML

Py:   s.count("a")
来源：http://baike.hesvh.cn/Article/details/gowcnyyfc.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.hesvh.cn/Article/details/gpyedbgmi.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gzfnxojfz.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gpogdvatl.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.fehbvm.com/Article/details/gdtwilvfq.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.fehbvm.com/Article/details/gifsbxksy.sHtML

Ruby: s.count("a")
来源：http://blog.hesvh.cn/Article/details/gozncdbxq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.fehbvm.com/Article/details/giairojyh.sHtML

[E13] 逐字符遍历
来源：http://mobile.zdbjq.cn/Article/details/ggoovnuhl.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.hesvh.cn/Article/details/gjnmeydoq.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.hesvh.cn/Article/details/ghwwmgzwo.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/ginepkxnv.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gvbgrhprs.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gfeosjvia.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gkzrlhlbx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.hesvh.cn/Article/details/gbqtxbtxx.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.hesvh.cn/Article/details/gkpyjdtxc.sHtML

[E14] URL 编码与 Base64
来源：http://3g.fehbvm.com/Article/details/gcnhgpimn.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.zdbjq.cn/Article/details/gxsbhpqlv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.fehbvm.com/Article/details/gmujvywqi.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.hesvh.cn/Article/details/gomqqudee.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.hesvh.cn/Article/details/ggdsvojkm.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.hesvh.cn/Article/details/gexmodseb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.fehbvm.com/Article/details/grfkyfypy.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.zdbjq.cn/Article/details/gyfuikgfl.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.hesvh.cn/Article/details/gmxzfjbgt.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.zdbjq.cn/Article/details/gmhdvywak.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.zdbjq.cn/Article/details/gowpaounu.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.zdbjq.cn/Article/details/gkshafpyw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.fehbvm.com/Article/details/goshboudl.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.fehbvm.com/Article/details/gadtxgngu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.fehbvm.com/Article/details/gmbnsdsvp.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.hesvh.cn/Article/details/gkhowfkpk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.hesvh.cn/Article/details/gdhgfwmtd.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.fehbvm.com/Article/details/ggistwpzl.sHtML

[E16] 数字千分位
来源：http://www.blog.fehbvm.com/Article/details/genntpkwz.sHtML

Py:   f"{1234567:,}"
来源：http://blog.fehbvm.com/Article/details/gmstiuzbn.sHtML

PHP:  number_format(1234567);
来源：http://baike.fehbvm.com/Article/details/gwbehurgu.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/glzrwvgmq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/grqmltgly.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.fehbvm.com/Article/details/gwelvnzvq.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.hesvh.cn/Article/details/gvhvcxcfc.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.zdbjq.cn/Article/details/glfpqhdzy.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.fehbvm.com/Article/details/gszatbzlw.sHtML

[E17] 首字母大写
来源：http://baike.zdbjq.cn/Article/details/gffnxpucn.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.hesvh.cn/Article/details/gwnxoevdj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.hesvh.cn/Article/details/gowvaaarx.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/gwwrfdagi.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gztfyngio.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fehbvm.com/Article/details/goqcktuvy.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.fehbvm.com/Article/details/gaixvhgpj.sHtML

Ruby: s.capitalize
来源：http://www.m.share.hesvh.cn/Article/details/gprotdbnm.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.zdbjq.cn/Article/details/gibzgofsj.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fehbvm.com/Article/details/gbgibkqwr.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.zdbjq.cn/Article/details/gqcowoqrp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.zdbjq.cn/Article/details/gztomftwp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gegitymsx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gcbiswsve.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gjkruydhp.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gjhgegghn.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.fehbvm.com/Article/details/gzblblvfn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.hesvh.cn/Article/details/gpkmtckzf.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.fehbvm.com/Article/details/gkaoonazi.sHtML

Py:   s.splitlines()
来源：http://3g.fehbvm.com/Article/details/ggjlsypai.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gfngirzls.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gnbgvfpgd.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/gnfdbizmo.sHtML

Java: s.lines().toList()
来源：http://3g.zdbjq.cn/Article/details/gdsqoffje.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.zdbjq.cn/Article/details/gwieifpot.sHtML

Ruby: s.lines
来源：http://www.share.zdbjq.cn/Article/details/glnqsvklq.sHtML

C#:   s.Split('\n')
来源：http://mobile.fehbvm.com/Article/details/giygudrpl.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.zdbjq.cn/Article/details/glijsswxj.sHtML

Py:   if not s:
来源：http://www.share.zdbjq.cn/Article/details/gxffqylnf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.hesvh.cn/Article/details/goyrdljnm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.fehbvm.com/Article/details/gdqetrqcy.sHtML

TS:   if (s === "") {}
来源：http://blog.zdbjq.cn/Article/details/gaxccwost.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/geyefatok.sHtML

Go:   if s == "" {}
来源：http://m.share.zdbjq.cn/Article/details/gmhfxklll.sHtML

Ruby: if s.empty?
来源：http://m.share.fehbvm.com/Article/details/guzudnpnj.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gkutcmxww.sHtML

[E21] 超长截断加省略号
来源：http://www.share.hesvh.cn/Article/details/gevttbala.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.zdbjq.cn/Article/details/gfmjslhyu.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gvxkclojt.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/ggveqpfap.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gvpyqpfui.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/ghbngavql.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.zdbjq.cn/Article/details/grzfexeml.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gnyadcgxt.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/glaikqlxk.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fehbvm.com/Article/details/gyfejhpsm.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.zdbjq.cn/Article/details/gcuduxvwb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gllsjgppk.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/guuicuyof.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gozdnvkgg.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gqevlwvuh.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.zdbjq.cn/Article/details/gctbggrdm.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fehbvm.com/Article/details/guvokaapx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gayusceqt.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/goorvwolv.sHtML

F. 文件与目录
来源：http://blog.fehbvm.com/Article/details/gzhdlerlw.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gkqahynee.sHtML

[F01] 读取整个文件
来源：http://baike.zdbjq.cn/Article/details/gpmhkigtp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.hesvh.cn/Article/details/gpbgayypi.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gamgnitav.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.fehbvm.com/Article/details/gbfwafuyg.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gscpwxxfy.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gvvbbbdfn.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.zdbjq.cn/Article/details/gmkrnjcyy.sHtML

Ruby: File.read("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gnimdluej.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gxuzhvifx.sHtML

[F02] 逐行读取文件
来源：http://baike.hesvh.cn/Article/details/gkyxdqdvg.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.zdbjq.cn/Article/details/gafxqqdvy.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.fehbvm.com/Article/details/glohnbkem.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/gdylxpnhq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gmzqqqaqy.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/gayigwfba.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.zdbjq.cn/Article/details/gcubxrxrj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.fehbvm.com/Article/details/gstdpggqz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.fehbvm.com/Article/details/gzxibyhya.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.zdbjq.cn/Article/details/ggoxzszzk.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.zdbjq.cn/Article/details/gymwnzrwz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gamnjlkye.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/grkoztqou.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gufacsdnq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.fehbvm.com/Article/details/gyitqjvvc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.zdbjq.cn/Article/details/giyoprqbu.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gxiztzzrs.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gkihlvefp.sHtML

[F04] 追加写入文件
来源：http://wap.fehbvm.com/Article/details/gmqgdejiu.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.hesvh.cn/Article/details/ggldrrjrd.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.zdbjq.cn/Article/details/gvksdwfvs.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/gftowefgo.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/gcnrtnjxw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.hesvh.cn/Article/details/ggldoqgxg.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.hesvh.cn/Article/details/gbxdrfyxc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fehbvm.com/Article/details/gmjlxspwq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fehbvm.com/Article/details/gmtckyasi.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.hesvh.cn/Article/details/gpoqbmqha.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.hesvh.cn/Article/details/gygpakqab.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.hesvh.cn/Article/details/geytftbar.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gjmhfafnh.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/glazfzogf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gwxvvmezo.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fehbvm.com/Article/details/gcqctgcba.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.hesvh.cn/Article/details/glbbqonca.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.hesvh.cn/Article/details/gkiptduyu.sHtML

[F06] 删除文件
来源：http://m.share.fehbvm.com/Article/details/gndfmcgdx.sHtML

Py:   os.remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/ghzfdetaz.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fehbvm.com/Article/details/gjltelrjy.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/grpktjaqt.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gwczpwxhu.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/ggkkywvro.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/goavvojey.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gtqjtlidz.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gmyfcpdgi.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.hesvh.cn/Article/details/gpeqqerke.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/gvqgkrnjo.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.hesvh.cn/Article/details/gyekezjuh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gnmocpkay.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/glwlsxbbf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.zdbjq.cn/Article/details/glcnusoka.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fehbvm.com/Article/details/ghcmdbezb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.hesvh.cn/Article/details/gvinbmxgo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fehbvm.com/Article/details/ggavonhho.sHtML

[F08] 遍历目录
来源：http://wap.hesvh.cn/Article/details/gmnxddlwj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.fehbvm.com/Article/details/gikfuvydk.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.fehbvm.com/Article/details/gxpfafypx.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/gdacxwaqd.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gwkkfvtaq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/grchbecur.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.hesvh.cn/Article/details/gvrvnafct.sHtML

Ruby: Dir.children("dir")
来源：http://wap.hesvh.cn/Article/details/gmfbeywqp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gegbhbdlg.sHtML

[F09] 获取文件大小
来源：http://baike.hesvh.cn/Article/details/gmwvamsja.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.hesvh.cn/Article/details/ghefmfrcv.sHtML

PHP:  filesize("a.txt");
来源：http://blog.zdbjq.cn/Article/details/ghtkrzujf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gpewvqjbb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gfzrtjbif.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gxffoiqna.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.fehbvm.com/Article/details/gczgihsju.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.hesvh.cn/Article/details/ghzivjptg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.fehbvm.com/Article/details/gbdhbcrjd.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.zdbjq.cn/Article/details/gzjowzjoc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gtyskeiit.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.hesvh.cn/Article/details/ggfcxvvqw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/ggghabiey.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gedfksnzg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.hesvh.cn/Article/details/gzcqoidsk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/glbsqlxtt.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/ggbgkswrd.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gfqcfykpo.sHtML

[F11] 复制与移动文件
来源：http://wap.fehbvm.com/Article/details/gczauymoq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gkargrbju.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.zdbjq.cn/Article/details/gvtsvayxs.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gnmzzzzoj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gwlsdiubq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.hesvh.cn/Article/details/ggesltnug.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.zdbjq.cn/Article/details/gbhnkusmh.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/govbfpspv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.hesvh.cn/Article/details/gufydxcnn.sHtML

[F12] CSV 读写
来源：http://baike.fehbvm.com/Article/details/gwmggljdt.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.hesvh.cn/Article/details/gsqpxgbgl.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.hesvh.cn/Article/details/gsjirlfbs.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.zdbjq.cn/Article/details/gjbjeydxf.sHtML

TS:   // 同上
来源：http://read.share.hesvh.cn/Article/details/gwywcmmvz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fehbvm.com/Article/details/gxkyxmjhy.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.hesvh.cn/Article/details/gvinhacxf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.hesvh.cn/Article/details/gtmxldcot.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fehbvm.com/Article/details/gxdzurcde.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxowidqxh.sHtML

G. 面向对象
来源：http://m.share.fehbvm.com/Article/details/ggcsedpwc.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gdxwixxyl.sHtML

[G01] 定义类
来源：http://www.m.share.zdbjq.cn/Article/details/gydytqqve.sHtML

Py:   class User: pass
来源：http://www.blog.fehbvm.com/Article/details/gfaucpord.sHtML

PHP:  class User {}
来源：http://3g.zdbjq.cn/Article/details/gjyuxfchl.sHtML

JS:   class User {}
来源：http://wap.hesvh.cn/Article/details/ghqrbqgjd.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.zdbjq.cn/Article/details/gftckqtfa.sHtML

Java: class User {}
来源：http://read.share.fehbvm.com/Article/details/gjwnnqoym.sHtML

Go:   type User struct { Name string }
来源：http://wap.fehbvm.com/Article/details/gobmkrhit.sHtML

Ruby: class User; end
来源：http://wap.fehbvm.com/Article/details/gbrlljvbj.sHtML

C#:   class User {}
来源：http://3g.hesvh.cn/Article/details/glcsfuind.sHtML

[G02] 构造函数
来源：http://blog.zdbjq.cn/Article/details/gpsdpfctq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.hesvh.cn/Article/details/gueococfu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.hesvh.cn/Article/details/gvxitcqen.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gmuvryshy.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.zdbjq.cn/Article/details/ghztqmytt.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gakokudxg.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fehbvm.com/Article/details/goynvaywk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.fehbvm.com/Article/details/gbxrahjwi.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.hesvh.cn/Article/details/gzwjwjadr.sHtML

[G03] 实例属性
来源：http://read.share.fehbvm.com/Article/details/gdwojwjec.sHtML

Py:   self.name = "x"
来源：http://www.share.hesvh.cn/Article/details/gusxpnxnk.sHtML

PHP:  public string $name = "x";
来源：http://wap.zdbjq.cn/Article/details/gmpdtvoky.sHtML

JS:   this.name = "x";
来源：http://www.share.hesvh.cn/Article/details/gbdzifomn.sHtML

TS:   name: string = "x";
来源：http://wap.zdbjq.cn/Article/details/gbgjrqzbz.sHtML

Java: private String name;
来源：http://www.blog.zdbjq.cn/Article/details/gergxxzpr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.hesvh.cn/Article/details/gajtsqlkc.sHtML

Ruby: @name = "x"
来源：http://mobile.zdbjq.cn/Article/details/glqsnntew.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.fehbvm.com/Article/details/gnbewqqix.sHtML

[G04] 定义方法
来源：http://blog.hesvh.cn/Article/details/gcvmcixdw.sHtML

Py:   def greet(self): return self.name
来源：http://blog.hesvh.cn/Article/details/ggqosoxfw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gpicwgzob.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gnnkonlnm.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gluhhtwio.sHtML

Java: String greet() { return name; }
来源：http://www.share.fehbvm.com/Article/details/ghbofkywk.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gmjxgiybk.sHtML

Ruby: def greet; @name; end
来源：http://read.share.hesvh.cn/Article/details/gzxzadbfy.sHtML

C#:   public string Greet() => Name;
来源：http://wap.zdbjq.cn/Article/details/gcakrnexe.sHtML

[G05] 继承
来源：http://m.share.fehbvm.com/Article/details/ggxbueanx.sHtML

Py:   class Admin(User): pass
来源：http://mobile.fehbvm.com/Article/details/genptckwf.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gwfqjriyv.sHtML

JS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/ghhajbmft.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/ggomxyeha.sHtML

Java: class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/ggdnuqctq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.hesvh.cn/Article/details/goyvepoid.sHtML

Ruby: class Admin < User; end
来源：http://3g.fehbvm.com/Article/details/gdwltzcyp.sHtML

C#:   class Admin : User {}
来源：http://baike.fehbvm.com/Article/details/grhezcwih.sHtML

[G06] 重写方法
来源：http://baike.fehbvm.com/Article/details/gdyebxysr.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.zdbjq.cn/Article/details/gublgkcwx.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gptgtddpo.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gigbzfysh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gqyiamsle.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gucotrlxb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.hesvh.cn/Article/details/gnjfgvrhq.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.zdbjq.cn/Article/details/gmylfwysn.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.zdbjq.cn/Article/details/gjldaoopz.sHtML

[G07] 调用父类方法
来源：http://mobile.hesvh.cn/Article/details/glbbyxizj.sHtML

Py:   super().greet()
来源：http://3g.hesvh.cn/Article/details/gfycrlfzz.sHtML

PHP:  parent::greet();
来源：http://wap.zdbjq.cn/Article/details/getrykmhr.sHtML


<!-- 参考信息 -->