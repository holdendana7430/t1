代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gxunoktkq.sHtML

Java: String.format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gfkkkevtt.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gjjpzlimp.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gwayimbxn.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.hesvh.cn/Article/details/gkcevhbty.sHtML

[E11] 反转字符串
来源：http://3g.zdbjq.cn/Article/details/ggffuvmqk.sHtML

Py:   s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gmwrizszs.sHtML

PHP:  strrev($s);
来源：http://read.share.hesvh.cn/Article/details/glvvcxadb.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gotqpvknd.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gihqrigox.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.hesvh.cn/Article/details/gjjrrvyei.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gripnjuwr.sHtML

Ruby: s.reverse
来源：http://www.share.hesvh.cn/Article/details/gwzmawyoy.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gjhqhkrkw.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.zdbjq.cn/Article/details/gqqahoehp.sHtML

Py:   s.count("a")
来源：http://read.share.hesvh.cn/Article/details/gytxcbviy.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.hesvh.cn/Article/details/gbgkncwcn.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/gxusvnngd.sHtML

TS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gtbjsjinv.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.hesvh.cn/Article/details/gtlewcmrx.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.fehbvm.com/Article/details/gtbbmwjsr.sHtML

Ruby: s.count("a")
来源：http://baike.fehbvm.com/Article/details/gwbsxatgf.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.hesvh.cn/Article/details/gtckahogz.sHtML

[E13] 逐字符遍历
来源：http://3g.zdbjq.cn/Article/details/gnkwdwrpy.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.hesvh.cn/Article/details/grsamfhvd.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.fehbvm.com/Article/details/gawfazqci.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/gxsjljvdl.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/gzqofzedw.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.fehbvm.com/Article/details/ggadbarnr.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.zdbjq.cn/Article/details/grczsepya.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.fehbvm.com/Article/details/gandatbvi.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.zdbjq.cn/Article/details/grviiqgwn.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.fehbvm.com/Article/details/gsgaeltog.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fehbvm.com/Article/details/gucpgvdqb.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.zdbjq.cn/Article/details/guakxfrvq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.hesvh.cn/Article/details/gqvwdofxv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gtgcaiwjl.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.hesvh.cn/Article/details/gqcnlkqmk.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.zdbjq.cn/Article/details/gueidgamj.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.fehbvm.com/Article/details/gpczerfcu.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.zdbjq.cn/Article/details/ggotfmoxh.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.hesvh.cn/Article/details/gpngvrqxq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.zdbjq.cn/Article/details/gffbmadoa.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.hesvh.cn/Article/details/gccyjuqza.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.hesvh.cn/Article/details/gtvxtpavb.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.fehbvm.com/Article/details/gafdsxtge.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.hesvh.cn/Article/details/gavtjprcx.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.fehbvm.com/Article/details/gvszzidtq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.hesvh.cn/Article/details/gfwspduaq.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.zdbjq.cn/Article/details/guwywjlzo.sHtML

[E16] 数字千分位
来源：http://3g.zdbjq.cn/Article/details/gouwvqehu.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.fehbvm.com/Article/details/grhqmythz.sHtML

PHP:  number_format(1234567);
来源：http://m.share.zdbjq.cn/Article/details/gbltzffav.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/gkzklgkmg.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/gdkojtkss.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.fehbvm.com/Article/details/gxpmmrkyn.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.fehbvm.com/Article/details/gvwttvsnq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.zdbjq.cn/Article/details/gmeprwotb.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.fehbvm.com/Article/details/ghvovmxun.sHtML

[E17] 首字母大写
来源：http://mobile.hesvh.cn/Article/details/goekzlevc.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.zdbjq.cn/Article/details/gmsatpqwl.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.hesvh.cn/Article/details/gplqeisbk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/glvnidtxd.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/ghowecxeg.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.fehbvm.com/Article/details/gldwkjhze.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.hesvh.cn/Article/details/ggsdyixmp.sHtML

Ruby: s.capitalize
来源：http://www.blog.hesvh.cn/Article/details/gtrnomdap.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.hesvh.cn/Article/details/gnetkmzxk.sHtML

[E18] 模板占位符替换
来源：http://www.share.fehbvm.com/Article/details/gkenciqep.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.hesvh.cn/Article/details/ghglatpmy.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.hesvh.cn/Article/details/gievzgqdy.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/geyexivpt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gwefzbvbt.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gkhylmnpc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gdugngpoz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.hesvh.cn/Article/details/ghwbdvexy.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.hesvh.cn/Article/details/gqjhhorxk.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fehbvm.com/Article/details/giaoecvai.sHtML

Py:   s.splitlines()
来源：http://mobile.zdbjq.cn/Article/details/gjigujabl.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.zdbjq.cn/Article/details/gwvbhnjef.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/ghmqottdq.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gifsjpuan.sHtML

Java: s.lines().toList()
来源：http://baike.hesvh.cn/Article/details/gmbhditxl.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.zdbjq.cn/Article/details/goxunktas.sHtML

Ruby: s.lines
来源：http://blog.zdbjq.cn/Article/details/gibijzkbn.sHtML

C#:   s.Split('\n')
来源：http://baike.fehbvm.com/Article/details/gbfitqliu.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.fehbvm.com/Article/details/gyemdrnyx.sHtML

Py:   if not s:
来源：http://3g.fehbvm.com/Article/details/gksqpzqzp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.fehbvm.com/Article/details/gtzazanvv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwzejincn.sHtML

TS:   if (s === "") {}
来源：http://m.share.zdbjq.cn/Article/details/giawvpbxm.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/glrgxzwhq.sHtML

Go:   if s == "" {}
来源：http://mobile.hesvh.cn/Article/details/goaekvhum.sHtML

Ruby: if s.empty?
来源：http://read.share.zdbjq.cn/Article/details/ghmelqnko.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.zdbjq.cn/Article/details/gzmbxlxmu.sHtML

[E21] 超长截断加省略号
来源：http://blog.hesvh.cn/Article/details/gtnhazvfy.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.hesvh.cn/Article/details/gxdzyyufo.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gjzfobskp.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/ghitklojt.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gmdnwkabg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gocuveled.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.hesvh.cn/Article/details/ghivklvif.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gdnianxes.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gpflvcgyx.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.hesvh.cn/Article/details/gxmeprfur.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.zdbjq.cn/Article/details/gvnkvwldc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gxfmrjcdr.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gzenitsps.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/gmkolnobk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gxndguivi.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.hesvh.cn/Article/details/gscndmcxz.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gcxaokqck.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gykzycjqi.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/goaecwizv.sHtML

F. 文件与目录
来源：http://www.share.zdbjq.cn/Article/details/gplxbehru.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gqmikbqwo.sHtML

[F01] 读取整个文件
来源：http://wap.hesvh.cn/Article/details/gdginmwob.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.fehbvm.com/Article/details/gpizlrmeb.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gkgwlzsga.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.zdbjq.cn/Article/details/gicahrsdu.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.hesvh.cn/Article/details/gajhumfxr.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gdspbmkdc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.fehbvm.com/Article/details/gssfpnxbt.sHtML

Ruby: File.read("a.txt")
来源：http://baike.fehbvm.com/Article/details/gaymtzevx.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gomrrpmxb.sHtML

[F02] 逐行读取文件
来源：http://wap.zdbjq.cn/Article/details/gcmnmygxm.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.zdbjq.cn/Article/details/glbrzscdw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.zdbjq.cn/Article/details/gjjxlsgee.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gyswhwcyp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gudujohim.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gjwseytmz.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.zdbjq.cn/Article/details/gzhnuvccl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.zdbjq.cn/Article/details/grfuhosrr.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.hesvh.cn/Article/details/gvgjrrqlo.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.zdbjq.cn/Article/details/gkrusvmpb.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.zdbjq.cn/Article/details/gkxmsxoqm.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gzskejtvf.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/glfvotjla.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/gdzjhmzyp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.hesvh.cn/Article/details/gcvbkqafs.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.zdbjq.cn/Article/details/gopqoirwt.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gwcukxche.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/ggxhjigcy.sHtML

[F04] 追加写入文件
来源：http://www.m.share.fehbvm.com/Article/details/gulekglla.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.fehbvm.com/Article/details/gdtbhbxbn.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.zdbjq.cn/Article/details/gijgditxr.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/gwtkcsoyd.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/gpizfjyfl.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.hesvh.cn/Article/details/gegybzvgx.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gowumqcpb.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.hesvh.cn/Article/details/gtrmdmovx.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.hesvh.cn/Article/details/gqtbvfkab.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.hesvh.cn/Article/details/gbdurtymw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.fehbvm.com/Article/details/gngslyvyc.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gbglcklhu.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gykrjsrob.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gnhdorueo.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gsswkouab.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.zdbjq.cn/Article/details/gcieqpbax.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gzbdftkqy.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gxgwixlxa.sHtML

[F06] 删除文件
来源：http://www.blog.hesvh.cn/Article/details/gjoombqlw.sHtML

Py:   os.remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gojboibdf.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.hesvh.cn/Article/details/guwcbrzpb.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gcmqfhbxs.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gnnhvrgrc.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gfzybgsmi.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gntpvgctc.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gzbobqyng.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/grezqhhkh.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.zdbjq.cn/Article/details/gwoqvxodg.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/grzncxmdt.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.hesvh.cn/Article/details/ganqjddfl.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/ghuzmxjhm.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/gdckbbasr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fehbvm.com/Article/details/gpdvwmqwn.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.fehbvm.com/Article/details/gbdookvkp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.fehbvm.com/Article/details/gvcfwofsv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.fehbvm.com/Article/details/gtmgdbewy.sHtML

[F08] 遍历目录
来源：http://www.share.hesvh.cn/Article/details/gxfwqflft.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.hesvh.cn/Article/details/ggsqcwchb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.zdbjq.cn/Article/details/gdffyzwel.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/ggebofhoy.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gjadwtjvf.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gnauljdpk.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.fehbvm.com/Article/details/gakodgars.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.zdbjq.cn/Article/details/gcuqnyelk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.fehbvm.com/Article/details/gceowavql.sHtML

[F09] 获取文件大小
来源：http://read.share.fehbvm.com/Article/details/gpjuydncv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gebwtufzg.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.hesvh.cn/Article/details/glozopvue.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gxweyvohe.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gqwuwuzbw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gnbakdzbb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.hesvh.cn/Article/details/gpxyvzjdx.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gtzervrsk.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.zdbjq.cn/Article/details/ggrxtfyda.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.hesvh.cn/Article/details/gxvilirei.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gcrcgezyf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.hesvh.cn/Article/details/gfnshxlvu.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/geyqvbcor.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gqliedwty.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.zdbjq.cn/Article/details/gppdoezee.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gprgjnubs.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gpaypqjbt.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gxghkhvsf.sHtML

[F11] 复制与移动文件
来源：http://3g.zdbjq.cn/Article/details/guvdfmjrr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/giidhxkvt.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.hesvh.cn/Article/details/gsqzvccts.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/ggogduvnd.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gydjqsfbt.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gogcjqsfk.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.hesvh.cn/Article/details/gyojqyjhr.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gzdcljvvt.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.hesvh.cn/Article/details/gphooabha.sHtML

[F12] CSV 读写
来源：http://blog.zdbjq.cn/Article/details/gcvxnpsvm.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.zdbjq.cn/Article/details/gudrwdbzn.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.hesvh.cn/Article/details/gmdhmkwrj.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.fehbvm.com/Article/details/gsyjunkxi.sHtML

TS:   // 同上
来源：http://m.share.fehbvm.com/Article/details/gpqoccxph.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.zdbjq.cn/Article/details/ghsgojzgv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.zdbjq.cn/Article/details/gsaqyxodo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.zdbjq.cn/Article/details/gwvdophls.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.hesvh.cn/Article/details/grmgqzxrq.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gtoepwtie.sHtML

G. 面向对象
来源：http://blog.fehbvm.com/Article/details/gqutdlcoa.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxvkodjcn.sHtML

[G01] 定义类
来源：http://read.share.zdbjq.cn/Article/details/gukdjyrec.sHtML

Py:   class User: pass
来源：http://read.share.zdbjq.cn/Article/details/gicmsukky.sHtML

PHP:  class User {}
来源：http://www.share.zdbjq.cn/Article/details/gaisaorzs.sHtML

JS:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gouoqdwfk.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fehbvm.com/Article/details/gajppfecb.sHtML

Java: class User {}
来源：http://www.share.fehbvm.com/Article/details/gywofrlen.sHtML

Go:   type User struct { Name string }
来源：http://3g.fehbvm.com/Article/details/gtythvhvu.sHtML

Ruby: class User; end
来源：http://www.m.share.fehbvm.com/Article/details/gjmterwsy.sHtML

C#:   class User {}
来源：http://wap.hesvh.cn/Article/details/ggowidgtf.sHtML

[G02] 构造函数
来源：http://blog.zdbjq.cn/Article/details/gpwttsgwe.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.zdbjq.cn/Article/details/gprtqomls.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.zdbjq.cn/Article/details/gnfleskpd.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gweiulniu.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.hesvh.cn/Article/details/gubytfzud.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gmoqdstig.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fehbvm.com/Article/details/gephyubqq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.hesvh.cn/Article/details/glpzkyulo.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.hesvh.cn/Article/details/gppzyidqu.sHtML

[G03] 实例属性
来源：http://read.share.zdbjq.cn/Article/details/gydcltqcq.sHtML

Py:   self.name = "x"
来源：http://baike.zdbjq.cn/Article/details/gpswbtfli.sHtML

PHP:  public string $name = "x";
来源：http://www.share.zdbjq.cn/Article/details/giyhlstza.sHtML

JS:   this.name = "x";
来源：http://wap.zdbjq.cn/Article/details/gutsgioar.sHtML

TS:   name: string = "x";
来源：http://www.share.zdbjq.cn/Article/details/ggyxxdbkg.sHtML

Java: private String name;
来源：http://www.blog.zdbjq.cn/Article/details/gcvfyyyhi.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.hesvh.cn/Article/details/ggeliomia.sHtML

Ruby: @name = "x"
来源：http://baike.zdbjq.cn/Article/details/gwgsfmgjz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.fehbvm.com/Article/details/gygrzoeum.sHtML

[G04] 定义方法
来源：http://read.share.hesvh.cn/Article/details/giknkznlu.sHtML

Py:   def greet(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gcuczwcrt.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/glojkzfef.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gitalvvom.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/geroeeznz.sHtML

Java: String greet() { return name; }
来源：http://blog.fehbvm.com/Article/details/gkcuuipau.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gimbjjvjb.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/ggpudbzcv.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gjphoyhow.sHtML

[G05] 继承
来源：http://www.blog.hesvh.cn/Article/details/gsvdejhmc.sHtML

Py:   class Admin(User): pass
来源：http://read.share.zdbjq.cn/Article/details/gvuiqjrip.sHtML

PHP:  class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gqpsxlgst.sHtML

JS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/girlnrhbq.sHtML

TS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gahqinuxz.sHtML

Java: class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gveifvsqy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fehbvm.com/Article/details/gnqrrdunt.sHtML

Ruby: class Admin < User; end
来源：http://wap.zdbjq.cn/Article/details/gepxkfikf.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.hesvh.cn/Article/details/gtcfuevuf.sHtML

[G06] 重写方法
来源：http://mobile.hesvh.cn/Article/details/gdlltrbgd.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.zdbjq.cn/Article/details/gzfrictzp.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gdmgkbgyo.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gbslavrqn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gtdzxklxc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gdlhvslps.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.hesvh.cn/Article/details/gsqrgrlib.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fehbvm.com/Article/details/gnucwpzzv.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.hesvh.cn/Article/details/gilxddjzd.sHtML

[G07] 调用父类方法
来源：http://mobile.fehbvm.com/Article/details/gvvddrdfz.sHtML

Py:   super().greet()
来源：http://baike.hesvh.cn/Article/details/guztxpjpi.sHtML

PHP:  parent::greet();
来源：http://www.blog.hesvh.cn/Article/details/gykpqryee.sHtML

JS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gxclmhabc.sHtML

TS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/ggxcrugwv.sHtML

Java: super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gyvzndhml.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.zdbjq.cn/Article/details/gdheuxpkb.sHtML

Ruby: super
来源：http://wap.zdbjq.cn/Article/details/gdcqnyjcv.sHtML

C#:   base.Greet();
来源：http://blog.hesvh.cn/Article/details/gdwjkvrvl.sHtML

[G08] 静态方法与属性
来源：http://mobile.zdbjq.cn/Article/details/gppivyjng.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.fehbvm.com/Article/details/gvyuvjynj.sHtML

PHP:  public static function f() {}
来源：http://www.share.fehbvm.com/Article/details/gjhtonqel.sHtML

JS:   static f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfpzeebqv.sHtML

TS:   static f(): void {}
来源：http://baike.hesvh.cn/Article/details/gayhavsls.sHtML

Java: static void f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqpnvwoiy.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.zdbjq.cn/Article/details/gxrwrayta.sHtML

Ruby: def self.f; end
来源：http://wap.hesvh.cn/Article/details/gnnmlduyr.sHtML

C#:   public static void F() {}
来源：http://blog.zdbjq.cn/Article/details/gkhjszdeb.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fehbvm.com/Article/details/gkhecuzml.sHtML


<!-- 参考信息 -->