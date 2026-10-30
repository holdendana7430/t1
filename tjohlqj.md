代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.fehbvm.com/Article/details/gjtosdpam.sHtML

TS:   s.split(",")
来源：http://3g.hesvh.cn/Article/details/gqnzyquso.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.hesvh.cn/Article/details/gxapllozd.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.hesvh.cn/Article/details/geeltjlav.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.fehbvm.com/Article/details/gmmaoyixl.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.zdbjq.cn/Article/details/gsbitsovz.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.hesvh.cn/Article/details/giufaeykk.sHtML

Py:   ",".join(items)
来源：http://read.share.fehbvm.com/Article/details/gxprnnaui.sHtML

PHP:  implode(",", $items);
来源：http://blog.fehbvm.com/Article/details/gqvtxyqlx.sHtML

JS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gwyarvgeu.sHtML

TS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gzzxczyga.sHtML

Java: String.join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gdrhripog.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.zdbjq.cn/Article/details/gjnulykuu.sHtML

Ruby: items.join(",")
来源：http://blog.fehbvm.com/Article/details/gssmkybca.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/ggaccmube.sHtML

[E09] 去除所有空白字符
来源：http://wap.zdbjq.cn/Article/details/gfkcgqpbs.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.fehbvm.com/Article/details/gszlyifah.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gbtwlqxtk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/glrvtmxsi.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gvfhofupd.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gmhkklsmp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.fehbvm.com/Article/details/ghkduttej.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.hesvh.cn/Article/details/gjffalcec.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.hesvh.cn/Article/details/gytinlxbz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.fehbvm.com/Article/details/gvyqgvubg.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gwcgxoqdk.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fehbvm.com/Article/details/gywcdufxf.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gblhglmio.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gopwkaran.sHtML

Java: String.format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gdpetuojs.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gvezkhxpc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gebwrgoin.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.fehbvm.com/Article/details/gkrxkrkon.sHtML

[E11] 反转字符串
来源：http://blog.fehbvm.com/Article/details/gulcdsnju.sHtML

Py:   s[::-1]
来源：http://3g.fehbvm.com/Article/details/gvtpgoztc.sHtML

PHP:  strrev($s);
来源：http://blog.hesvh.cn/Article/details/ghyvgnqfq.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/glyqfpbrs.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gcylgqhui.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.zdbjq.cn/Article/details/gghnrwgeh.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/gnietorof.sHtML

Ruby: s.reverse
来源：http://baike.zdbjq.cn/Article/details/gdatzzbqw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gubpssivo.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.fehbvm.com/Article/details/gjvsjttke.sHtML

Py:   s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/gpfaeogyc.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.zdbjq.cn/Article/details/ghvugfbys.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/geoghxyct.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/glzzurxfq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.hesvh.cn/Article/details/gjutqrtxv.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.hesvh.cn/Article/details/gghwnjxrh.sHtML

Ruby: s.count("a")
来源：http://mobile.hesvh.cn/Article/details/gyepibsag.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.zdbjq.cn/Article/details/govbljpic.sHtML

[E13] 逐字符遍历
来源：http://wap.fehbvm.com/Article/details/gwiagomvo.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.hesvh.cn/Article/details/glfevaxjj.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.zdbjq.cn/Article/details/gqpjffdig.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gevpftosi.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/gtskszrhb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.fehbvm.com/Article/details/gzjqmgirf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.zdbjq.cn/Article/details/ggqufdycc.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.hesvh.cn/Article/details/gkyfqnjvw.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.fehbvm.com/Article/details/geszuiksr.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.fehbvm.com/Article/details/gykwtgkal.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.hesvh.cn/Article/details/gfckmppdq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.fehbvm.com/Article/details/gzcfjvvzx.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.hesvh.cn/Article/details/gjuayfrby.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.hesvh.cn/Article/details/gemxftloe.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.zdbjq.cn/Article/details/grfxsdaqa.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.hesvh.cn/Article/details/gzjvvwetq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.fehbvm.com/Article/details/gsftsztem.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.hesvh.cn/Article/details/gpkjfnmpp.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.zdbjq.cn/Article/details/gqpbfmrlp.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.hesvh.cn/Article/details/ghhxkzbyf.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.zdbjq.cn/Article/details/gkecmpeon.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.hesvh.cn/Article/details/gndnyiauz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.hesvh.cn/Article/details/gxerhrtev.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.zdbjq.cn/Article/details/ghluohiwn.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.hesvh.cn/Article/details/gwulrwzdm.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.fehbvm.com/Article/details/gxynajjdr.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.hesvh.cn/Article/details/gojqkepfr.sHtML

[E16] 数字千分位
来源：http://wap.fehbvm.com/Article/details/gwmksrmfn.sHtML

Py:   f"{1234567:,}"
来源：http://blog.fehbvm.com/Article/details/gfkqqocfi.sHtML

PHP:  number_format(1234567);
来源：http://wap.fehbvm.com/Article/details/ggsaqkfiu.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/gzrxbbjyx.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/gqyhcpdzv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.fehbvm.com/Article/details/gbkjgkqcr.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.hesvh.cn/Article/details/gbhvaflll.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.fehbvm.com/Article/details/gqnqahtho.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.zdbjq.cn/Article/details/gfkybpsvc.sHtML

[E17] 首字母大写
来源：http://wap.hesvh.cn/Article/details/gshdcdeph.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.hesvh.cn/Article/details/gdvpsfypj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.zdbjq.cn/Article/details/gsegtbdnc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/gyuxqgygn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/ganhajsou.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fehbvm.com/Article/details/givlozeqf.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.zdbjq.cn/Article/details/guvtzzzvl.sHtML

Ruby: s.capitalize
来源：http://baike.fehbvm.com/Article/details/gmmaszgii.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fehbvm.com/Article/details/gqlmpapwt.sHtML

[E18] 模板占位符替换
来源：http://wap.hesvh.cn/Article/details/gtemufpya.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.hesvh.cn/Article/details/ghepspjhm.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.hesvh.cn/Article/details/gbhvfdojq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/ggjillexe.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gpxwgfzfb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/giwzcwvmy.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.hesvh.cn/Article/details/gitlfvycc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.zdbjq.cn/Article/details/gvjlkmcao.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.hesvh.cn/Article/details/gepdjvbjd.sHtML

[E19] 多行文本按行拆分
来源：http://wap.fehbvm.com/Article/details/grbdzktph.sHtML

Py:   s.splitlines()
来源：http://www.m.share.hesvh.cn/Article/details/ghlxputqi.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gagxbndul.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/gdajnmzrv.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/gseprphwi.sHtML

Java: s.lines().toList()
来源：http://blog.fehbvm.com/Article/details/guyzwwond.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.hesvh.cn/Article/details/glglhhges.sHtML

Ruby: s.lines
来源：http://www.share.zdbjq.cn/Article/details/gfhnbkhrw.sHtML

C#:   s.Split('\n')
来源：http://mobile.hesvh.cn/Article/details/gzawqlpht.sHtML

[E20] 判断字符串是否为空
来源：http://3g.zdbjq.cn/Article/details/gbgozfwjg.sHtML

Py:   if not s:
来源：http://baike.zdbjq.cn/Article/details/ggympvkcm.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.fehbvm.com/Article/details/gkotxfwez.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fehbvm.com/Article/details/guaitiiif.sHtML

TS:   if (s === "") {}
来源：http://baike.fehbvm.com/Article/details/giomiadxn.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.fehbvm.com/Article/details/gmcpaimqq.sHtML

Go:   if s == "" {}
来源：http://www.m.share.zdbjq.cn/Article/details/glgjjhtme.sHtML

Ruby: if s.empty?
来源：http://mobile.zdbjq.cn/Article/details/giioicqlf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.fehbvm.com/Article/details/gekyozhae.sHtML

[E21] 超长截断加省略号
来源：http://blog.fehbvm.com/Article/details/gjjenbred.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.zdbjq.cn/Article/details/gwqyllrsb.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gwjikcuij.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gletorwly.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/grdltwwvv.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gxkmrletx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.zdbjq.cn/Article/details/glbexlzen.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/geyzmmmfg.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/ggetleeai.sHtML

[E22] 字节长度与字符长度
来源：http://wap.zdbjq.cn/Article/details/gxtshdwyb.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.zdbjq.cn/Article/details/gixvehftx.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gfldlmqmr.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/gcathtrjy.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/gooypyhed.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.hesvh.cn/Article/details/gluucfkan.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.zdbjq.cn/Article/details/glawrjprb.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gkpsnfbfn.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.hesvh.cn/Article/details/glhslmczs.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gyfdkplhk.sHtML

F. 文件与目录
来源：http://m.share.zdbjq.cn/Article/details/gshvvwucu.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gurgphann.sHtML

[F01] 读取整个文件
来源：http://3g.fehbvm.com/Article/details/gkusbsygk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.fehbvm.com/Article/details/ggcbuvlkg.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.fehbvm.com/Article/details/gavnghcml.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.zdbjq.cn/Article/details/gaahyjtmw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.hesvh.cn/Article/details/glbeeqrdn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gnvnycomv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.hesvh.cn/Article/details/gouzmkzpx.sHtML

Ruby: File.read("a.txt")
来源：http://wap.fehbvm.com/Article/details/gekndowhv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gfnkwdjul.sHtML

[F02] 逐行读取文件
来源：http://baike.zdbjq.cn/Article/details/gjtlvcfzf.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.hesvh.cn/Article/details/gcvrroxjo.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.fehbvm.com/Article/details/gwfsofmme.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/gbdqlxygy.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/gynzgddvm.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gltbkkepr.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.zdbjq.cn/Article/details/gedfkjtob.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.fehbvm.com/Article/details/ghjpiyeth.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.zdbjq.cn/Article/details/gerzjjvsv.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.zdbjq.cn/Article/details/gnhwmgxvz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.zdbjq.cn/Article/details/gwkbjypjh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gyuaqjwlr.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gnuljtqxf.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/gdjhlyvqr.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.zdbjq.cn/Article/details/gvdjdvgei.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.fehbvm.com/Article/details/gyooohtcf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.hesvh.cn/Article/details/gitgomfef.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/ghuyyidqw.sHtML

[F04] 追加写入文件
来源：http://m.share.zdbjq.cn/Article/details/gpmmclkzj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.zdbjq.cn/Article/details/gjvtrsnqm.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.hesvh.cn/Article/details/gpoxywwsg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gkyvfdnwr.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gjvnrkitl.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.hesvh.cn/Article/details/gsdgmmumu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.zdbjq.cn/Article/details/gehyyrtuu.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fehbvm.com/Article/details/govmqodec.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fehbvm.com/Article/details/gnoljlavl.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.fehbvm.com/Article/details/gnvjggprx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.hesvh.cn/Article/details/gtdlqazui.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.fehbvm.com/Article/details/gdpfrlbhr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gypwawtna.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gvdvxnhjp.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gshqlmiec.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.fehbvm.com/Article/details/gsvvqkzqw.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.hesvh.cn/Article/details/gefjvozxp.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gqfhmyyxp.sHtML

[F06] 删除文件
来源：http://m.share.zdbjq.cn/Article/details/gzecghxzw.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gmdjmjdrs.sHtML

PHP:  unlink("a.txt");
来源：http://blog.hesvh.cn/Article/details/gszdbsokn.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gzyrshias.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gdemnttpz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gayuinwkz.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gjqzppcui.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gzvbopdnx.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.zdbjq.cn/Article/details/ggeivvlnw.sHtML

[F07] 创建目录（含多级）
来源：http://blog.fehbvm.com/Article/details/gxtoeiioi.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gvbzxvqnn.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.zdbjq.cn/Article/details/gnfcwuavz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/gamwbmteq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gmfpbnkjc.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.zdbjq.cn/Article/details/gdmiwdmxo.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.zdbjq.cn/Article/details/gpqlgmuay.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.fehbvm.com/Article/details/gbhprxrph.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.zdbjq.cn/Article/details/glioqqrdt.sHtML

[F08] 遍历目录
来源：http://www.m.share.fehbvm.com/Article/details/gvhbgopov.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.hesvh.cn/Article/details/gtoutqzlg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.zdbjq.cn/Article/details/gdmwqccox.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gproqjijw.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/ghqvgwgtk.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gdqvbuczi.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gurfinibj.sHtML

Ruby: Dir.children("dir")
来源：http://3g.zdbjq.cn/Article/details/gphsaoqut.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.zdbjq.cn/Article/details/gltcgwcxx.sHtML

[F09] 获取文件大小
来源：http://wap.fehbvm.com/Article/details/gwwbwotoh.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gdmzndegf.sHtML

PHP:  filesize("a.txt");
来源：http://wap.fehbvm.com/Article/details/gxpjzlrug.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gvmtlcvkd.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gyjxpxmkq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/ggceaseua.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.hesvh.cn/Article/details/gnmqjcfxa.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.hesvh.cn/Article/details/goubcmwug.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.fehbvm.com/Article/details/gxonpklzd.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.fehbvm.com/Article/details/grsmtntsd.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gmcujswlm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.hesvh.cn/Article/details/gwlswvqis.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gemiroomg.sHtML

TS:   path.extname("a.txt")
来源：http://wap.hesvh.cn/Article/details/gaqorfcef.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.hesvh.cn/Article/details/gdixycnov.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/goqcctjue.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gjddndtni.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gldcrcqzl.sHtML

[F11] 复制与移动文件
来源：http://mobile.fehbvm.com/Article/details/gmemtdjes.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gmqlpmmoa.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gmkvlcgds.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gjyoopuqf.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gopulsgam.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.hesvh.cn/Article/details/gbgjifhpv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.hesvh.cn/Article/details/gnleijkfc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gmnezzudb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.hesvh.cn/Article/details/getxqbqyg.sHtML

[F12] CSV 读写
来源：http://3g.hesvh.cn/Article/details/guamesdrl.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.zdbjq.cn/Article/details/gkupjexkn.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.zdbjq.cn/Article/details/gnywahvyu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.fehbvm.com/Article/details/gvvawpzdb.sHtML

TS:   // 同上
来源：http://3g.hesvh.cn/Article/details/ghjurqbnk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.hesvh.cn/Article/details/gkjlcevib.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.hesvh.cn/Article/details/gouqiujyw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.fehbvm.com/Article/details/gsdupsldm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.fehbvm.com/Article/details/gpqbjgpiy.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gkipnwetq.sHtML

G. 面向对象
来源：http://blog.hesvh.cn/Article/details/gzwyhxksd.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ggyhmkbhr.sHtML

[G01] 定义类
来源：http://m.share.fehbvm.com/Article/details/gftgsxfij.sHtML

Py:   class User: pass
来源：http://wap.zdbjq.cn/Article/details/gueqhbugt.sHtML

PHP:  class User {}
来源：http://mobile.hesvh.cn/Article/details/ghyykdrzr.sHtML

JS:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/gqckblfaf.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.hesvh.cn/Article/details/gqfdjaqgb.sHtML

Java: class User {}
来源：http://www.share.zdbjq.cn/Article/details/gbxbkyubj.sHtML

Go:   type User struct { Name string }
来源：http://wap.hesvh.cn/Article/details/gxdvtlbth.sHtML

Ruby: class User; end
来源：http://read.share.hesvh.cn/Article/details/gvpazchmn.sHtML

C#:   class User {}
来源：http://3g.fehbvm.com/Article/details/gfyksnmqo.sHtML

[G02] 构造函数
来源：http://www.blog.fehbvm.com/Article/details/gghpvrebe.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.zdbjq.cn/Article/details/gatgoucvz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.zdbjq.cn/Article/details/gjsylrnff.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gfwkuilhc.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.fehbvm.com/Article/details/gtwgehrum.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gbsohjycf.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fehbvm.com/Article/details/gqjernwkf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.zdbjq.cn/Article/details/gjxpbslct.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.zdbjq.cn/Article/details/gzlbcvbtx.sHtML

[G03] 实例属性
来源：http://blog.hesvh.cn/Article/details/gxliedolr.sHtML

Py:   self.name = "x"
来源：http://wap.hesvh.cn/Article/details/gffxdqmqi.sHtML

PHP:  public string $name = "x";
来源：http://www.share.fehbvm.com/Article/details/gcdzzaevc.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/gctpiotoh.sHtML

TS:   name: string = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gfsaofxep.sHtML

Java: private String name;
来源：http://m.share.zdbjq.cn/Article/details/gafotsqqv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.zdbjq.cn/Article/details/gsxjvnujt.sHtML

Ruby: @name = "x"
来源：http://blog.zdbjq.cn/Article/details/gthzvwdzv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/gkvvjmufu.sHtML

[G04] 定义方法
来源：http://blog.hesvh.cn/Article/details/gtdymbwpw.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/gvoppdezb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gxrgtckzu.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gtrqwwlwm.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gqdqoarjt.sHtML

Java: String greet() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gbentnmki.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/geegkccqa.sHtML

Ruby: def greet; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gxisoussr.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.fehbvm.com/Article/details/gcmzsjqny.sHtML

[G05] 继承
来源：http://baike.zdbjq.cn/Article/details/gimzssmzd.sHtML

Py:   class Admin(User): pass
来源：http://blog.zdbjq.cn/Article/details/grxbqnled.sHtML

PHP:  class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gkffrzskj.sHtML

JS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gmpaaqzdo.sHtML

TS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/grwncakgf.sHtML

Java: class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gydeuwigw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.zdbjq.cn/Article/details/ghqkrmtmh.sHtML

Ruby: class Admin < User; end
来源：http://blog.hesvh.cn/Article/details/gbwyczyna.sHtML

C#:   class Admin : User {}
来源：http://baike.zdbjq.cn/Article/details/gquhurcka.sHtML


<!-- 参考信息 -->