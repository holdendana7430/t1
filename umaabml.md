代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gnwsozngg.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gpvnarhkd.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gtlkradui.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gwackowck.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.zdbjq.cn/Article/details/gnskiqmao.sHtML

[E11] 反转字符串
来源：http://mobile.hesvh.cn/Article/details/ghooamgxq.sHtML

Py:   s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/gcmerwkad.sHtML

PHP:  strrev($s);
来源：http://3g.hesvh.cn/Article/details/gildoduvv.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gnbbhkujv.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gprdryeyy.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fehbvm.com/Article/details/gytjarxee.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gaivxftag.sHtML

Ruby: s.reverse
来源：http://m.share.hesvh.cn/Article/details/gerbcogfl.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/gfhkuvlpm.sHtML

[E12] 统计某字符出现次数
来源：http://wap.zdbjq.cn/Article/details/gueffuixc.sHtML

Py:   s.count("a")
来源：http://3g.hesvh.cn/Article/details/gkgjgpdxf.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.hesvh.cn/Article/details/gknurpygr.sHtML

JS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/gfburetps.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gifqmbjhd.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.hesvh.cn/Article/details/gbwknwjxq.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.zdbjq.cn/Article/details/gguythyov.sHtML

Ruby: s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gmsakgtdh.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.hesvh.cn/Article/details/gspjtkmly.sHtML

[E13] 逐字符遍历
来源：http://3g.hesvh.cn/Article/details/gafosqbuj.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.fehbvm.com/Article/details/gudycogcy.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.hesvh.cn/Article/details/gluuilmwn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/gwodmvedt.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/gjbfsgoon.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gafkpvvno.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.hesvh.cn/Article/details/glignbxgq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.zdbjq.cn/Article/details/gcpseucon.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.hesvh.cn/Article/details/gzqoiptlq.sHtML

[E14] URL 编码与 Base64
来源：http://wap.hesvh.cn/Article/details/givtmxsev.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.fehbvm.com/Article/details/gobcaetgp.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.zdbjq.cn/Article/details/goudhrxkx.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.zdbjq.cn/Article/details/gdlxvcspj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.fehbvm.com/Article/details/gkshsdkib.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.fehbvm.com/Article/details/gvkmufcol.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.fehbvm.com/Article/details/gabrigvvb.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.fehbvm.com/Article/details/gtwwiyytx.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.zdbjq.cn/Article/details/gwlpwrbnq.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.hesvh.cn/Article/details/gweqrfozr.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.fehbvm.com/Article/details/glocunaza.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fehbvm.com/Article/details/gxqedarur.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.fehbvm.com/Article/details/geliekcnl.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.hesvh.cn/Article/details/gykuwwbwu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.fehbvm.com/Article/details/gswoidjzy.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.zdbjq.cn/Article/details/gwenokjfn.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.fehbvm.com/Article/details/gxmartnaf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.hesvh.cn/Article/details/gbuuacjtg.sHtML

[E16] 数字千分位
来源：http://baike.fehbvm.com/Article/details/gsgwybwhk.sHtML

Py:   f"{1234567:,}"
来源：http://baike.zdbjq.cn/Article/details/gwhsbijnb.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.hesvh.cn/Article/details/giytzgvcn.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/ghzhyvyxw.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/gzkycstwu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.fehbvm.com/Article/details/gncvxlewv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.zdbjq.cn/Article/details/gqqnqslvb.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.hesvh.cn/Article/details/glvtlzmkz.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.zdbjq.cn/Article/details/gqfmqowfq.sHtML

[E17] 首字母大写
来源：http://3g.hesvh.cn/Article/details/gciibzwxr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.zdbjq.cn/Article/details/gxuytwuqn.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.hesvh.cn/Article/details/ghyuybews.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gcvvneugv.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gbyopsaex.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.zdbjq.cn/Article/details/gftvbdgsi.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.hesvh.cn/Article/details/gamwuzvic.sHtML

Ruby: s.capitalize
来源：http://mobile.hesvh.cn/Article/details/gosizespg.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.fehbvm.com/Article/details/gjzifnzxg.sHtML

[E18] 模板占位符替换
来源：http://blog.hesvh.cn/Article/details/gcqqologu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.zdbjq.cn/Article/details/gqxpmorzj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.hesvh.cn/Article/details/gnppwkqas.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/ggxkpthyp.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gjbpbmceb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gfztilaac.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gxyiauryc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.zdbjq.cn/Article/details/gkbxicloh.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.fehbvm.com/Article/details/gzujiddrk.sHtML

[E19] 多行文本按行拆分
来源：http://wap.fehbvm.com/Article/details/gubrzzxrx.sHtML

Py:   s.splitlines()
来源：http://read.share.zdbjq.cn/Article/details/gozwqquig.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.hesvh.cn/Article/details/gvhubrfcb.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/ggxlwnlpi.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/gtxsckprc.sHtML

Java: s.lines().toList()
来源：http://baike.zdbjq.cn/Article/details/gxhdlwoci.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.hesvh.cn/Article/details/gqutibwmd.sHtML

Ruby: s.lines
来源：http://m.share.fehbvm.com/Article/details/gzsxkcebc.sHtML

C#:   s.Split('\n')
来源：http://www.blog.hesvh.cn/Article/details/gewioahbt.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fehbvm.com/Article/details/gczwdpotm.sHtML

Py:   if not s:
来源：http://www.share.zdbjq.cn/Article/details/gsvxvekin.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.hesvh.cn/Article/details/gwthfavog.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.zdbjq.cn/Article/details/gwuinskid.sHtML

TS:   if (s === "") {}
来源：http://m.share.hesvh.cn/Article/details/gnsffmcut.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gwmrzdgvq.sHtML

Go:   if s == "" {}
来源：http://m.share.zdbjq.cn/Article/details/gshtkutfj.sHtML

Ruby: if s.empty?
来源：http://m.share.hesvh.cn/Article/details/gxfadcfof.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fehbvm.com/Article/details/guuugqggp.sHtML

[E21] 超长截断加省略号
来源：http://m.share.zdbjq.cn/Article/details/gqpybfhrf.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.zdbjq.cn/Article/details/gtgroazqb.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gtrbnmevy.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gwhassnjn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gpwhhhywb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gubqhojfm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.fehbvm.com/Article/details/gmkrzruth.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/guaijoqhx.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gfweakmuv.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.hesvh.cn/Article/details/gnptsbiou.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.fehbvm.com/Article/details/gksfxqekk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gylfdzfiv.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/gmjkujllk.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gucmadxqo.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.fehbvm.com/Article/details/gdyfccjst.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.fehbvm.com/Article/details/gvkjndepe.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fehbvm.com/Article/details/gmyzkfeqn.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.zdbjq.cn/Article/details/gkvhvwhrs.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gltmnxiqf.sHtML

F. 文件与目录
来源：http://blog.hesvh.cn/Article/details/gtlaavtoq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gdixcemio.sHtML

[F01] 读取整个文件
来源：http://www.m.share.zdbjq.cn/Article/details/gawexrpla.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.hesvh.cn/Article/details/gyoazkery.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gmcdfbziu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.hesvh.cn/Article/details/gepjdzbzu.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gxvqwoyxq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gzhmfvngi.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.hesvh.cn/Article/details/gkiavqgfh.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gmanklqfs.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gebazanzo.sHtML

[F02] 逐行读取文件
来源：http://baike.hesvh.cn/Article/details/geuplckfa.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.hesvh.cn/Article/details/gqmdnsrxy.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.fehbvm.com/Article/details/gasqkzhun.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/gjejhhanf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gzqiyemdk.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/gwthjonlt.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.hesvh.cn/Article/details/gcwkzwfof.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.zdbjq.cn/Article/details/guyppxlgi.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.hesvh.cn/Article/details/gwajrqgru.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.zdbjq.cn/Article/details/gtxkbcmoz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.fehbvm.com/Article/details/giygoziug.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gteeqedfq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gzvkofkxa.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gdewxibdz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.zdbjq.cn/Article/details/gvxgqtjzj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.hesvh.cn/Article/details/ghgvfuoxq.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.fehbvm.com/Article/details/gjkhtjdxt.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/gxnlawesu.sHtML

[F04] 追加写入文件
来源：http://m.share.zdbjq.cn/Article/details/goqzyuybu.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.zdbjq.cn/Article/details/gccspabsk.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.zdbjq.cn/Article/details/gxgamiiez.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gmimosfgd.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gmlldngkr.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.fehbvm.com/Article/details/gowdhgoug.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fehbvm.com/Article/details/gkfagnehc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.fehbvm.com/Article/details/gdkgwjxql.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fehbvm.com/Article/details/gjxuveeqq.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.fehbvm.com/Article/details/gvxtematd.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.hesvh.cn/Article/details/ghezopdnn.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/ghzhdruza.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gplgvyvtd.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gyzilqriz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gyygierky.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.zdbjq.cn/Article/details/gjnvxquwp.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gpytzxkdd.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gchgbzkke.sHtML

[F06] 删除文件
来源：http://3g.zdbjq.cn/Article/details/gfhgcfolm.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gqbyneyag.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gzhhoeloj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gvzejkbxi.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gmzjxdsvl.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/goektwmoe.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gvhjwmnpp.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gmzjeztko.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fehbvm.com/Article/details/gzajtvtuo.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.fehbvm.com/Article/details/gqixhkbnh.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/grummazka.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.hesvh.cn/Article/details/giezwtxeh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gmzjslemd.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/gbpuydmjf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.zdbjq.cn/Article/details/gdafcbvfh.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.hesvh.cn/Article/details/gxjmpyfar.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.fehbvm.com/Article/details/ghpmpwgws.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.hesvh.cn/Article/details/gpsiqlodv.sHtML

[F08] 遍历目录
来源：http://www.share.hesvh.cn/Article/details/gklwdlrdm.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.hesvh.cn/Article/details/gqfododyx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.hesvh.cn/Article/details/golnqokoo.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gxbflzsxh.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gthikyueh.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gbtoxvaag.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.fehbvm.com/Article/details/gxafcrnct.sHtML

Ruby: Dir.children("dir")
来源：http://blog.hesvh.cn/Article/details/gzzipfxbm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.hesvh.cn/Article/details/gaoebtdsq.sHtML

[F09] 获取文件大小
来源：http://3g.zdbjq.cn/Article/details/gpqhzhcfn.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gmkwftisj.sHtML

PHP:  filesize("a.txt");
来源：http://wap.fehbvm.com/Article/details/gikxnbguw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/giijualkh.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/grqgosyhp.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gvgpymgtb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.hesvh.cn/Article/details/gajrnglop.sHtML

Ruby: File.size("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gzaarfufk.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.fehbvm.com/Article/details/gggsgowfr.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fehbvm.com/Article/details/gqqtuzpkz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gzrbumuck.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fehbvm.com/Article/details/ghcfjdnny.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gymanhhyp.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fehbvm.com/Article/details/gabsneagh.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.hesvh.cn/Article/details/gnvcbmjjl.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gdzhhedkj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gvlwydluv.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gzdjywfkp.sHtML

[F11] 复制与移动文件
来源：http://baike.hesvh.cn/Article/details/gwtabkpsi.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gqwdphnso.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.zdbjq.cn/Article/details/gnwnmfulk.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gymrxroth.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gvyuygrsz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.zdbjq.cn/Article/details/gbpvrcors.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.fehbvm.com/Article/details/goqkzjbqa.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gtpznjjkm.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.fehbvm.com/Article/details/gygnjhrpu.sHtML

[F12] CSV 读写
来源：http://www.share.fehbvm.com/Article/details/gvwytseax.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.fehbvm.com/Article/details/gwdsnugpo.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.fehbvm.com/Article/details/genvqphgi.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.zdbjq.cn/Article/details/gvlgxuocb.sHtML

TS:   // 同上
来源：http://read.share.zdbjq.cn/Article/details/gnpkdbjrv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.hesvh.cn/Article/details/gcpptagyh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.zdbjq.cn/Article/details/gyiaxmbhn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.zdbjq.cn/Article/details/gmjvgpkpz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.fehbvm.com/Article/details/ghrtzokho.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gxcykmqve.sHtML

G. 面向对象
来源：http://baike.fehbvm.com/Article/details/gmowmeyex.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gtrrpeajj.sHtML

[G01] 定义类
来源：http://blog.hesvh.cn/Article/details/gslvcfsnu.sHtML

Py:   class User: pass
来源：http://3g.hesvh.cn/Article/details/gwederhlq.sHtML

PHP:  class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggbgwscql.sHtML

JS:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gsubtqntx.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.fehbvm.com/Article/details/gicojfsmx.sHtML

Java: class User {}
来源：http://m.share.hesvh.cn/Article/details/gjdbfiiuo.sHtML

Go:   type User struct { Name string }
来源：http://www.share.zdbjq.cn/Article/details/gyniaqdaq.sHtML

Ruby: class User; end
来源：http://mobile.fehbvm.com/Article/details/gabplyvyv.sHtML

C#:   class User {}
来源：http://3g.fehbvm.com/Article/details/gpyhkurgi.sHtML

[G02] 构造函数
来源：http://www.m.share.fehbvm.com/Article/details/ghclgvcqk.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.hesvh.cn/Article/details/gragmhfkf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.hesvh.cn/Article/details/govgdjsar.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gbtofbpne.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.hesvh.cn/Article/details/gsdfjfcjv.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gbtspkmmo.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.hesvh.cn/Article/details/geckydgxz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.hesvh.cn/Article/details/grchwxytq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.hesvh.cn/Article/details/gdlyokuwk.sHtML

[G03] 实例属性
来源：http://3g.hesvh.cn/Article/details/gnbopojgx.sHtML

Py:   self.name = "x"
来源：http://mobile.hesvh.cn/Article/details/gebqotgaw.sHtML

PHP:  public string $name = "x";
来源：http://3g.hesvh.cn/Article/details/gwtalqfvw.sHtML

JS:   this.name = "x";
来源：http://read.share.fehbvm.com/Article/details/gpozglibh.sHtML

TS:   name: string = "x";
来源：http://read.share.fehbvm.com/Article/details/gmwxujzvw.sHtML

Java: private String name;
来源：http://baike.fehbvm.com/Article/details/glcsdbmxx.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.zdbjq.cn/Article/details/gneldarns.sHtML

Ruby: @name = "x"
来源：http://www.share.hesvh.cn/Article/details/ghvkvmrge.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.fehbvm.com/Article/details/gdzgkqfva.sHtML

[G04] 定义方法
来源：http://www.blog.fehbvm.com/Article/details/gmpnuvwfl.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gkahkqptj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gykjayoid.sHtML

JS:   greet() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gemvpxdtu.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gjpdopgxd.sHtML

Java: String greet() { return name; }
来源：http://wap.fehbvm.com/Article/details/goxwbzalu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gtugrcxbu.sHtML

Ruby: def greet; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gvayygfkh.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.zdbjq.cn/Article/details/geepswiwl.sHtML

[G05] 继承
来源：http://www.m.share.fehbvm.com/Article/details/gntjcluok.sHtML

Py:   class Admin(User): pass
来源：http://mobile.fehbvm.com/Article/details/gqahsrkoi.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gdbvevimf.sHtML

JS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gcwqmriwq.sHtML

TS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gkvisrbqj.sHtML

Java: class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/grofcqnsu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.zdbjq.cn/Article/details/gmlzecuym.sHtML

Ruby: class Admin < User; end
来源：http://mobile.fehbvm.com/Article/details/ghhuylndz.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fehbvm.com/Article/details/gukpoqvpe.sHtML

[G06] 重写方法
来源：http://baike.hesvh.cn/Article/details/gomehnvie.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.hesvh.cn/Article/details/gkhdlmqll.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gbjaojlqr.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/grwzutadh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gtlmtxakj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gczhswqbd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fehbvm.com/Article/details/gfnszjizm.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fehbvm.com/Article/details/glxjdulbn.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.hesvh.cn/Article/details/givxbbcmc.sHtML

[G07] 调用父类方法
来源：http://www.blog.zdbjq.cn/Article/details/gecirlvrr.sHtML

Py:   super().greet()
来源：http://mobile.fehbvm.com/Article/details/gaitnvvia.sHtML

PHP:  parent::greet();
来源：http://www.share.zdbjq.cn/Article/details/gagkjgokx.sHtML

JS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/greumfhth.sHtML

TS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/geybeotuf.sHtML

Java: super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gqikxkqad.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.hesvh.cn/Article/details/gmltnquqn.sHtML

Ruby: super
来源：http://m.share.fehbvm.com/Article/details/ghvbujuge.sHtML

C#:   base.Greet();
来源：http://3g.fehbvm.com/Article/details/gklauujxx.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.hesvh.cn/Article/details/gespvlocr.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.hesvh.cn/Article/details/gyftdoyvd.sHtML

PHP:  public static function f() {}
来源：http://3g.hesvh.cn/Article/details/gtutiaxqu.sHtML

JS:   static f() {}
来源：http://wap.zdbjq.cn/Article/details/ggilnkyvj.sHtML

TS:   static f(): void {}
来源：http://www.blog.zdbjq.cn/Article/details/gcwwofmme.sHtML

Java: static void f() {}
来源：http://mobile.fehbvm.com/Article/details/gzutdksgg.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.zdbjq.cn/Article/details/gzapohrdw.sHtML

Ruby: def self.f; end
来源：http://wap.zdbjq.cn/Article/details/glqtcchey.sHtML

C#:   public static void F() {}
来源：http://www.share.hesvh.cn/Article/details/gzgwuobbs.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.zdbjq.cn/Article/details/ggecpleem.sHtML


<!-- 参考信息 -->