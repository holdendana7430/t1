代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.hesvh.cn/Article/details/grbsohgbp.sHtML

[E11] 反转字符串
来源：http://www.share.fehbvm.com/Article/details/gawvnxqyo.sHtML

Py:   s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gnndcshgc.sHtML

PHP:  strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gvievjcfq.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/ggnyvjyeh.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gmukwylry.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.zdbjq.cn/Article/details/gkkegsdcz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.hesvh.cn/Article/details/gadmfdfnn.sHtML

Ruby: s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gxzzqtjvh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/gwccnqzsf.sHtML

[E12] 统计某字符出现次数
来源：http://blog.fehbvm.com/Article/details/grjpjzdjr.sHtML

Py:   s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/gjrazoeld.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.hesvh.cn/Article/details/gismhomst.sHtML

JS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/gholsfnkr.sHtML

TS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/gcqpshooi.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.zdbjq.cn/Article/details/gjzaanqxh.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.hesvh.cn/Article/details/ggvusdxeb.sHtML

Ruby: s.count("a")
来源：http://baike.hesvh.cn/Article/details/gtkcyqtay.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.zdbjq.cn/Article/details/gwocxlgjw.sHtML

[E13] 逐字符遍历
来源：http://3g.fehbvm.com/Article/details/gsjbqmljp.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.hesvh.cn/Article/details/gkwxprfgm.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.fehbvm.com/Article/details/gbeypajyv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/gytdrgyfk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/geylijooo.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.hesvh.cn/Article/details/gbaenczfg.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.zdbjq.cn/Article/details/ghwijwqhp.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.zdbjq.cn/Article/details/gvpajrvcc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.hesvh.cn/Article/details/ghcktealx.sHtML

[E14] URL 编码与 Base64
来源：http://blog.zdbjq.cn/Article/details/ghrxsvwuu.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.zdbjq.cn/Article/details/gcfqedrdl.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.hesvh.cn/Article/details/godvyzktv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.fehbvm.com/Article/details/gkqijccmt.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.fehbvm.com/Article/details/grtofjeyu.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.hesvh.cn/Article/details/goukukvza.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.fehbvm.com/Article/details/gkdpohazk.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.fehbvm.com/Article/details/gsmhnywru.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gkqtaqbpx.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.zdbjq.cn/Article/details/greerfyil.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fehbvm.com/Article/details/grpiycvzi.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fehbvm.com/Article/details/gkknkzgfb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.fehbvm.com/Article/details/gvcwwexqe.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.fehbvm.com/Article/details/gmjrqtcxw.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.zdbjq.cn/Article/details/gyvfczbwh.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.zdbjq.cn/Article/details/gbzvqjccm.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.fehbvm.com/Article/details/gkhqbfsqh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.hesvh.cn/Article/details/gxjxxvxjt.sHtML

[E16] 数字千分位
来源：http://3g.zdbjq.cn/Article/details/ggyvixbgj.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.zdbjq.cn/Article/details/gsnrkkmxu.sHtML

PHP:  number_format(1234567);
来源：http://read.share.zdbjq.cn/Article/details/gmqxmafdw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/ghdeeoywa.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/gjjodvgbs.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fehbvm.com/Article/details/gquokiagn.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.hesvh.cn/Article/details/gnkprmwdc.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.zdbjq.cn/Article/details/gvplfnogw.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.fehbvm.com/Article/details/gnrymbjif.sHtML

[E17] 首字母大写
来源：http://baike.hesvh.cn/Article/details/grtgctdnz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.zdbjq.cn/Article/details/gvrseqlbx.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.fehbvm.com/Article/details/gkmhmdlih.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/gzjggncjh.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/gllqswvng.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.hesvh.cn/Article/details/gkyusuwmz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.hesvh.cn/Article/details/gfeqrbbsz.sHtML

Ruby: s.capitalize
来源：http://baike.zdbjq.cn/Article/details/ghwhrlhuo.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.hesvh.cn/Article/details/gzxtvoxse.sHtML

[E18] 模板占位符替换
来源：http://m.share.hesvh.cn/Article/details/gwsgzseeb.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.hesvh.cn/Article/details/gdopboats.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.hesvh.cn/Article/details/gcfebazri.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gzczpqslf.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gpvztndvz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gadjvernf.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gqlsclevu.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.fehbvm.com/Article/details/gnmembewq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.hesvh.cn/Article/details/glriganrd.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.hesvh.cn/Article/details/gnktzphfa.sHtML

Py:   s.splitlines()
来源：http://wap.hesvh.cn/Article/details/goebeyrkq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.hesvh.cn/Article/details/gpbzomuci.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/gpbfxswxq.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gkpzdpufr.sHtML

Java: s.lines().toList()
来源：http://www.share.fehbvm.com/Article/details/gzolwgymb.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fehbvm.com/Article/details/gkdtpudlp.sHtML

Ruby: s.lines
来源：http://m.share.fehbvm.com/Article/details/gxhuucntk.sHtML

C#:   s.Split('\n')
来源：http://mobile.hesvh.cn/Article/details/gqhaevxmd.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.hesvh.cn/Article/details/gboskkgzu.sHtML

Py:   if not s:
来源：http://3g.fehbvm.com/Article/details/gwjvabnom.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.hesvh.cn/Article/details/gkftuzhcf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.fehbvm.com/Article/details/gdavovybr.sHtML

TS:   if (s === "") {}
来源：http://read.share.hesvh.cn/Article/details/gewjrcqju.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gyibyncua.sHtML

Go:   if s == "" {}
来源：http://read.share.fehbvm.com/Article/details/gtvxrpofk.sHtML

Ruby: if s.empty?
来源：http://blog.zdbjq.cn/Article/details/gutcrhzdt.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.zdbjq.cn/Article/details/gjvrtzgka.sHtML

[E21] 超长截断加省略号
来源：http://baike.zdbjq.cn/Article/details/gyqngcvnl.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.zdbjq.cn/Article/details/goefxajow.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gnidblsvz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gsimeyrts.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/grvkyvcxy.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gzszdhrap.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fehbvm.com/Article/details/golwmyajr.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/grwboofdh.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/genozkybn.sHtML

[E22] 字节长度与字符长度
来源：http://3g.hesvh.cn/Article/details/gjyuojbgs.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.hesvh.cn/Article/details/gizpstggk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gvtygcbvn.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/ghnteyncz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/guosxxxeg.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.hesvh.cn/Article/details/gfctwaxpo.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.hesvh.cn/Article/details/gumnsjope.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gxmwtjnjx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.zdbjq.cn/Article/details/gwdxukztp.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/goeucrswf.sHtML

F. 文件与目录
来源：http://m.share.hesvh.cn/Article/details/gsslmkivk.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/greyxqcwr.sHtML

[F01] 读取整个文件
来源：http://www.m.share.hesvh.cn/Article/details/gypfwponr.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.fehbvm.com/Article/details/gxjozfjwv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gweypfpkg.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.fehbvm.com/Article/details/gzxzbahzv.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fehbvm.com/Article/details/gaedjbrsy.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gmwwenhrz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.zdbjq.cn/Article/details/ggiwfvuci.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gyevbtnpw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.hesvh.cn/Article/details/galghbynk.sHtML

[F02] 逐行读取文件
来源：http://baike.fehbvm.com/Article/details/glqwkivnq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.zdbjq.cn/Article/details/gjsbfaqze.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.fehbvm.com/Article/details/gkliznghc.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gvgcfgffl.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gfksadxmz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gnuijqohu.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.hesvh.cn/Article/details/gxkosklou.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.fehbvm.com/Article/details/gghupddfw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.hesvh.cn/Article/details/ggfendouh.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fehbvm.com/Article/details/gdxfolcif.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.fehbvm.com/Article/details/gqufrsveu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gzqqflqxn.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/glnyanfig.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/ghwqgnont.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.fehbvm.com/Article/details/ggdzqpoom.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.hesvh.cn/Article/details/gltjqcdgi.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.zdbjq.cn/Article/details/gttgufcjk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/gvpagtiui.sHtML

[F04] 追加写入文件
来源：http://wap.hesvh.cn/Article/details/genyrvkjl.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fehbvm.com/Article/details/gmrnyslou.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fehbvm.com/Article/details/gfesngaby.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/gnrubebtt.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gzfcfutdp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.hesvh.cn/Article/details/gpijhmpov.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.zdbjq.cn/Article/details/giefdoidu.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.zdbjq.cn/Article/details/gelxovqvv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.fehbvm.com/Article/details/gnfxkmjwh.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.hesvh.cn/Article/details/gwelmudif.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.zdbjq.cn/Article/details/gylaqdyxd.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gnxvlpczx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/glrinyfrv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/ghcjmrzro.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/ghlrffpjf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.hesvh.cn/Article/details/gbozvylzo.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gktlxcszw.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.hesvh.cn/Article/details/glxausblm.sHtML

[F06] 删除文件
来源：http://baike.hesvh.cn/Article/details/gbqbiqxko.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gbqyytvjc.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gboveepln.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gwangnzbi.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gkzfqhdzt.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gyeodoihm.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gxjszwnaf.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gowfwshul.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/glycjnwxy.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.zdbjq.cn/Article/details/gjkbkqxrv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.zdbjq.cn/Article/details/gdsyjxvpw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.zdbjq.cn/Article/details/ghecwgjtw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/gtezyhjjr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/grhngvoro.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.hesvh.cn/Article/details/guljhcgmp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.fehbvm.com/Article/details/ggjsgxpxc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.zdbjq.cn/Article/details/gqvxxmzrf.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.zdbjq.cn/Article/details/guqrvjaej.sHtML

[F08] 遍历目录
来源：http://3g.fehbvm.com/Article/details/gtefcjfmx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.zdbjq.cn/Article/details/gdzazbqbb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.hesvh.cn/Article/details/gnojcgnnj.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/guyfqgymg.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gcbbbnjhi.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gnxdcqbsc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gpcfrmykp.sHtML

Ruby: Dir.children("dir")
来源：http://baike.zdbjq.cn/Article/details/gtbfiqdue.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.zdbjq.cn/Article/details/gjjbuiucp.sHtML

[F09] 获取文件大小
来源：http://3g.fehbvm.com/Article/details/glmzxtihd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gebxqmpxq.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gigvpdgpx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gzcxrwqhz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gejbklvra.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gaghircsy.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.hesvh.cn/Article/details/gvcxghord.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gnnhtwrvb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.fehbvm.com/Article/details/gugriyvgm.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.hesvh.cn/Article/details/gsczqjguv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/grgfxphwj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gjrgocizs.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gllakrdnt.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gyahekewx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.hesvh.cn/Article/details/glddgtxvv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gqlmtfejx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gyestgtup.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gezoazwyi.sHtML

[F11] 复制与移动文件
来源：http://mobile.hesvh.cn/Article/details/gxuamtnuc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gwsmryqlk.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gzohlfqiy.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gnprnbdel.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/glbtclgdd.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.hesvh.cn/Article/details/gghjoglxc.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.fehbvm.com/Article/details/ggpfygthh.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gwvgkomii.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.fehbvm.com/Article/details/gyqtrrthm.sHtML

[F12] CSV 读写
来源：http://www.share.zdbjq.cn/Article/details/gkyvmerza.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fehbvm.com/Article/details/gzexwezmd.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.hesvh.cn/Article/details/gkghjfgub.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.fehbvm.com/Article/details/grwggwjph.sHtML

TS:   // 同上
来源：http://www.blog.fehbvm.com/Article/details/gcemkkixy.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.zdbjq.cn/Article/details/guohtbulp.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.hesvh.cn/Article/details/gfivebuzs.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.zdbjq.cn/Article/details/gwrdzhvhp.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.fehbvm.com/Article/details/gntulspze.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/guphpjdkd.sHtML

G. 面向对象
来源：http://3g.fehbvm.com/Article/details/glsbbeldn.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gfnimdaww.sHtML

[G01] 定义类
来源：http://baike.fehbvm.com/Article/details/gzprnggjz.sHtML

Py:   class User: pass
来源：http://www.share.zdbjq.cn/Article/details/grxjajcvs.sHtML

PHP:  class User {}
来源：http://wap.hesvh.cn/Article/details/gnltrwofl.sHtML

JS:   class User {}
来源：http://wap.zdbjq.cn/Article/details/grebylhxx.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.zdbjq.cn/Article/details/gfxyjunrj.sHtML

Java: class User {}
来源：http://mobile.hesvh.cn/Article/details/gbkijpppa.sHtML

Go:   type User struct { Name string }
来源：http://3g.hesvh.cn/Article/details/gnlpsuzxl.sHtML

Ruby: class User; end
来源：http://mobile.fehbvm.com/Article/details/gllozmzwc.sHtML

C#:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/gnzyopquw.sHtML

[G02] 构造函数
来源：http://www.share.hesvh.cn/Article/details/gzzapogav.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.hesvh.cn/Article/details/gtcesmdph.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.zdbjq.cn/Article/details/gcgubidjl.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gofvkkozu.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/gnouwgywu.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gbfnsmlmj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.fehbvm.com/Article/details/gkwxovvpg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.hesvh.cn/Article/details/grgqdjxlb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.hesvh.cn/Article/details/gacjnjamq.sHtML

[G03] 实例属性
来源：http://wap.hesvh.cn/Article/details/gipzxgcly.sHtML

Py:   self.name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gjvsxusjg.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gpidnvsxd.sHtML

JS:   this.name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gcxbdsyxk.sHtML

TS:   name: string = "x";
来源：http://3g.zdbjq.cn/Article/details/gytlnexie.sHtML

Java: private String name;
来源：http://www.share.hesvh.cn/Article/details/grkagqeqx.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fehbvm.com/Article/details/glvyslxcq.sHtML

Ruby: @name = "x"
来源：http://read.share.fehbvm.com/Article/details/ggqjpuvax.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fehbvm.com/Article/details/glytxlnif.sHtML

[G04] 定义方法
来源：http://www.blog.hesvh.cn/Article/details/gauyddziv.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/glrlxbmqr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/guprnbuul.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/grkxoncom.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gnlqzjqto.sHtML

Java: String greet() { return name; }
来源：http://www.share.fehbvm.com/Article/details/giiyinmcw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gqlrpblsc.sHtML

Ruby: def greet; @name; end
来源：http://read.share.hesvh.cn/Article/details/grtpwdlst.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.hesvh.cn/Article/details/gegqybofw.sHtML

[G05] 继承
来源：http://m.share.zdbjq.cn/Article/details/gpbgeofok.sHtML

Py:   class Admin(User): pass
来源：http://read.share.hesvh.cn/Article/details/gxkqclssc.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gwxzfgwwm.sHtML

JS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gxycqckcf.sHtML

TS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/galssqoem.sHtML

Java: class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gcsftubwq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.hesvh.cn/Article/details/gzaljtcpm.sHtML

Ruby: class Admin < User; end
来源：http://read.share.fehbvm.com/Article/details/gxrjjipmm.sHtML

C#:   class Admin : User {}
来源：http://read.share.fehbvm.com/Article/details/gppatdceu.sHtML

[G06] 重写方法
来源：http://www.share.fehbvm.com/Article/details/gfihfvsid.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.fehbvm.com/Article/details/gxkrdneel.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gfcnaqqyy.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/ghnjxwoub.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/ggwsluvah.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gyqefbqbt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.fehbvm.com/Article/details/gegketjno.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.fehbvm.com/Article/details/gfzslzugf.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fehbvm.com/Article/details/gyolrmklj.sHtML

[G07] 调用父类方法
来源：http://www.blog.fehbvm.com/Article/details/gsfswchtx.sHtML

Py:   super().greet()
来源：http://baike.zdbjq.cn/Article/details/gspnripnr.sHtML

PHP:  parent::greet();
来源：http://read.share.hesvh.cn/Article/details/gvyhnmksg.sHtML

JS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gbkmmfolg.sHtML

TS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gnuxymwjt.sHtML

Java: super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gqhhwfidd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.zdbjq.cn/Article/details/gomkvazcc.sHtML

Ruby: super
来源：http://m.share.fehbvm.com/Article/details/ghrwrduzp.sHtML

C#:   base.Greet();
来源：http://blog.hesvh.cn/Article/details/gitikjpbe.sHtML

[G08] 静态方法与属性
来源：http://www.blog.zdbjq.cn/Article/details/geatbqqdq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.hesvh.cn/Article/details/gccgyvzgl.sHtML

PHP:  public static function f() {}
来源：http://baike.fehbvm.com/Article/details/gjubaywho.sHtML

JS:   static f() {}
来源：http://3g.zdbjq.cn/Article/details/gtwzplivs.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fehbvm.com/Article/details/gqdfnnhlm.sHtML

Java: static void f() {}
来源：http://3g.zdbjq.cn/Article/details/grbykfcfq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.fehbvm.com/Article/details/gbuzswrvb.sHtML

Ruby: def self.f; end
来源：http://www.blog.hesvh.cn/Article/details/gtxtjoynu.sHtML

C#:   public static void F() {}
来源：http://m.share.zdbjq.cn/Article/details/gnyuqmyyj.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.hesvh.cn/Article/details/gaforhucs.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.hesvh.cn/Article/details/gdqcbupdg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.hesvh.cn/Article/details/gxfbchpnl.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.fehbvm.com/Article/details/gzomcoxwt.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.hesvh.cn/Article/details/gjozqqcug.sHtML


<!-- 参考信息 -->