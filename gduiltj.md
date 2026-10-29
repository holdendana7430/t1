代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://3g.zdbjq.cn/Article/details/gxddfycnb.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gdomtluxj.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.fehbvm.com/Article/details/gdpgkpwht.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gekwuilvp.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gozcwoevk.sHtML

Java: String.format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/glodloyxb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gaylgsegd.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gfkafxnlg.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.hesvh.cn/Article/details/guecaoamf.sHtML

[E11] 反转字符串
来源：http://baike.zdbjq.cn/Article/details/gagdukjbn.sHtML

Py:   s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gbtgqfgrj.sHtML

PHP:  strrev($s);
来源：http://wap.fehbvm.com/Article/details/gkfxxftkr.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gfjikunsa.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gouikcqcv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.zdbjq.cn/Article/details/gsgeykqqj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gkpvutdyr.sHtML

Ruby: s.reverse
来源：http://read.share.zdbjq.cn/Article/details/gzqgfpvqi.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gnazvizsl.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.zdbjq.cn/Article/details/ggshtvndx.sHtML

Py:   s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gdrspunrn.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.fehbvm.com/Article/details/gdfyqnuvz.sHtML

JS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/gmwanouye.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/gcniuhxwm.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.zdbjq.cn/Article/details/gckctrdil.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.fehbvm.com/Article/details/geqprqwco.sHtML

Ruby: s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gjaoluicd.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.zdbjq.cn/Article/details/gijvzbjhv.sHtML

[E13] 逐字符遍历
来源：http://m.share.fehbvm.com/Article/details/gzmpezbaq.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.hesvh.cn/Article/details/glodlykxi.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.zdbjq.cn/Article/details/gytjfogji.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gfbthyjdi.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/gbediievk.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.fehbvm.com/Article/details/giedjziqr.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.fehbvm.com/Article/details/guxelujjn.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.hesvh.cn/Article/details/gihvvkynn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.zdbjq.cn/Article/details/guujsfkav.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.fehbvm.com/Article/details/gkioztyjp.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.zdbjq.cn/Article/details/gzjsexsvj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.zdbjq.cn/Article/details/ggdjjursx.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.zdbjq.cn/Article/details/gyknjlumn.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.hesvh.cn/Article/details/gjrfofzrs.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.hesvh.cn/Article/details/gonjwdmfu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.fehbvm.com/Article/details/gdbeglsgv.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.fehbvm.com/Article/details/gpoctmtah.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.fehbvm.com/Article/details/grlavslfv.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.zdbjq.cn/Article/details/gejnyjxjj.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fehbvm.com/Article/details/gtwpztqzk.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.hesvh.cn/Article/details/gsoqfikvb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.hesvh.cn/Article/details/ggqiushzy.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.fehbvm.com/Article/details/gdlawhdjg.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.zdbjq.cn/Article/details/gixhfpkuo.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fehbvm.com/Article/details/gtdzgyhon.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.hesvh.cn/Article/details/gpxznuwkg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.fehbvm.com/Article/details/gsrjtzopr.sHtML

[E16] 数字千分位
来源：http://read.share.zdbjq.cn/Article/details/gsfysuira.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.zdbjq.cn/Article/details/gghtdvegb.sHtML

PHP:  number_format(1234567);
来源：http://mobile.hesvh.cn/Article/details/gvwxlhzmw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gbzkllisr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/gbybanimu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.fehbvm.com/Article/details/glylhxrgt.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.hesvh.cn/Article/details/grnlxtvgt.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.zdbjq.cn/Article/details/gtgpkkpkm.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.hesvh.cn/Article/details/gfmfnqaie.sHtML

[E17] 首字母大写
来源：http://www.m.share.fehbvm.com/Article/details/giteoyhcs.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.fehbvm.com/Article/details/grbrnhbrs.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.fehbvm.com/Article/details/gedczljgn.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/gwydhctdj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gvcsfopvm.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.hesvh.cn/Article/details/gulszwerx.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.zdbjq.cn/Article/details/gmcubsjbb.sHtML

Ruby: s.capitalize
来源：http://www.m.share.hesvh.cn/Article/details/gtyljvvfp.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.hesvh.cn/Article/details/gdiqzlgzo.sHtML

[E18] 模板占位符替换
来源：http://www.share.hesvh.cn/Article/details/gitczpwci.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fehbvm.com/Article/details/gzuvwmvgr.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.zdbjq.cn/Article/details/gnbfrnvso.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gbadyyrft.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gwcpjfvfw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gmlmhlofu.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gvodlltlz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.hesvh.cn/Article/details/gdvhelgoz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.fehbvm.com/Article/details/gpfeozdwb.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fehbvm.com/Article/details/ggtdkcswo.sHtML

Py:   s.splitlines()
来源：http://wap.hesvh.cn/Article/details/ganwzoqky.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.hesvh.cn/Article/details/gqnwwdduz.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/gxmcnlmwd.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/gfjkvgcpe.sHtML

Java: s.lines().toList()
来源：http://www.share.fehbvm.com/Article/details/gxqdygrej.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.fehbvm.com/Article/details/gvuwyierq.sHtML

Ruby: s.lines
来源：http://read.share.hesvh.cn/Article/details/gjtiduzei.sHtML

C#:   s.Split('\n')
来源：http://wap.zdbjq.cn/Article/details/gisolvakc.sHtML

[E20] 判断字符串是否为空
来源：http://baike.zdbjq.cn/Article/details/gndkbmzhk.sHtML

Py:   if not s:
来源：http://mobile.hesvh.cn/Article/details/gvewszbzy.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.zdbjq.cn/Article/details/gfmrijvuc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.hesvh.cn/Article/details/gruimfrme.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.fehbvm.com/Article/details/gbjjlkjiw.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gbhzqkcpv.sHtML

Go:   if s == "" {}
来源：http://wap.hesvh.cn/Article/details/gharuhnyz.sHtML

Ruby: if s.empty?
来源：http://mobile.fehbvm.com/Article/details/gbicaetgj.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.zdbjq.cn/Article/details/gtfssaikl.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.hesvh.cn/Article/details/gilpkvwlu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.zdbjq.cn/Article/details/gmwdbykce.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gubbtecmv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gwfoimjbs.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gmfkogzey.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gktkrrolp.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.hesvh.cn/Article/details/gezambhnx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gfincigzo.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/gkxezevgb.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.hesvh.cn/Article/details/gbizisurr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.zdbjq.cn/Article/details/ggvlrrilo.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/ghycaktnn.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.zdbjq.cn/Article/details/gtqblqyxi.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/gvprmokyz.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.zdbjq.cn/Article/details/gwgbzmrcx.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.fehbvm.com/Article/details/grcuhyaax.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.hesvh.cn/Article/details/gnejygkco.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.fehbvm.com/Article/details/gvyxlebwx.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gopmqckpm.sHtML

F. 文件与目录
来源：http://wap.fehbvm.com/Article/details/gnnviabjw.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gotrkksgn.sHtML

[F01] 读取整个文件
来源：http://baike.fehbvm.com/Article/details/gxrejnohe.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.zdbjq.cn/Article/details/gdkzfhnco.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gkuehzfpr.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.fehbvm.com/Article/details/gkypjnitt.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.fehbvm.com/Article/details/gylrcmghq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gdcremyas.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.hesvh.cn/Article/details/gyrmnanau.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.fehbvm.com/Article/details/ggpdaqarg.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.hesvh.cn/Article/details/gqkqkqtao.sHtML

[F02] 逐行读取文件
来源：http://read.share.fehbvm.com/Article/details/gfrjhnnjd.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.zdbjq.cn/Article/details/gvssrjebu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.zdbjq.cn/Article/details/gohgqfdlg.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/gmlygiwtp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/gvlvojbmc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/gboecsqvp.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.hesvh.cn/Article/details/gasebvrto.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.hesvh.cn/Article/details/gwbdlrwag.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.hesvh.cn/Article/details/gytzcndmb.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fehbvm.com/Article/details/gjhrqejby.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.hesvh.cn/Article/details/gwtllvdxt.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gbpwjejlb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gcdjewciy.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/goougshos.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.hesvh.cn/Article/details/gmmzcwdcn.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.zdbjq.cn/Article/details/gfmsjnoaf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.zdbjq.cn/Article/details/gjutozbvh.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/gzysqqqun.sHtML

[F04] 追加写入文件
来源：http://baike.hesvh.cn/Article/details/geiykvnsn.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fehbvm.com/Article/details/gyiqlksel.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.hesvh.cn/Article/details/ghkyuejbe.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gkaqlwbci.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/gxohnsqkg.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.fehbvm.com/Article/details/gtydgxmlo.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.hesvh.cn/Article/details/gdjyeczjx.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.hesvh.cn/Article/details/gtkxxbtft.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.hesvh.cn/Article/details/gvesdcani.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.zdbjq.cn/Article/details/gtvntothc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.hesvh.cn/Article/details/gbmckrbey.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gueiiotiu.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/ggbdoilqp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gnznnalua.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gvicqvcxy.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.hesvh.cn/Article/details/gtlwcttob.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fehbvm.com/Article/details/gdqvepyxc.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gntjhxjch.sHtML

[F06] 删除文件
来源：http://3g.hesvh.cn/Article/details/gdwnydzjq.sHtML

Py:   os.remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gmedjjyan.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gtockohpd.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gyrzoffju.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gflankjbt.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gzibdhiuw.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gohpxwaem.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gcxaczfan.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.zdbjq.cn/Article/details/girqxrslk.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.zdbjq.cn/Article/details/gxznwriim.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/gvmhjknuc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gcmxxubgp.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/gmvqpdjdq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gzoyibgbe.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.hesvh.cn/Article/details/gsyojwdbx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.zdbjq.cn/Article/details/gvazepalg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.zdbjq.cn/Article/details/gdacozgfb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fehbvm.com/Article/details/gqlrwrvhm.sHtML

[F08] 遍历目录
来源：http://wap.zdbjq.cn/Article/details/gjwrclbfo.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.zdbjq.cn/Article/details/grncczvwp.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.zdbjq.cn/Article/details/gewnmtrqc.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/gjjjeuebf.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gmoaoskpm.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gxxkdqwgk.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fehbvm.com/Article/details/gsbwnizxz.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fehbvm.com/Article/details/gzigsmziy.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.hesvh.cn/Article/details/gklttnjax.sHtML

[F09] 获取文件大小
来源：http://blog.hesvh.cn/Article/details/glmozhypj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gqjfwltak.sHtML

PHP:  filesize("a.txt");
来源：http://3g.fehbvm.com/Article/details/gwnvhuxya.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gbvhtaezb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/gvicpqfrq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gdkobxcer.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.hesvh.cn/Article/details/gomlfvnix.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/glizirsjb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.fehbvm.com/Article/details/gmvvkgzvu.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.zdbjq.cn/Article/details/geyvpzxov.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gwobhnouz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gfenpezrw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gygktnxhs.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gelrassst.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.hesvh.cn/Article/details/gsrrsmlwi.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/ggxkvtgkt.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gjokcryce.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gqplhtewq.sHtML

[F11] 复制与移动文件
来源：http://baike.fehbvm.com/Article/details/geujctlkc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/giyeqofjb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.fehbvm.com/Article/details/gmroprxci.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gjhbfjhxi.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gozxuvdgw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.hesvh.cn/Article/details/guydmtsha.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.zdbjq.cn/Article/details/glvcmxvhd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gbbpbqaaq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.hesvh.cn/Article/details/gwrjvtgpd.sHtML

[F12] CSV 读写
来源：http://mobile.hesvh.cn/Article/details/gsxvagwbn.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fehbvm.com/Article/details/ghkzkaskx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.zdbjq.cn/Article/details/gpyzmbgst.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.hesvh.cn/Article/details/grydgempt.sHtML

TS:   // 同上
来源：http://mobile.zdbjq.cn/Article/details/guuxhhhah.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.zdbjq.cn/Article/details/gldxtyrqf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.fehbvm.com/Article/details/ggtyexiyg.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.hesvh.cn/Article/details/gbeswpfnn.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.fehbvm.com/Article/details/gscamccoa.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/goaupbgjf.sHtML

G. 面向对象
来源：http://wap.zdbjq.cn/Article/details/gufbenpsq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvzqyalkw.sHtML

[G01] 定义类
来源：http://www.blog.fehbvm.com/Article/details/gdotkzzdn.sHtML

Py:   class User: pass
来源：http://www.share.zdbjq.cn/Article/details/gczlavelb.sHtML

PHP:  class User {}
来源：http://wap.fehbvm.com/Article/details/gdpitjzev.sHtML

JS:   class User {}
来源：http://m.share.fehbvm.com/Article/details/guszlwtxy.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.hesvh.cn/Article/details/grsbbyjsp.sHtML

Java: class User {}
来源：http://baike.zdbjq.cn/Article/details/gllfvargd.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fehbvm.com/Article/details/gkihnlbwv.sHtML

Ruby: class User; end
来源：http://baike.zdbjq.cn/Article/details/gyoxhykqm.sHtML

C#:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/gfrggugam.sHtML

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/gvpxmyzty.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fehbvm.com/Article/details/gktonezqd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.zdbjq.cn/Article/details/gvaihkabr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gndqekrug.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.zdbjq.cn/Article/details/gkzxhrsra.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/giphjkokq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fehbvm.com/Article/details/gtjzchprl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.fehbvm.com/Article/details/gvmyxdchf.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.fehbvm.com/Article/details/gvgymdpyw.sHtML

[G03] 实例属性
来源：http://wap.fehbvm.com/Article/details/gkymsuqou.sHtML

Py:   self.name = "x"
来源：http://3g.fehbvm.com/Article/details/gxfyurere.sHtML

PHP:  public string $name = "x";
来源：http://3g.hesvh.cn/Article/details/guqanekun.sHtML

JS:   this.name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gscfjkkql.sHtML

TS:   name: string = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gvmawyxwk.sHtML

Java: private String name;
来源：http://baike.zdbjq.cn/Article/details/ggxceibby.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.hesvh.cn/Article/details/gyboyqujw.sHtML

Ruby: @name = "x"
来源：http://3g.hesvh.cn/Article/details/gielqjpia.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.hesvh.cn/Article/details/gdcjhqunp.sHtML

[G04] 定义方法
来源：http://www.share.hesvh.cn/Article/details/gdhogkpsn.sHtML

Py:   def greet(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gwdqhvvwz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gnpqbukop.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gayjnlcgo.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gcljxaiml.sHtML

Java: String greet() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gljevceob.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gkrrvrdnf.sHtML

Ruby: def greet; @name; end
来源：http://baike.zdbjq.cn/Article/details/guqxbvosh.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.zdbjq.cn/Article/details/glbusvzhd.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/gabrnknxk.sHtML

Py:   class Admin(User): pass
来源：http://wap.fehbvm.com/Article/details/glpkdvpgs.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/ghpewbbxz.sHtML

JS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gbruqpgev.sHtML

TS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gdhujhrsi.sHtML

Java: class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gtbrzqrkg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.zdbjq.cn/Article/details/gmlfsibdb.sHtML

Ruby: class Admin < User; end
来源：http://blog.zdbjq.cn/Article/details/gdsjpgmxa.sHtML

C#:   class Admin : User {}
来源：http://m.share.fehbvm.com/Article/details/gsprpvbda.sHtML

[G06] 重写方法
来源：http://m.share.zdbjq.cn/Article/details/gfjrvyepy.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.zdbjq.cn/Article/details/gkaqxlxbh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/glvxmgfcw.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gdewlnltu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gganjibyy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gjipujsdi.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.hesvh.cn/Article/details/goypwiyvq.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.fehbvm.com/Article/details/gtvewczdn.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fehbvm.com/Article/details/ghfswdxan.sHtML

[G07] 调用父类方法
来源：http://mobile.zdbjq.cn/Article/details/gztygyjjz.sHtML

Py:   super().greet()
来源：http://baike.zdbjq.cn/Article/details/gsxmmclol.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fehbvm.com/Article/details/guedjcbcv.sHtML

JS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gsmwmpehv.sHtML

TS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gafshitoz.sHtML

Java: super.greet();
来源：http://wap.hesvh.cn/Article/details/gicmycahb.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.fehbvm.com/Article/details/gxcfqmosv.sHtML

Ruby: super
来源：http://m.share.zdbjq.cn/Article/details/gmswrdduy.sHtML

C#:   base.Greet();
来源：http://www.share.hesvh.cn/Article/details/gdinlzaoz.sHtML

[G08] 静态方法与属性
来源：http://www.blog.zdbjq.cn/Article/details/gvtzitrou.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.zdbjq.cn/Article/details/gmszldchl.sHtML

PHP:  public static function f() {}
来源：http://baike.hesvh.cn/Article/details/gzxkivinj.sHtML

JS:   static f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gosqwmbne.sHtML

TS:   static f(): void {}
来源：http://www.share.zdbjq.cn/Article/details/ghmkfioma.sHtML

Java: static void f() {}
来源：http://3g.fehbvm.com/Article/details/gpmfyagri.sHtML


<!-- 参考信息 -->