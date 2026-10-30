代发 wailian999

PHP:  implode(",", $items);
来源：http://m.share.fanxiaobao.xyz/Article/details/gydbhlevk.sHtML

JS:   items.join(",")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnszzxvrd.sHtML

TS:   items.join(",")
来源：http://www.share.fanxiaobao.xyz/Article/details/ggaawufus.sHtML

Java: String.join(",", items)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmnzizyu.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.fanxiaobao.xyz/Article/details/grmhsikyw.sHtML

Ruby: items.join(",")
来源：http://m.share.fanxiaobao.xyz/Article/details/gatidyjvx.sHtML

C#:   string.Join(",", items)
来源：http://m.share.fanxiaobao.xyz/Article/details/gahrlsbtb.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkqggepk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.fanxiaobao.xyz/Article/details/gkcojukam.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.fanxiaobao.xyz/Article/details/geolucbji.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxiigblw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fanxiaobao.xyz/Article/details/geffneosi.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.fanxiaobao.xyz/Article/details/guweiflyw.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.fanxiaobao.xyz/Article/details/gblnpnzfq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.fanxiaobao.xyz/Article/details/gesistlfc.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.fanxiaobao.xyz/Article/details/gcgkmsyqw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.fanxiaobao.xyz/Article/details/gudgjecjm.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.fanxiaobao.xyz/Article/details/grlgkgscz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.fanxiaobao.xyz/Article/details/giceudvav.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnleywrvb.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.fanxiaobao.xyz/Article/details/gmmdhhmbr.sHtML

Java: String.format("%03d", 7)
来源：http://3g.fanxiaobao.xyz/Article/details/gwnypjnsi.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjotmjau.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fanxiaobao.xyz/Article/details/gofsevksa.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.fanxiaobao.xyz/Article/details/goonvwxmw.sHtML

[E11] 反转字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gckgcmxrt.sHtML

Py:   s[::-1]
来源：http://m.share.fanxiaobao.xyz/Article/details/grgcpncxy.sHtML

PHP:  strrev($s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxzfpffu.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.fanxiaobao.xyz/Article/details/guqsjjiaf.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.fanxiaobao.xyz/Article/details/gmryxmloi.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfdcdfpb.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.fanxiaobao.xyz/Article/details/gllyrroud.sHtML

Ruby: s.reverse
来源：http://wap.fanxiaobao.xyz/Article/details/gmhtodksj.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.fanxiaobao.xyz/Article/details/gtoqvczzm.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhhtuxsx.sHtML

Py:   s.count("a")
来源：http://baike.fanxiaobao.xyz/Article/details/garngouwc.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.fanxiaobao.xyz/Article/details/gaydtnzom.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtyienln.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fanxiaobao.xyz/Article/details/gcradxvze.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.fanxiaobao.xyz/Article/details/gnayskfpn.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjnntohn.sHtML

Ruby: s.count("a")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvpthxiv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.fanxiaobao.xyz/Article/details/gvoraekri.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grbcryqru.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.fanxiaobao.xyz/Article/details/gjuxhyfob.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.fanxiaobao.xyz/Article/details/gzvcstefg.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fanxiaobao.xyz/Article/details/gedsydxlg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fanxiaobao.xyz/Article/details/gphwvfesz.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.fanxiaobao.xyz/Article/details/ghikbrhmb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gxamysxlk.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.fanxiaobao.xyz/Article/details/gpkqgcafe.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbprlvzb.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gubaqrhkq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.fanxiaobao.xyz/Article/details/gfrlyctrx.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.fanxiaobao.xyz/Article/details/geajpqedq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdlvqata.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gacqakftv.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.fanxiaobao.xyz/Article/details/gndjheegd.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.fanxiaobao.xyz/Article/details/geojgpyxu.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.fanxiaobao.xyz/Article/details/gwaobrbdh.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaejygbqd.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fanxiaobao.xyz/Article/details/gjmbiroac.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fanxiaobao.xyz/Article/details/genxxpwra.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxuajoak.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwasvmlr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gewdkqity.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.fanxiaobao.xyz/Article/details/guoijrhkk.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpeadcjr.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gmentophf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gpzrhbnzy.sHtML

[E16] 数字千分位
来源：http://3g.fanxiaobao.xyz/Article/details/gqsoofiby.sHtML

Py:   f"{1234567:,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gyemewwrb.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgxdudlv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxejketf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.fanxiaobao.xyz/Article/details/glrixdtsh.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzmltchs.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.fanxiaobao.xyz/Article/details/gkyrbkdli.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grhfeeval.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.fanxiaobao.xyz/Article/details/groylmfhb.sHtML

[E17] 首字母大写
来源：http://mobile.fanxiaobao.xyz/Article/details/gtysvxlrg.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjqtvmzc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvxtlpgy.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/geqxagrwq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gfplfydge.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.fanxiaobao.xyz/Article/details/gocovumzp.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.fanxiaobao.xyz/Article/details/giyyjeurv.sHtML

Ruby: s.capitalize
来源：http://3g.fanxiaobao.xyz/Article/details/gwubncsmv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.fanxiaobao.xyz/Article/details/gbjbltknf.sHtML

[E18] 模板占位符替换
来源：http://baike.fanxiaobao.xyz/Article/details/gvnjukjyw.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.fanxiaobao.xyz/Article/details/gzadduavn.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjkjanji.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdelyepkl.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvizlhpnm.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqhpiohu.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubwsyrso.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gkcqsibfv.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbtfavvb.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezohjvdv.sHtML

Py:   s.splitlines()
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzkpxyvj.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.fanxiaobao.xyz/Article/details/gbeuvvxvy.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggasxgprm.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fanxiaobao.xyz/Article/details/gjxbcgrjt.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvzsidpx.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvhtuiss.sHtML

Ruby: s.lines
来源：http://3g.fanxiaobao.xyz/Article/details/gykqtzntc.sHtML

C#:   s.Split('\n')
来源：http://mobile.fanxiaobao.xyz/Article/details/gffybfrti.sHtML

[E20] 判断字符串是否为空
来源：http://wap.fanxiaobao.xyz/Article/details/gazuqmadd.sHtML

Py:   if not s:
来源：http://m.share.fanxiaobao.xyz/Article/details/gdzwkpblj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqzpsxkw.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.fanxiaobao.xyz/Article/details/guarwvjlh.sHtML

TS:   if (s === "") {}
来源：http://baike.fanxiaobao.xyz/Article/details/geikcebtq.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gjavaccux.sHtML

Go:   if s == "" {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldsshfen.sHtML

Ruby: if s.empty?
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemrwmtce.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyzxcxrzi.sHtML

[E21] 超长截断加省略号
来源：http://baike.fanxiaobao.xyz/Article/details/gaujwirki.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.fanxiaobao.xyz/Article/details/goskykvji.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.fanxiaobao.xyz/Article/details/ghxtkjirq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fanxiaobao.xyz/Article/details/ggeimofig.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktfuobnu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzgyelxwu.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.fanxiaobao.xyz/Article/details/guaacdzoh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrvxilid.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.fanxiaobao.xyz/Article/details/gmbhoapor.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gtyrhqikf.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gpbtityeo.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fanxiaobao.xyz/Article/details/givjfkfno.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fanxiaobao.xyz/Article/details/gouqzkqkh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gdydvonhj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.fanxiaobao.xyz/Article/details/gotqiavda.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.fanxiaobao.xyz/Article/details/gjkokxwbb.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbwakocei.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.fanxiaobao.xyz/Article/details/gbqivurlp.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gibvnxway.sHtML

F. 文件与目录
来源：http://baike.fanxiaobao.xyz/Article/details/gipbyxubp.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxuyiklw.sHtML

[F01] 读取整个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gjnttbaun.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.fanxiaobao.xyz/Article/details/gidpiihgj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjzoudby.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfjrjzpg.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.fanxiaobao.xyz/Article/details/gqqypzvaj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.fanxiaobao.xyz/Article/details/gvromogfv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwjdopzc.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrvkskpt.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gamzkttkt.sHtML

[F02] 逐行读取文件
来源：http://baike.fanxiaobao.xyz/Article/details/gwmyvohmk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.fanxiaobao.xyz/Article/details/grogsaues.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsaklkrxj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gcutwuvop.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgwgbcfa.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwbrxbwx.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvtmtjsm.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpsdixjgx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.fanxiaobao.xyz/Article/details/gcoolupub.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.fanxiaobao.xyz/Article/details/gfkbjehzy.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrosxhug.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gvjjifdlw.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fanxiaobao.xyz/Article/details/gobdrdrvf.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fanxiaobao.xyz/Article/details/guqiswusr.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.fanxiaobao.xyz/Article/details/givrxwprr.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.fanxiaobao.xyz/Article/details/gclrjgzli.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.fanxiaobao.xyz/Article/details/gsljpprvp.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzpuzguf.sHtML

[F04] 追加写入文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/grnhgdham.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.fanxiaobao.xyz/Article/details/grdpqsyfo.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.fanxiaobao.xyz/Article/details/gelmibdsh.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fanxiaobao.xyz/Article/details/gvrrjcavo.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlffzjjy.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpemzryv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fanxiaobao.xyz/Article/details/gldfiyqsc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvctuaqq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.fanxiaobao.xyz/Article/details/ggrqkzujw.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goybvngjh.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgtnnnuf.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.fanxiaobao.xyz/Article/details/gjatspqgy.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gtkrgdaau.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gqzuybmuu.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxnerjzf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsanktqfw.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbmdwbwv.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gihregimh.sHtML

[F06] 删除文件
来源：http://wap.fanxiaobao.xyz/Article/details/gromyvukt.sHtML

Py:   os.remove("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gpjexzsat.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqqjrllt.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goabemkvp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjgmljnt.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgwihzxn.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gpukuuwab.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gihyzrjlo.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/gahfsqpws.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.fanxiaobao.xyz/Article/details/gfeitgknh.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.fanxiaobao.xyz/Article/details/gcepgmtan.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.fanxiaobao.xyz/Article/details/grnqnfhcj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fanxiaobao.xyz/Article/details/gieuuokbl.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fanxiaobao.xyz/Article/details/gdrerwuek.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.fanxiaobao.xyz/Article/details/ggqngphlj.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkcfboyn.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.fanxiaobao.xyz/Article/details/gpjtuykwy.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.fanxiaobao.xyz/Article/details/guxxgpcjp.sHtML

[F08] 遍历目录
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqotjsgmv.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.fanxiaobao.xyz/Article/details/gapebwpuy.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmtnxyvz.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.fanxiaobao.xyz/Article/details/gxkzzbazf.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fanxiaobao.xyz/Article/details/gxcfchkra.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fanxiaobao.xyz/Article/details/grjhvhclb.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fanxiaobao.xyz/Article/details/godsxaahd.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnfpkurk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.fanxiaobao.xyz/Article/details/gnafejrkn.sHtML

[F09] 获取文件大小
来源：http://wap.fanxiaobao.xyz/Article/details/gvfzitzfm.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gwnjuwsxu.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmxmbedh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwkzgbtj.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fanxiaobao.xyz/Article/details/gfxsqvxsp.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.fanxiaobao.xyz/Article/details/guvfbmwmg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fanxiaobao.xyz/Article/details/gokgvxklf.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghcvlijur.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gueoaezhu.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.fanxiaobao.xyz/Article/details/gfmrgtmyf.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gybcjicog.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gezbzjnzj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gfqtihwmc.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgehljhb.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.fanxiaobao.xyz/Article/details/gczsphfgq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzfvxjph.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grecuhmca.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfclimikc.sHtML

[F11] 复制与移动文件
来源：http://wap.fanxiaobao.xyz/Article/details/gtzpyagpj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gytlfteul.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/geljpxusr.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvvaksmz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gbynevkms.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvevbapz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzpqtkdt.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gwohdoxwr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.fanxiaobao.xyz/Article/details/gclbtbhgv.sHtML

[F12] CSV 读写
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmbcamig.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdbquxij.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.fanxiaobao.xyz/Article/details/gobslomjr.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.fanxiaobao.xyz/Article/details/gnlkplhos.sHtML

TS:   // 同上
来源：http://www.blog.fanxiaobao.xyz/Article/details/gauzwmlxw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fanxiaobao.xyz/Article/details/ghsmoklui.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.fanxiaobao.xyz/Article/details/gppyxpzjf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvaqgceiu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fanxiaobao.xyz/Article/details/gfcjkjlto.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gxpnosgby.sHtML

G. 面向对象
来源：http://baike.fanxiaobao.xyz/Article/details/gcjdhxhoz.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gwdpkfwkv.sHtML

[G01] 定义类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrqhgksf.sHtML

Py:   class User: pass
来源：http://www.share.fanxiaobao.xyz/Article/details/ghdckhzpy.sHtML

PHP:  class User {}
来源：http://baike.fanxiaobao.xyz/Article/details/gvnlyhznz.sHtML

JS:   class User {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gawrwkxfw.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.fanxiaobao.xyz/Article/details/gsqpkmuez.sHtML

Java: class User {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaglunhje.sHtML

Go:   type User struct { Name string }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfajaita.sHtML

Ruby: class User; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gorsjsukm.sHtML

C#:   class User {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjsurysg.sHtML

[G02] 构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/gbbhszwlv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxopstdzk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gprlzzewl.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohcynnbw.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlnsliff.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxvydcgx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtcnfaqj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqggbmyo.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gxgmjhgfx.sHtML

[G03] 实例属性
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpmyhjuq.sHtML

Py:   self.name = "x"
来源：http://wap.fanxiaobao.xyz/Article/details/gpapngwls.sHtML

PHP:  public string $name = "x";
来源：http://baike.fanxiaobao.xyz/Article/details/gplzwagzs.sHtML

JS:   this.name = "x";
来源：http://www.share.fanxiaobao.xyz/Article/details/gfemfeohb.sHtML

TS:   name: string = "x";
来源：http://mobile.fanxiaobao.xyz/Article/details/ghsyrcgla.sHtML

Java: private String name;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdstgfebv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fanxiaobao.xyz/Article/details/gxeyqiwko.sHtML

Ruby: @name = "x"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjrsrtzm.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fanxiaobao.xyz/Article/details/gtduiuury.sHtML

[G04] 定义方法
来源：http://blog.fanxiaobao.xyz/Article/details/gxpxdilru.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fanxiaobao.xyz/Article/details/gxavgyekg.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gblxddnfw.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gwpmhymqk.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfcmcxxt.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gryiijjyh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gginijfeh.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwyvffcnl.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpufgxdri.sHtML

[G05] 继承
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhlpsroq.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fanxiaobao.xyz/Article/details/gqwwhdaio.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvnsokqz.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnuhvgsdl.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjzzdvry.sHtML

Java: class Admin extends User {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqotixpv.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glyzyzvuj.sHtML

Ruby: class Admin < User; end
来源：http://baike.fanxiaobao.xyz/Article/details/gniiacgav.sHtML

C#:   class Admin : User {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gqsnnaasb.sHtML

[G06] 重写方法
来源：http://baike.fanxiaobao.xyz/Article/details/gxzmzyrdz.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.fanxiaobao.xyz/Article/details/ggbpfctmt.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gasrieqnr.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/giucssxmb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbntbgxh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gtjnqisrd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fanxiaobao.xyz/Article/details/gdanqtqdv.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.fanxiaobao.xyz/Article/details/gpfzhcdpu.sHtML


<!-- 参考信息 -->