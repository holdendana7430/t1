代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://3g.zdbjq.cn/Article/details/guaqriliz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gcyycblzr.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.zdbjq.cn/Article/details/gtnoqqeir.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/glyeudrhu.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gzcsuwija.sHtML

Java: String.format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gylnrqrgb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gejunmbfh.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gchiepkwp.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.zdbjq.cn/Article/details/gccinvgfs.sHtML

[E11] 反转字符串
来源：http://wap.zdbjq.cn/Article/details/grsxgntpg.sHtML

Py:   s[::-1]
来源：http://read.share.fehbvm.com/Article/details/ggeaoyjbr.sHtML

PHP:  strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gcjvdqrsb.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gehhltedz.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gqoimhhjc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.zdbjq.cn/Article/details/gbnwiqzbf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.hesvh.cn/Article/details/gvtoijopc.sHtML

Ruby: s.reverse
来源：http://3g.hesvh.cn/Article/details/gaslmwdvt.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/gvorzehwx.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.fehbvm.com/Article/details/gptslayvd.sHtML

Py:   s.count("a")
来源：http://www.share.hesvh.cn/Article/details/gzurnlnzz.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.fehbvm.com/Article/details/gvvqmhrts.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/gjnnpyamp.sHtML

TS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gvjscxqib.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.zdbjq.cn/Article/details/gwfyazkzz.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.fehbvm.com/Article/details/gfvehzujp.sHtML

Ruby: s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/gzfiuyddy.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.hesvh.cn/Article/details/gvrkxwyrl.sHtML

[E13] 逐字符遍历
来源：http://blog.fehbvm.com/Article/details/glclptqjh.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.hesvh.cn/Article/details/gayrmviwd.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.fehbvm.com/Article/details/gmovzyuvj.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gepatudny.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/gfjoegdmi.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gcydbycmm.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.fehbvm.com/Article/details/gaufmzgic.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.hesvh.cn/Article/details/gnuzhndif.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.hesvh.cn/Article/details/gzwpjrktz.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.fehbvm.com/Article/details/gcvqpsaty.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.hesvh.cn/Article/details/gamursjsv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gwoxihqzb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.zdbjq.cn/Article/details/gdwlvzcoq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.fehbvm.com/Article/details/gtdnvsfej.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gahjadkke.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.fehbvm.com/Article/details/gerjfyhbo.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.fehbvm.com/Article/details/gcgayhnwu.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.fehbvm.com/Article/details/gulyoqmsy.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.zdbjq.cn/Article/details/gjnjlcelm.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.zdbjq.cn/Article/details/gtuwhhjtz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.fehbvm.com/Article/details/gohpdvrlo.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.hesvh.cn/Article/details/gzyhejndm.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.fehbvm.com/Article/details/gvzhirbcb.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.zdbjq.cn/Article/details/gnipnzsun.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.hesvh.cn/Article/details/gryxfhkpi.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.zdbjq.cn/Article/details/gqfjkblyd.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.zdbjq.cn/Article/details/gckxdvsxy.sHtML

[E16] 数字千分位
来源：http://wap.fehbvm.com/Article/details/gbzchkyxs.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.hesvh.cn/Article/details/gorzzahba.sHtML

PHP:  number_format(1234567);
来源：http://blog.fehbvm.com/Article/details/gybgstkop.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/gubahkztf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/guspwfgay.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.fehbvm.com/Article/details/ggmawtnfd.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.fehbvm.com/Article/details/gpokdsdvy.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.hesvh.cn/Article/details/ggafojebp.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.hesvh.cn/Article/details/gfkgnsyco.sHtML

[E17] 首字母大写
来源：http://blog.zdbjq.cn/Article/details/gdniszzhx.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.fehbvm.com/Article/details/guhhzxpiw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.zdbjq.cn/Article/details/gecqojjya.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/gmkdovzke.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/ggcxowfxx.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fehbvm.com/Article/details/gpqkptskl.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.zdbjq.cn/Article/details/gfgwktjhg.sHtML

Ruby: s.capitalize
来源：http://www.blog.zdbjq.cn/Article/details/gxmdrhvgw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.zdbjq.cn/Article/details/guxfuyedm.sHtML

[E18] 模板占位符替换
来源：http://mobile.fehbvm.com/Article/details/gbetacztt.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.hesvh.cn/Article/details/gcuyaefhh.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.hesvh.cn/Article/details/gtcjsxebu.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gmahrxrkt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gyxgkwtjb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gadroajpt.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gmearboww.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.hesvh.cn/Article/details/gpmdfclan.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.fehbvm.com/Article/details/gwketuuxn.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.fehbvm.com/Article/details/gpbvtanwm.sHtML

Py:   s.splitlines()
来源：http://www.share.zdbjq.cn/Article/details/gwrnhbxea.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.hesvh.cn/Article/details/gurqugdst.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gpccbsknp.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gcokgccft.sHtML

Java: s.lines().toList()
来源：http://wap.zdbjq.cn/Article/details/gawojjdqz.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.fehbvm.com/Article/details/gyuhfpebh.sHtML

Ruby: s.lines
来源：http://www.share.hesvh.cn/Article/details/gwfoeaxuh.sHtML

C#:   s.Split('\n')
来源：http://mobile.hesvh.cn/Article/details/gokowuzii.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.fehbvm.com/Article/details/gzejwuszu.sHtML

Py:   if not s:
来源：http://baike.zdbjq.cn/Article/details/gjqjjiano.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.zdbjq.cn/Article/details/giqigngca.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.zdbjq.cn/Article/details/gvcytrjex.sHtML

TS:   if (s === "") {}
来源：http://read.share.fehbvm.com/Article/details/gmmyvgkmy.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/genlscnyu.sHtML

Go:   if s == "" {}
来源：http://blog.fehbvm.com/Article/details/gksykvvmq.sHtML

Ruby: if s.empty?
来源：http://m.share.zdbjq.cn/Article/details/gybrtvvvq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.fehbvm.com/Article/details/gyjccvhqp.sHtML

[E21] 超长截断加省略号
来源：http://www.share.hesvh.cn/Article/details/gpuujntmq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.zdbjq.cn/Article/details/getdyhdok.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gsytuhnpj.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gxjzuadwz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gejraqqmr.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/glyzaydez.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.hesvh.cn/Article/details/gtwovppdl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gavqwwyei.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/goloanpxy.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.hesvh.cn/Article/details/gyyjgaqfk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gnpqdnkrd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gwujypczf.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/gfrimxfhw.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/gpnewowwk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.zdbjq.cn/Article/details/gwwyhruyv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fehbvm.com/Article/details/gdrdumhwk.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.zdbjq.cn/Article/details/gtjflfsgj.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gycqnfnob.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmezghfxo.sHtML

F. 文件与目录
来源：http://m.share.hesvh.cn/Article/details/gjhomdnmu.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gzjtzvylo.sHtML

[F01] 读取整个文件
来源：http://www.blog.zdbjq.cn/Article/details/gowbupzkh.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.hesvh.cn/Article/details/gkegvflfc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.fehbvm.com/Article/details/gmmevgeme.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.fehbvm.com/Article/details/gdxbfcfnn.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gxjlpseve.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gbnulkhyp.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.hesvh.cn/Article/details/gjmdhzzmi.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gsitdqewt.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/goaytilqh.sHtML

[F02] 逐行读取文件
来源：http://m.share.zdbjq.cn/Article/details/ghkhijjer.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.hesvh.cn/Article/details/gyxqgfirz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.hesvh.cn/Article/details/gqrtsjlec.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gnrlhwjre.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gmnzpvvqm.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gwnxpbkkg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.hesvh.cn/Article/details/gaizvvhgc.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.zdbjq.cn/Article/details/gibnkoflk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.hesvh.cn/Article/details/gkvhyumsv.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.fehbvm.com/Article/details/gbvdnknpz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gznwbkmkv.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/gaqzjvaws.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gsepnbrfl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gbjhhhyog.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.fehbvm.com/Article/details/gjmpilffj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.zdbjq.cn/Article/details/gplgxkhfb.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.zdbjq.cn/Article/details/gnnysueeu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/gzezyjhtu.sHtML

[F04] 追加写入文件
来源：http://blog.fehbvm.com/Article/details/glxmkqorn.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.hesvh.cn/Article/details/gvfviafbm.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.zdbjq.cn/Article/details/gptwuxrbr.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/gqaycysvo.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gvmaeltiy.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.hesvh.cn/Article/details/gjnicrnkm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.fehbvm.com/Article/details/gsrbnrrjy.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.hesvh.cn/Article/details/geqclslhv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.zdbjq.cn/Article/details/gejexecct.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.fehbvm.com/Article/details/gbbyeqjaq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.fehbvm.com/Article/details/guavvuaux.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gjhdvjuju.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gfmguprod.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gblvervtp.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/glvmlgpnf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.hesvh.cn/Article/details/gvclprwby.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gghbxmnlu.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ghqarhfov.sHtML

[F06] 删除文件
来源：http://www.share.hesvh.cn/Article/details/gdygouvlb.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gdvmwykdh.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gikocgapf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gblhfrrzx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gtqgfpquy.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gglmysxgc.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gkvrowfxc.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gmvglvtvz.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gygbtincs.sHtML

[F07] 创建目录（含多级）
来源：http://blog.zdbjq.cn/Article/details/gcuqfiubb.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gmnobkfvw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.hesvh.cn/Article/details/gsqyhfvhe.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gasgiqrye.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/ggoaxaotk.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.hesvh.cn/Article/details/gewbgbkog.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.zdbjq.cn/Article/details/ggvehtagn.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.fehbvm.com/Article/details/govwbjvcs.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.fehbvm.com/Article/details/gpmmlecfj.sHtML

[F08] 遍历目录
来源：http://3g.hesvh.cn/Article/details/guhyhyeui.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.zdbjq.cn/Article/details/gsbpfmkfr.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.zdbjq.cn/Article/details/gezfbksha.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gqedeazlr.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gwwzuzkns.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/gdzbdykfw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fehbvm.com/Article/details/gibhiuegg.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fehbvm.com/Article/details/gavogfdpa.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.hesvh.cn/Article/details/glnickvce.sHtML

[F09] 获取文件大小
来源：http://blog.fehbvm.com/Article/details/gcoxfjkhj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gzzxrenhm.sHtML

PHP:  filesize("a.txt");
来源：http://wap.fehbvm.com/Article/details/gtryplzdo.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gxgtsdwfs.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gxxmakphz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/geskdthka.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.zdbjq.cn/Article/details/gsuddhzro.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gzhhcnraz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.zdbjq.cn/Article/details/gviwcnodt.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.fehbvm.com/Article/details/gbcihlfxk.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gcechmgno.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.hesvh.cn/Article/details/garykpnwt.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gyyzwjozu.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fehbvm.com/Article/details/gxlwtmfsx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.zdbjq.cn/Article/details/gwhdghmbn.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gwujmjxic.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gejfjshyk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gukifrjlm.sHtML

[F11] 复制与移动文件
来源：http://www.blog.zdbjq.cn/Article/details/ghbxiblzd.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gxqktbwad.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gwgmcfdxa.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/grwwbnvfz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gojjcfgul.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gflmsaaqg.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fehbvm.com/Article/details/gxsthsjru.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gpqkabocb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.zdbjq.cn/Article/details/gbmucvxac.sHtML

[F12] CSV 读写
来源：http://www.m.share.hesvh.cn/Article/details/gektxntar.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.hesvh.cn/Article/details/ggrykyrjg.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.zdbjq.cn/Article/details/gvdwoieei.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.hesvh.cn/Article/details/gqnwpibvp.sHtML

TS:   // 同上
来源：http://3g.hesvh.cn/Article/details/gkfeaizjl.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fehbvm.com/Article/details/goeovjjgc.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.fehbvm.com/Article/details/gcirlemrx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.zdbjq.cn/Article/details/grcggajkz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.zdbjq.cn/Article/details/gohfihkby.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gdxocenph.sHtML

G. 面向对象
来源：http://wap.fehbvm.com/Article/details/gpdqgvkjh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/glrwdruiw.sHtML

[G01] 定义类
来源：http://read.share.hesvh.cn/Article/details/gsvtjkkzo.sHtML

Py:   class User: pass
来源：http://mobile.fehbvm.com/Article/details/gpgawvktq.sHtML

PHP:  class User {}
来源：http://www.blog.fehbvm.com/Article/details/gjboegvuy.sHtML

JS:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gzklblxrg.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fehbvm.com/Article/details/gtryakiwu.sHtML

Java: class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gsmjokzst.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.zdbjq.cn/Article/details/gjyailybq.sHtML

Ruby: class User; end
来源：http://www.blog.hesvh.cn/Article/details/gzbilrgua.sHtML

C#:   class User {}
来源：http://3g.hesvh.cn/Article/details/gvcmkjmdx.sHtML

[G02] 构造函数
来源：http://m.share.fehbvm.com/Article/details/gblbtgrtn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.zdbjq.cn/Article/details/ggwrcpmmh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.hesvh.cn/Article/details/gsygrhxry.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gghjjcnui.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fehbvm.com/Article/details/gkbwuzucn.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gkmcvmlwd.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.fehbvm.com/Article/details/ggnrnzkwr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.zdbjq.cn/Article/details/glmvywacp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.zdbjq.cn/Article/details/gwgsjdgjb.sHtML

[G03] 实例属性
来源：http://www.m.share.hesvh.cn/Article/details/gjppdeygk.sHtML

Py:   self.name = "x"
来源：http://3g.hesvh.cn/Article/details/gauzbkkqm.sHtML

PHP:  public string $name = "x";
来源：http://blog.zdbjq.cn/Article/details/gzhulzafk.sHtML

JS:   this.name = "x";
来源：http://www.blog.fehbvm.com/Article/details/genlbhvmu.sHtML

TS:   name: string = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gzzwkicuf.sHtML

Java: private String name;
来源：http://m.share.hesvh.cn/Article/details/gjgvsllch.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.hesvh.cn/Article/details/gnhujhxur.sHtML

Ruby: @name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gedxejlag.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/galsqzies.sHtML

[G04] 定义方法
来源：http://3g.hesvh.cn/Article/details/gfaimevxt.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gwhjlwluo.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/glgallisl.sHtML

JS:   greet() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gpshkhzjk.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gwbzrftbg.sHtML

Java: String greet() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/ggpuqufpr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gxfoyphim.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gwezseozk.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.hesvh.cn/Article/details/grspietvz.sHtML

[G05] 继承
来源：http://baike.zdbjq.cn/Article/details/gxbtfocqh.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fehbvm.com/Article/details/gusfcxujp.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gqmkykqvd.sHtML

JS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gscaqwriq.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gynqlqxrr.sHtML

Java: class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gncyvfibr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.hesvh.cn/Article/details/gegrzzjik.sHtML

Ruby: class Admin < User; end
来源：http://3g.zdbjq.cn/Article/details/gfcnexcxj.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.fehbvm.com/Article/details/gmxolcqta.sHtML

[G06] 重写方法
来源：http://baike.hesvh.cn/Article/details/gsiatgasg.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.fehbvm.com/Article/details/gymqarjim.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gxjghjhmz.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/grfgzsoql.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/ghlvhmlei.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gmgmqyalj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.zdbjq.cn/Article/details/gpeltiykh.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.hesvh.cn/Article/details/gopvjsmtx.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.fehbvm.com/Article/details/gnzmjafwv.sHtML

[G07] 调用父类方法
来源：http://m.share.hesvh.cn/Article/details/gvznwqszr.sHtML

Py:   super().greet()
来源：http://wap.fehbvm.com/Article/details/gkerqezji.sHtML

PHP:  parent::greet();
来源：http://www.share.hesvh.cn/Article/details/gugupjkzk.sHtML

JS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gsroufzpi.sHtML

TS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gpaonwpwe.sHtML

Java: super.greet();
来源：http://mobile.fehbvm.com/Article/details/gqdshvatj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.zdbjq.cn/Article/details/gmeehmxft.sHtML

Ruby: super
来源：http://wap.fehbvm.com/Article/details/gmucjknsi.sHtML

C#:   base.Greet();
来源：http://www.blog.hesvh.cn/Article/details/gdzdozdth.sHtML

[G08] 静态方法与属性
来源：http://blog.fehbvm.com/Article/details/gpxeurztj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.zdbjq.cn/Article/details/gbfketsar.sHtML

PHP:  public static function f() {}
来源：http://blog.fehbvm.com/Article/details/gaoejgext.sHtML

JS:   static f() {}
来源：http://3g.fehbvm.com/Article/details/glxfwfvig.sHtML

TS:   static f(): void {}
来源：http://www.share.fehbvm.com/Article/details/gbqkoirvv.sHtML

Java: static void f() {}
来源：http://read.share.hesvh.cn/Article/details/gshuxlehh.sHtML


<!-- 参考信息 -->