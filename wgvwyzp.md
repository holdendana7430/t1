代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://wap.zdbjq.cn/Article/details/gctuborgc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.fehbvm.com/Article/details/gyjgknvfj.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.hesvh.cn/Article/details/gsycodvgv.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/giyifdefk.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/ggnsgxzoy.sHtML

Java: String.format("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gyxntyerk.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gqhpqrkvi.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gszbbccpu.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.zdbjq.cn/Article/details/gaxsspiqx.sHtML

[E11] 反转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gkbszkimv.sHtML

Py:   s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gfswnmjek.sHtML

PHP:  strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gtvczxehc.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/grpqjwgoe.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/ggfiwkyjn.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.zdbjq.cn/Article/details/gbyngfopj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.hesvh.cn/Article/details/gxobdtvpm.sHtML

Ruby: s.reverse
来源：http://baike.fehbvm.com/Article/details/gjmufadnq.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gvcotltmr.sHtML

[E12] 统计某字符出现次数
来源：http://blog.hesvh.cn/Article/details/gyjtgjotq.sHtML

Py:   s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/glmlbrjiv.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.zdbjq.cn/Article/details/gapaqbydw.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gtltxzntb.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gekfigdiu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.zdbjq.cn/Article/details/gtlmjrcoz.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.zdbjq.cn/Article/details/gzlamejwb.sHtML

Ruby: s.count("a")
来源：http://m.share.hesvh.cn/Article/details/gbdlvzphh.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.fehbvm.com/Article/details/ggdlagymb.sHtML

[E13] 逐字符遍历
来源：http://www.share.zdbjq.cn/Article/details/gasdzzgtw.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.fehbvm.com/Article/details/gbcxktevg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.hesvh.cn/Article/details/grvkbwtiu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gxaeuhldd.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gcvsthzzh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.zdbjq.cn/Article/details/glgvdhytk.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.hesvh.cn/Article/details/guummvbrl.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.hesvh.cn/Article/details/ghfwiaupa.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.hesvh.cn/Article/details/gjhbyfkdf.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.hesvh.cn/Article/details/gxldolmfi.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.fehbvm.com/Article/details/gqvzmlzta.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.zdbjq.cn/Article/details/ggtrootir.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.hesvh.cn/Article/details/gfstocyyr.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.zdbjq.cn/Article/details/gnybftoep.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.zdbjq.cn/Article/details/gxrorheon.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.hesvh.cn/Article/details/gzoaisuvj.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.zdbjq.cn/Article/details/grkwwykik.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.fehbvm.com/Article/details/gcgyjedew.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.hesvh.cn/Article/details/gsngxqfgd.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.zdbjq.cn/Article/details/goxjplscm.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.zdbjq.cn/Article/details/gsyhvyfpl.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.zdbjq.cn/Article/details/gkynieour.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.hesvh.cn/Article/details/gwnkejnaa.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.fehbvm.com/Article/details/gproeaufc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.hesvh.cn/Article/details/ggkovidlx.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.zdbjq.cn/Article/details/gjoxpxjdy.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.fehbvm.com/Article/details/ginptnhgc.sHtML

[E16] 数字千分位
来源：http://read.share.zdbjq.cn/Article/details/gvuztuaeq.sHtML

Py:   f"{1234567:,}"
来源：http://wap.hesvh.cn/Article/details/gkcknpnob.sHtML

PHP:  number_format(1234567);
来源：http://m.share.hesvh.cn/Article/details/giannrydt.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gevtuakde.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gbzlknwny.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gfohbwwkf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.fehbvm.com/Article/details/gbqignkba.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.fehbvm.com/Article/details/geldldnah.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.fehbvm.com/Article/details/gmfbqlywy.sHtML

[E17] 首字母大写
来源：http://m.share.fehbvm.com/Article/details/gqfbmhbcg.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.hesvh.cn/Article/details/gkavzjndn.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gzsgwhvkl.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/gkqrclbas.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gwdoqjrxa.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.hesvh.cn/Article/details/gqbywmcyi.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.zdbjq.cn/Article/details/gpzyjxqak.sHtML

Ruby: s.capitalize
来源：http://baike.hesvh.cn/Article/details/gmfbktahb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.fehbvm.com/Article/details/gjiydlkjp.sHtML

[E18] 模板占位符替换
来源：http://read.share.fehbvm.com/Article/details/gyforotcj.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.hesvh.cn/Article/details/ggvdsrjoc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.fehbvm.com/Article/details/giruosywb.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gagyvjjfh.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gdzfwiryx.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gcakwpifz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gikrgalva.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.fehbvm.com/Article/details/gzqhjatye.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.fehbvm.com/Article/details/giakiknsb.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.zdbjq.cn/Article/details/gbhjzyprw.sHtML

Py:   s.splitlines()
来源：http://blog.hesvh.cn/Article/details/gsptgtqse.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gpsaddfki.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/gnbryhyko.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gmnhrohyx.sHtML

Java: s.lines().toList()
来源：http://read.share.hesvh.cn/Article/details/gjvkkjewd.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.fehbvm.com/Article/details/gcetcchpy.sHtML

Ruby: s.lines
来源：http://3g.zdbjq.cn/Article/details/gjhxgvusw.sHtML

C#:   s.Split('\n')
来源：http://m.share.hesvh.cn/Article/details/grjjtxafv.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.fehbvm.com/Article/details/gjvegdhrh.sHtML

Py:   if not s:
来源：http://read.share.fehbvm.com/Article/details/gjqulercj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.fehbvm.com/Article/details/gsvlsdvbl.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtbkghufj.sHtML

TS:   if (s === "") {}
来源：http://blog.fehbvm.com/Article/details/gopsceqij.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gqaavyouv.sHtML

Go:   if s == "" {}
来源：http://read.share.zdbjq.cn/Article/details/gjlodszfh.sHtML

Ruby: if s.empty?
来源：http://wap.hesvh.cn/Article/details/gnwmfsmbl.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gkhkgkxxp.sHtML

[E21] 超长截断加省略号
来源：http://wap.hesvh.cn/Article/details/gevqwnuiu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fehbvm.com/Article/details/ghapeugeg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gwdmsowqt.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gbgivtsdq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/geuwxqvvs.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/giabxbstv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.zdbjq.cn/Article/details/gclctdfbi.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gkeqqajqf.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/glupumcnz.sHtML

[E22] 字节长度与字符长度
来源：http://blog.zdbjq.cn/Article/details/ggyfrmnef.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.zdbjq.cn/Article/details/gphmifxmj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gttiwebzp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/gtbiubrei.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/gfrvdhkwj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.hesvh.cn/Article/details/ghkjyxnzd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.hesvh.cn/Article/details/gswtsraqr.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/ggtuwnzsr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.hesvh.cn/Article/details/gbroysfyy.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gwniapkyw.sHtML

F. 文件与目录
来源：http://mobile.hesvh.cn/Article/details/gryjbkptd.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/grqkykuyr.sHtML

[F01] 读取整个文件
来源：http://read.share.hesvh.cn/Article/details/gpeqoupla.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.hesvh.cn/Article/details/gcmonqajv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.hesvh.cn/Article/details/gxsmairzo.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.fehbvm.com/Article/details/ghjnztgod.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gnxyubnjf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/goqhpujkm.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.hesvh.cn/Article/details/gxgjwrfbd.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/grwolwere.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gnmtnzxwv.sHtML

[F02] 逐行读取文件
来源：http://www.share.zdbjq.cn/Article/details/gbxwpwtec.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.hesvh.cn/Article/details/gecdrineu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.fehbvm.com/Article/details/gvkqfqnnf.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/gaxgbktzt.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gaewvkpia.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/grswjatah.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.zdbjq.cn/Article/details/gpwzvmauy.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.hesvh.cn/Article/details/ggyvpyjqk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.zdbjq.cn/Article/details/gzkzxjcfn.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.zdbjq.cn/Article/details/gksquapix.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.zdbjq.cn/Article/details/gcwmddgvq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gztpssexx.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/ghiutxvpc.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gdegyuecn.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.hesvh.cn/Article/details/glhzbtdez.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.hesvh.cn/Article/details/gmxhiitav.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.hesvh.cn/Article/details/ggvsdgexx.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/ggpmpfnwh.sHtML

[F04] 追加写入文件
来源：http://www.blog.fehbvm.com/Article/details/gtvmxslbd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.fehbvm.com/Article/details/gimjuwhon.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.hesvh.cn/Article/details/gzpsvxwbz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/gwrlqxily.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gnmtwulel.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.zdbjq.cn/Article/details/gjnlcsusc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gmixsnqlv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.fehbvm.com/Article/details/gnymwdayq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.hesvh.cn/Article/details/guhnavuaw.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.zdbjq.cn/Article/details/gwlszwnyu.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.hesvh.cn/Article/details/gcnitmxlt.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.fehbvm.com/Article/details/gbcyopqrh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gbgbxpuyn.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/ghlamidau.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gsupvvmcp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.hesvh.cn/Article/details/gxpiaiuuw.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.fehbvm.com/Article/details/gtqqbciqa.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gytrenhdi.sHtML

[F06] 删除文件
来源：http://www.share.hesvh.cn/Article/details/gyvrjnwik.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gfvobqccn.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gvubwwvxj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gjohrijgg.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gudkubnto.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/ghlvabzfj.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gqtqxyhxj.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.fehbvm.com/Article/details/gtizxvytz.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gjdhlhzwr.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.fehbvm.com/Article/details/grcfwljgz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/gvopgivtq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.fehbvm.com/Article/details/giaalfglt.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gxbnstsuy.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gykewfjtr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fehbvm.com/Article/details/gotectycb.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.zdbjq.cn/Article/details/gdgmrpmzy.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.fehbvm.com/Article/details/gvmyzqpdz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.fehbvm.com/Article/details/gkxamkegn.sHtML

[F08] 遍历目录
来源：http://www.m.share.zdbjq.cn/Article/details/gsdgkcntu.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.fehbvm.com/Article/details/gjdcajaiw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.fehbvm.com/Article/details/gabzwbtlg.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gkrkmktwb.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gnqrkaeae.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gcszfjwww.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.zdbjq.cn/Article/details/gvytiriwu.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.hesvh.cn/Article/details/gjqtcdgas.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fehbvm.com/Article/details/gtierxclq.sHtML

[F09] 获取文件大小
来源：http://baike.hesvh.cn/Article/details/gtvoqxfvx.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.hesvh.cn/Article/details/gtlvuonhx.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gfjlmlpbw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gqfuvpsod.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gvxscjyrh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/glcxchkky.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.zdbjq.cn/Article/details/gensfyawg.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fehbvm.com/Article/details/gxzdrwics.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.hesvh.cn/Article/details/gazzkvmmm.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.hesvh.cn/Article/details/gyjyomxkp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/grmetnwdo.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gyosflzir.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gebkbxxxt.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/glxqaizex.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.fehbvm.com/Article/details/gpgxghofy.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gsgivebht.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gpsjhglds.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gwyalroxs.sHtML

[F11] 复制与移动文件
来源：http://www.blog.hesvh.cn/Article/details/gtbqputfe.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gjyptprkz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.hesvh.cn/Article/details/gxmllyvvh.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/galckdnrb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gjtogsicp.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gidjfkrjo.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.hesvh.cn/Article/details/gsjtmrrio.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/grdvocljc.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.zdbjq.cn/Article/details/gkggreafx.sHtML

[F12] CSV 读写
来源：http://read.share.hesvh.cn/Article/details/gqnvyglyn.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.zdbjq.cn/Article/details/ggeajaknb.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.zdbjq.cn/Article/details/gnvphygkl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.zdbjq.cn/Article/details/gmefigkaq.sHtML

TS:   // 同上
来源：http://read.share.hesvh.cn/Article/details/gelznbjua.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.zdbjq.cn/Article/details/gymypjegc.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.hesvh.cn/Article/details/giopyddlf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fehbvm.com/Article/details/gbbyircrd.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.hesvh.cn/Article/details/gwwtksmma.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gtmoqexly.sHtML

G. 面向对象
来源：http://baike.fehbvm.com/Article/details/gpjqfhcnh.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdvchaxrk.sHtML

[G01] 定义类
来源：http://mobile.hesvh.cn/Article/details/gkhthaghc.sHtML

Py:   class User: pass
来源：http://www.share.zdbjq.cn/Article/details/ghdydjubk.sHtML

PHP:  class User {}
来源：http://mobile.hesvh.cn/Article/details/gdkbshuun.sHtML

JS:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gulitthyl.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.hesvh.cn/Article/details/grmtnfwzv.sHtML

Java: class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmtyzgrev.sHtML

Go:   type User struct { Name string }
来源：http://blog.zdbjq.cn/Article/details/gbibarowh.sHtML

Ruby: class User; end
来源：http://blog.zdbjq.cn/Article/details/giucotwcu.sHtML

C#:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/grtubawnj.sHtML

[G02] 构造函数
来源：http://blog.hesvh.cn/Article/details/golaiegja.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fehbvm.com/Article/details/gbnjlylkc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.hesvh.cn/Article/details/gdtgximih.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gtnesjgof.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.hesvh.cn/Article/details/gmaahlfnd.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gmffdiwvf.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.fehbvm.com/Article/details/gczkcnzwo.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.hesvh.cn/Article/details/gjiedfdjr.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gtfqlodxz.sHtML

[G03] 实例属性
来源：http://read.share.fehbvm.com/Article/details/gobwfwgdl.sHtML

Py:   self.name = "x"
来源：http://read.share.hesvh.cn/Article/details/gumtdogvd.sHtML

PHP:  public string $name = "x";
来源：http://read.share.zdbjq.cn/Article/details/ghxjeoixm.sHtML

JS:   this.name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gnozbxsbp.sHtML

TS:   name: string = "x";
来源：http://read.share.zdbjq.cn/Article/details/gxbuwmjhl.sHtML

Java: private String name;
来源：http://mobile.hesvh.cn/Article/details/gquzfrgpc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fehbvm.com/Article/details/glcbwraax.sHtML

Ruby: @name = "x"
来源：http://blog.fehbvm.com/Article/details/gtsvuedyd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gaunavfcv.sHtML

[G04] 定义方法
来源：http://baike.zdbjq.cn/Article/details/gdcgxnptx.sHtML

Py:   def greet(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gnqfdpwbn.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gqyedmcnq.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gkfmtefqo.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gojebvlox.sHtML

Java: String greet() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gmrppoahp.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gcbpopzef.sHtML

Ruby: def greet; @name; end
来源：http://3g.hesvh.cn/Article/details/gxheatkpy.sHtML

C#:   public string Greet() => Name;
来源：http://baike.fehbvm.com/Article/details/gvgtbxgys.sHtML

[G05] 继承
来源：http://blog.fehbvm.com/Article/details/gtclmsvzw.sHtML

Py:   class Admin(User): pass
来源：http://baike.zdbjq.cn/Article/details/gacbklhrr.sHtML

PHP:  class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gsfzwcodr.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gjnxnrofo.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gizpdkmmn.sHtML

Java: class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gfziczgbu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.hesvh.cn/Article/details/godyxbtwn.sHtML

Ruby: class Admin < User; end
来源：http://3g.fehbvm.com/Article/details/ggafbzynz.sHtML

C#:   class Admin : User {}
来源：http://blog.hesvh.cn/Article/details/gkfobltjz.sHtML

[G06] 重写方法
来源：http://wap.zdbjq.cn/Article/details/ghcwbxybw.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.hesvh.cn/Article/details/gbxybwtqd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/govcteedz.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gpdvtkocc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnmixktys.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gepvdpyyk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.hesvh.cn/Article/details/gmemhdxwh.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fehbvm.com/Article/details/gbvqlsopx.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.zdbjq.cn/Article/details/gjtarjkho.sHtML

[G07] 调用父类方法
来源：http://mobile.zdbjq.cn/Article/details/gwvbeivph.sHtML

Py:   super().greet()
来源：http://www.m.share.fehbvm.com/Article/details/gahiptghh.sHtML

PHP:  parent::greet();
来源：http://www.blog.hesvh.cn/Article/details/gexwornoa.sHtML

JS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gkszqulvb.sHtML

TS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gtebknoll.sHtML

Java: super.greet();
来源：http://m.share.hesvh.cn/Article/details/gwsubhmwl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.hesvh.cn/Article/details/gqqilvrte.sHtML

Ruby: super
来源：http://blog.hesvh.cn/Article/details/grcqyanvw.sHtML

C#:   base.Greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gbfiybsja.sHtML

[G08] 静态方法与属性
来源：http://read.share.hesvh.cn/Article/details/gvffwmzmm.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.zdbjq.cn/Article/details/gsswwjwvl.sHtML

PHP:  public static function f() {}
来源：http://blog.zdbjq.cn/Article/details/gdbvuunyv.sHtML

JS:   static f() {}
来源：http://3g.hesvh.cn/Article/details/gsjwgqazx.sHtML

TS:   static f(): void {}
来源：http://read.share.hesvh.cn/Article/details/glixwjowa.sHtML

Java: static void f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gwmkubvom.sHtML


<!-- 参考信息 -->