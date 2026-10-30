代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://baike.fanxiaobao.xyz/Article/details/gbkogflej.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvcmzgvyr.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.fanxiaobao.xyz/Article/details/gedxysqsc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlxdubwd.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnvebauc.sHtML

[E11] 反转字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gkfklzzgf.sHtML

Py:   s[::-1]
来源：http://mobile.fanxiaobao.xyz/Article/details/gckttfawc.sHtML

PHP:  strrev($s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbyadehja.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.fanxiaobao.xyz/Article/details/gtnhbijjy.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckscocjv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.fanxiaobao.xyz/Article/details/gdoimkhnm.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.fanxiaobao.xyz/Article/details/gfyolhvdm.sHtML

Ruby: s.reverse
来源：http://www.share.fanxiaobao.xyz/Article/details/gbscrhcdk.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.fanxiaobao.xyz/Article/details/gbjysgwac.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.fanxiaobao.xyz/Article/details/gntbuxmsg.sHtML

Py:   s.count("a")
来源：http://wap.fanxiaobao.xyz/Article/details/gogdcfbpc.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.fanxiaobao.xyz/Article/details/gslwzzvyl.sHtML

JS:   s.split("a").length - 1
来源：http://blog.fanxiaobao.xyz/Article/details/ggtxcqnuu.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fanxiaobao.xyz/Article/details/gahtaaqme.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdomvtdp.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpukrskcp.sHtML

Ruby: s.count("a")
来源：http://3g.fanxiaobao.xyz/Article/details/glestzuzj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.fanxiaobao.xyz/Article/details/gdxbsbidd.sHtML

[E13] 逐字符遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gdzsezlzn.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.fanxiaobao.xyz/Article/details/gcjpkzddn.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxfiuvon.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fanxiaobao.xyz/Article/details/gsmwfaxms.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fanxiaobao.xyz/Article/details/gazvpprkc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gudkadtmo.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvlbbfove.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.fanxiaobao.xyz/Article/details/grvvvzahu.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.fanxiaobao.xyz/Article/details/gzkkxvfdr.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpjmrhjc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.fanxiaobao.xyz/Article/details/gytylltnm.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwscnuxa.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.fanxiaobao.xyz/Article/details/gupnbngmc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.fanxiaobao.xyz/Article/details/geqkwyftb.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.fanxiaobao.xyz/Article/details/geqtevwey.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdacshqop.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.fanxiaobao.xyz/Article/details/ggksdpmmm.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.fanxiaobao.xyz/Article/details/grfqklzbk.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdeuroyc.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsligqteg.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkzejrab.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnshyqjyk.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltfgqvlj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.fanxiaobao.xyz/Article/details/galzqgcoq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.fanxiaobao.xyz/Article/details/ghgnaokqt.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpktfvkyl.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gslkhfzzt.sHtML

[E16] 数字千分位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvcnrbgl.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtgiscfp.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fanxiaobao.xyz/Article/details/gulxiutns.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.fanxiaobao.xyz/Article/details/gqsaofxep.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqrzghbo.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/griqmsztv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpwbbexi.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjhwulqp.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.fanxiaobao.xyz/Article/details/gqdrujpjy.sHtML

[E17] 首字母大写
来源：http://baike.fanxiaobao.xyz/Article/details/gptolqjnr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.fanxiaobao.xyz/Article/details/gefsocmqr.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnhpbpdq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqmzhjjc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fanxiaobao.xyz/Article/details/gjmdwteak.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.fanxiaobao.xyz/Article/details/ghrqsfdzc.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.fanxiaobao.xyz/Article/details/gvzthfdzy.sHtML

Ruby: s.capitalize
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvzmmgay.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fanxiaobao.xyz/Article/details/gctgktqjo.sHtML

[E18] 模板占位符替换
来源：http://blog.fanxiaobao.xyz/Article/details/gnktiidca.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gleekhkuu.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjeygzsxj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqdowleh.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkbwxsuc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fanxiaobao.xyz/Article/details/gkqceksgo.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.fanxiaobao.xyz/Article/details/grycfmcxd.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdyaynmea.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.fanxiaobao.xyz/Article/details/gdyzgvsei.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.fanxiaobao.xyz/Article/details/gufjzczyg.sHtML

Py:   s.splitlines()
来源：http://mobile.fanxiaobao.xyz/Article/details/gnyknmzvm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsctpaubt.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fanxiaobao.xyz/Article/details/grkozhilv.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gullkephj.sHtML

Java: s.lines().toList()
来源：http://blog.fanxiaobao.xyz/Article/details/gutosjjyf.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.fanxiaobao.xyz/Article/details/gmgdbxycv.sHtML

Ruby: s.lines
来源：http://wap.fanxiaobao.xyz/Article/details/gwifrpjna.sHtML

C#:   s.Split('\n')
来源：http://read.share.fanxiaobao.xyz/Article/details/gysmbcorz.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbyxdmtj.sHtML

Py:   if not s:
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gilgfkyjk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnubdzxir.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/givjihvmg.sHtML

TS:   if (s === "") {}
来源：http://www.share.fanxiaobao.xyz/Article/details/guwiuabow.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gevzipugq.sHtML

Go:   if s == "" {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gumlodrgp.sHtML

Ruby: if s.empty?
来源：http://mobile.fanxiaobao.xyz/Article/details/gaqpsxmhv.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gevapnwbu.sHtML

[E21] 超长截断加省略号
来源：http://3g.fanxiaobao.xyz/Article/details/gmfaapjty.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmbdjgmp.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggquzkfia.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fanxiaobao.xyz/Article/details/gpmnwpsph.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhduombl.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fanxiaobao.xyz/Article/details/grixkqmaj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.fanxiaobao.xyz/Article/details/gcomarmtj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrfpdsqt.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.fanxiaobao.xyz/Article/details/gwfnhibjz.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxocuffk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gpixqvnxp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fanxiaobao.xyz/Article/details/gbzuratrm.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fanxiaobao.xyz/Article/details/gafegzaxg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fanxiaobao.xyz/Article/details/gvamntnas.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.fanxiaobao.xyz/Article/details/glmsimdka.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.fanxiaobao.xyz/Article/details/gcehzecsd.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gckutqfqq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.fanxiaobao.xyz/Article/details/gaoitpkai.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/ggixfiztm.sHtML

F. 文件与目录
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjhboesq.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gpblchxtm.sHtML

[F01] 读取整个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gkijszrak.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.fanxiaobao.xyz/Article/details/gwuymggtf.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/gazdcjafp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.fanxiaobao.xyz/Article/details/gnrvffvfx.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fanxiaobao.xyz/Article/details/gxjisdqne.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.fanxiaobao.xyz/Article/details/gztryvmid.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.fanxiaobao.xyz/Article/details/gbktnnvdf.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkrlmqpoj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/gcvykppfp.sHtML

[F02] 逐行读取文件
来源：http://baike.fanxiaobao.xyz/Article/details/gvasvkfhx.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfswzgun.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.fanxiaobao.xyz/Article/details/grhabmeji.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gkiekldcd.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gtugrirkb.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggitqecpo.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.fanxiaobao.xyz/Article/details/glavcahot.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.fanxiaobao.xyz/Article/details/gboiqmklb.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fanxiaobao.xyz/Article/details/glswyvzdt.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqrsfeuu.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.fanxiaobao.xyz/Article/details/gipumsidh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxoxmilu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glaxqgwtt.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvnjkoklv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.fanxiaobao.xyz/Article/details/ggzbfsyfq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.fanxiaobao.xyz/Article/details/gctqobetm.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjafcgqo.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxnbidqv.sHtML

[F04] 追加写入文件
来源：http://www.share.fanxiaobao.xyz/Article/details/glexjgdne.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fanxiaobao.xyz/Article/details/gibcntrzh.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.fanxiaobao.xyz/Article/details/gwwzpqozx.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnfaeylwm.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fanxiaobao.xyz/Article/details/gdkycjwvk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.fanxiaobao.xyz/Article/details/gjxyzsxiu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fanxiaobao.xyz/Article/details/gdicmdbjo.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gteevdtco.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzfccaxx.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgrlugpj.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.fanxiaobao.xyz/Article/details/gspjfbukm.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.fanxiaobao.xyz/Article/details/gfnjqtadm.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggawvimed.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/giidbamsb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggijnzvbj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.fanxiaobao.xyz/Article/details/gczgmcslz.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gjjcytiok.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gqltywhxz.sHtML

[F06] 删除文件
来源：http://blog.fanxiaobao.xyz/Article/details/gxosoajnp.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gayyglfvm.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fanxiaobao.xyz/Article/details/gdprryxid.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfkbhzxn.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfeildso.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.fanxiaobao.xyz/Article/details/ghhfghlxy.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/grcwmopqv.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/ghylyjsrj.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/geearcuok.sHtML

[F07] 创建目录（含多级）
来源：http://wap.fanxiaobao.xyz/Article/details/gxmzxogwl.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.fanxiaobao.xyz/Article/details/gxtznfrso.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghraweodz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fanxiaobao.xyz/Article/details/gymnfzmul.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fanxiaobao.xyz/Article/details/govchrkyg.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzhgezha.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyfxbmlkn.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.fanxiaobao.xyz/Article/details/gucaiuebg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfjgypuf.sHtML

[F08] 遍历目录
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnstpaeog.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjctfdam.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grufzhrxf.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.fanxiaobao.xyz/Article/details/ghznjblxl.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gccwilwqd.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnafxqji.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.fanxiaobao.xyz/Article/details/gcstmvogz.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.fanxiaobao.xyz/Article/details/gbyyzbsbz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjvxsfqj.sHtML

[F09] 获取文件大小
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxzrbkci.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/glfmntqvy.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/gikakrkfm.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.fanxiaobao.xyz/Article/details/gvagfcdbc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fanxiaobao.xyz/Article/details/gikqvmrzy.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fanxiaobao.xyz/Article/details/gewpaktmr.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geukvsutr.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gdayumubc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdcptxvh.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fanxiaobao.xyz/Article/details/gonxrabbc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gmgslkpnv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkwixayj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gunyhurve.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gyodwumhs.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fanxiaobao.xyz/Article/details/gyjxorygh.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpnvymis.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gtykbmraw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gqesyeprh.sHtML

[F11] 复制与移动文件
来源：http://baike.fanxiaobao.xyz/Article/details/gnflbaftt.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/groxdzfzh.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.fanxiaobao.xyz/Article/details/gdpdafukh.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gbvburiqs.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gbsfimrru.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.fanxiaobao.xyz/Article/details/gdnwwyuir.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsbkkypmo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gptwskxyt.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtzcatpqt.sHtML

[F12] CSV 读写
来源：http://wap.fanxiaobao.xyz/Article/details/gsvgrchrw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcntjblfc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdsrkams.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fanxiaobao.xyz/Article/details/gzyptdatp.sHtML

TS:   // 同上
来源：http://blog.fanxiaobao.xyz/Article/details/gpqekqkdi.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gupojahma.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibeiupxh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gilqbyoim.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.fanxiaobao.xyz/Article/details/gbfmbvwyy.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbgzxzmw.sHtML

G. 面向对象
来源：http://m.share.fanxiaobao.xyz/Article/details/gumcvuptj.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvttmlopp.sHtML

[G01] 定义类
来源：http://www.share.fanxiaobao.xyz/Article/details/gaiijwekv.sHtML

Py:   class User: pass
来源：http://read.share.fanxiaobao.xyz/Article/details/gehzpsnnv.sHtML

PHP:  class User {}
来源：http://m.share.fanxiaobao.xyz/Article/details/glgaysrsh.sHtML

JS:   class User {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghckllejv.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtuggkpc.sHtML

Java: class User {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvphvetp.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fanxiaobao.xyz/Article/details/guikgaaef.sHtML

Ruby: class User; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gosaxjzyc.sHtML

C#:   class User {}
来源：http://3g.fanxiaobao.xyz/Article/details/gvejhnzdq.sHtML

[G02] 构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzarbyew.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fanxiaobao.xyz/Article/details/grxdvgcuw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpsyaayn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpubapllw.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmmtpoli.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gzbrffoab.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkykoeyr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gjaetbgog.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjglkmqtx.sHtML

[G03] 实例属性
来源：http://mobile.fanxiaobao.xyz/Article/details/gdlfykvxd.sHtML

Py:   self.name = "x"
来源：http://www.share.fanxiaobao.xyz/Article/details/gvziephvi.sHtML

PHP:  public string $name = "x";
来源：http://wap.fanxiaobao.xyz/Article/details/gutgcuzvc.sHtML

JS:   this.name = "x";
来源：http://wap.fanxiaobao.xyz/Article/details/gpknqyzeh.sHtML

TS:   name: string = "x";
来源：http://3g.fanxiaobao.xyz/Article/details/gnxcmgwbm.sHtML

Java: private String name;
来源：http://3g.fanxiaobao.xyz/Article/details/gfpfzgizq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fanxiaobao.xyz/Article/details/grzsylatw.sHtML

Ruby: @name = "x"
来源：http://mobile.fanxiaobao.xyz/Article/details/gyulhzlqs.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fanxiaobao.xyz/Article/details/gditcdjuk.sHtML

[G04] 定义方法
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlptjado.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fanxiaobao.xyz/Article/details/goufruchx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjgvcbsn.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fanxiaobao.xyz/Article/details/geybfwdfm.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gntmiwabs.sHtML

Java: String greet() { return name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gcawrwnxq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwxffbba.sHtML

Ruby: def greet; @name; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjftbbsp.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fanxiaobao.xyz/Article/details/gnmopexou.sHtML

[G05] 继承
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpjwmljq.sHtML

Py:   class Admin(User): pass
来源：http://blog.fanxiaobao.xyz/Article/details/gbkbqldwo.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fanxiaobao.xyz/Article/details/gxieitwuh.sHtML

JS:   class Admin extends User {}
来源：http://wap.fanxiaobao.xyz/Article/details/gwkilhzhh.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggcvtovxk.sHtML

Java: class Admin extends User {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdkxycsh.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.fanxiaobao.xyz/Article/details/gtseeuszz.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqoascmk.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsycjnhdf.sHtML

[G06] 重写方法
来源：http://baike.fanxiaobao.xyz/Article/details/ghxaduuit.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fanxiaobao.xyz/Article/details/gbrxpvbqk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/guitgbpvx.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctrkxnxq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjjwitwgy.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzekanrk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.fanxiaobao.xyz/Article/details/gzpfqewwa.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmhtfxlh.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fanxiaobao.xyz/Article/details/geuswsthc.sHtML

[G07] 调用父类方法
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahiiigjh.sHtML

Py:   super().greet()
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwqmomhs.sHtML

PHP:  parent::greet();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstrudnvh.sHtML

JS:   super.greet();
来源：http://baike.fanxiaobao.xyz/Article/details/gqjooopeq.sHtML

TS:   super.greet();
来源：http://wap.fanxiaobao.xyz/Article/details/ggslqobin.sHtML

Java: super.greet();
来源：http://mobile.fanxiaobao.xyz/Article/details/gzekzkaxp.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fanxiaobao.xyz/Article/details/ggyreryvg.sHtML

Ruby: super
来源：http://wap.fanxiaobao.xyz/Article/details/guwfdliem.sHtML

C#:   base.Greet();
来源：http://m.share.fanxiaobao.xyz/Article/details/govgqwded.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqodhwpsj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxeoimtz.sHtML

PHP:  public static function f() {}
来源：http://3g.fanxiaobao.xyz/Article/details/gjlckjxak.sHtML

JS:   static f() {}
来源：http://blog.fanxiaobao.xyz/Article/details/gqdiqsxkr.sHtML

TS:   static f(): void {}
来源：http://read.share.fanxiaobao.xyz/Article/details/grxfhpwjg.sHtML

Java: static void f() {}
来源：http://blog.fanxiaobao.xyz/Article/details/gkjutxjvl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fanxiaobao.xyz/Article/details/gaojrtipr.sHtML

Ruby: def self.f; end
来源：http://blog.fanxiaobao.xyz/Article/details/gjwampusp.sHtML

C#:   public static void F() {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gwitpgsyr.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvlfueoz.sHtML


<!-- 参考信息 -->