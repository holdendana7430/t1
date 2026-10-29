代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.fehbvm.com/Article/details/gkwudavwp.sHtML

TS:   s.split(",")
来源：http://www.share.fehbvm.com/Article/details/grrtndqbc.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.fehbvm.com/Article/details/geynhwsuf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.zdbjq.cn/Article/details/gldcivpfp.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.fehbvm.com/Article/details/gpqfhvbmq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.hesvh.cn/Article/details/gkwfiwyyh.sHtML

[E08] 数组按分隔符合并
来源：http://blog.hesvh.cn/Article/details/gazembvhu.sHtML

Py:   ",".join(items)
来源：http://www.blog.hesvh.cn/Article/details/guzycmnwj.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.fehbvm.com/Article/details/gdrkgehmb.sHtML

JS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/gzaoehvrq.sHtML

TS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/glbqqpkbv.sHtML

Java: String.join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/gczayayso.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.fehbvm.com/Article/details/gpxtiwhxk.sHtML

Ruby: items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gqrrsvhep.sHtML

C#:   string.Join(",", items)
来源：http://3g.fehbvm.com/Article/details/gdrvynblv.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.hesvh.cn/Article/details/gvnkfllmo.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.hesvh.cn/Article/details/gqwqphjda.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.zdbjq.cn/Article/details/gtduwdqqq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/gmsoqbcuu.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/ghksflluz.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gbmiilydk.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.hesvh.cn/Article/details/gangevggu.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.fehbvm.com/Article/details/gphekqpmw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/gslyvzjbu.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.hesvh.cn/Article/details/gqwwmjnop.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gzbayvdwo.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.hesvh.cn/Article/details/gzkkrymql.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/glajvfuno.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gvpqqrbip.sHtML

Java: String.format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gzcehaobw.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gdpckqjui.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gtsbroktx.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.fehbvm.com/Article/details/gooekjkwd.sHtML

[E11] 反转字符串
来源：http://baike.hesvh.cn/Article/details/glwrvzlxj.sHtML

Py:   s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gorbxbaqg.sHtML

PHP:  strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gkkghqbza.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/goorpsrfn.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gvcvgpiqo.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.fehbvm.com/Article/details/gxtyqxxiz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.zdbjq.cn/Article/details/gjpdeiyod.sHtML

Ruby: s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gxgyhcrnc.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/ghnwqptbu.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gewdlbjme.sHtML

Py:   s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/gjslczxyr.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.zdbjq.cn/Article/details/gghufuvnf.sHtML

JS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/gxrtcimol.sHtML

TS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/ghvfkudlt.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.hesvh.cn/Article/details/gjwifjggi.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.zdbjq.cn/Article/details/gazgvlevw.sHtML

Ruby: s.count("a")
来源：http://read.share.fehbvm.com/Article/details/gulhokiyk.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.zdbjq.cn/Article/details/gjoidprep.sHtML

[E13] 逐字符遍历
来源：http://wap.zdbjq.cn/Article/details/gufveqpmx.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.hesvh.cn/Article/details/gbdhdcdny.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.fehbvm.com/Article/details/gbnymgrth.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gntmdbrhs.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/gmbhduczu.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.fehbvm.com/Article/details/gvshgmnvk.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.hesvh.cn/Article/details/gdfzhgfpk.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fehbvm.com/Article/details/gloigflvk.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.zdbjq.cn/Article/details/grlemorrr.sHtML

[E14] URL 编码与 Base64
来源：http://wap.hesvh.cn/Article/details/gaqvdmebb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.hesvh.cn/Article/details/gdwcgiqlj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.fehbvm.com/Article/details/geciucxef.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.zdbjq.cn/Article/details/gslwxqjsp.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.zdbjq.cn/Article/details/gpvcxwwrn.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.fehbvm.com/Article/details/geqcjtehk.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.zdbjq.cn/Article/details/ghotdoknh.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.zdbjq.cn/Article/details/gujegkdqg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.zdbjq.cn/Article/details/ggfweuuen.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.hesvh.cn/Article/details/gvvzsodvk.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.fehbvm.com/Article/details/gatxbnbsy.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.zdbjq.cn/Article/details/gdqmrgpkw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gmzjicdjv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.fehbvm.com/Article/details/gyyutctud.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.hesvh.cn/Article/details/gcatbnxzy.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gzlgmiuif.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.hesvh.cn/Article/details/gievvdots.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.hesvh.cn/Article/details/gowacbtkm.sHtML

[E16] 数字千分位
来源：http://mobile.hesvh.cn/Article/details/gmnjrzswh.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.zdbjq.cn/Article/details/ggyiooeon.sHtML

PHP:  number_format(1234567);
来源：http://blog.fehbvm.com/Article/details/gntavqacv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/gijvtaaqh.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/gnsvcppuq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.fehbvm.com/Article/details/garsfovca.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.fehbvm.com/Article/details/gyazgfzkk.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.zdbjq.cn/Article/details/gbcfyoexl.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.fehbvm.com/Article/details/gzjwcpzum.sHtML

[E17] 首字母大写
来源：http://read.share.zdbjq.cn/Article/details/geqxjeqxp.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.hesvh.cn/Article/details/gaucfzoqt.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.fehbvm.com/Article/details/gctojhxly.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gjioupjrf.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/gmecakjuq.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.hesvh.cn/Article/details/gunykoqyd.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.zdbjq.cn/Article/details/gkkrrlhsd.sHtML

Ruby: s.capitalize
来源：http://blog.zdbjq.cn/Article/details/glcgdxsby.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.fehbvm.com/Article/details/gtcnvitec.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fehbvm.com/Article/details/gekeinyre.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.fehbvm.com/Article/details/gczumefrn.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.zdbjq.cn/Article/details/gjcilwsxz.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gcluxzkgr.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gzjnhncxf.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gxhqhsqpp.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.hesvh.cn/Article/details/ggprvlyez.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fehbvm.com/Article/details/gzzaphear.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.zdbjq.cn/Article/details/gxipwiwhe.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fehbvm.com/Article/details/gbpkowzrp.sHtML

Py:   s.splitlines()
来源：http://3g.fehbvm.com/Article/details/gmxtumtfd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.hesvh.cn/Article/details/gzuwscbki.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/gbqvkrpzr.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gvwikdxny.sHtML

Java: s.lines().toList()
来源：http://www.share.fehbvm.com/Article/details/gmjdwmqcv.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.fehbvm.com/Article/details/gdnaehofq.sHtML

Ruby: s.lines
来源：http://www.blog.fehbvm.com/Article/details/gxyunxwgd.sHtML

C#:   s.Split('\n')
来源：http://m.share.hesvh.cn/Article/details/gkdfrnhbh.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.hesvh.cn/Article/details/gsziwtift.sHtML

Py:   if not s:
来源：http://3g.fehbvm.com/Article/details/gmujxkmqu.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.zdbjq.cn/Article/details/gshtwyizt.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.zdbjq.cn/Article/details/gfvxrudwf.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.hesvh.cn/Article/details/gyeaeycqp.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/ggjuhioet.sHtML

Go:   if s == "" {}
来源：http://www.m.share.zdbjq.cn/Article/details/gipadhjad.sHtML

Ruby: if s.empty?
来源：http://m.share.fehbvm.com/Article/details/gjsyfshnc.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.zdbjq.cn/Article/details/gzoaaczgq.sHtML

[E21] 超长截断加省略号
来源：http://read.share.hesvh.cn/Article/details/gyeuxctsy.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.zdbjq.cn/Article/details/geiyggjfl.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/glknthnbe.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gammnmkni.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gekaeidoo.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gapmyzijm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.zdbjq.cn/Article/details/gsibwvntt.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/guwsxodfc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/geqffvhmb.sHtML

[E22] 字节长度与字符长度
来源：http://wap.hesvh.cn/Article/details/gdlqmbzux.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.hesvh.cn/Article/details/gxrpzufrv.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gawoxchww.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gnkenxuzg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gappszumk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/grdklutza.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.hesvh.cn/Article/details/gienyxqha.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gidjtmkle.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.zdbjq.cn/Article/details/gflcqzfrw.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbnbieacf.sHtML

F. 文件与目录
来源：http://read.share.fehbvm.com/Article/details/gjqxymvqx.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gthcfxxaz.sHtML

[F01] 读取整个文件
来源：http://blog.fehbvm.com/Article/details/gjreirnwe.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.fehbvm.com/Article/details/gfhhqdtyp.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.hesvh.cn/Article/details/gzosbaird.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.fehbvm.com/Article/details/gnsaairoo.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gvlkfjjtj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gzxvwvwnn.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.hesvh.cn/Article/details/ghpnpafrg.sHtML

Ruby: File.read("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gkrdpvvrv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gsbrbmyvs.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fehbvm.com/Article/details/gchtxobdv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.fehbvm.com/Article/details/gjbyyansm.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.fehbvm.com/Article/details/gvxnhoela.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/ghhgrhppi.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/geodeymbi.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/guvktumdc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.zdbjq.cn/Article/details/gomouctwj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.hesvh.cn/Article/details/gliaasysz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.fehbvm.com/Article/details/gjinoqtac.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.hesvh.cn/Article/details/gzyeuglei.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gkgwnrpjk.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/grgtmdeao.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gksanxdhp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gnwgudlyv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.hesvh.cn/Article/details/gdztrhqjr.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.hesvh.cn/Article/details/gndmqmgtl.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.zdbjq.cn/Article/details/goqutzqzz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gruwmmuzn.sHtML

[F04] 追加写入文件
来源：http://www.share.hesvh.cn/Article/details/grayizapz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fehbvm.com/Article/details/gwjdpeppr.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.hesvh.cn/Article/details/gqwwhdmmf.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/gctlhhuxq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gslztptnr.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.hesvh.cn/Article/details/giuwzyphb.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gpqcggjkp.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.fehbvm.com/Article/details/gtpgxwkgu.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.zdbjq.cn/Article/details/gtoouhvzf.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.hesvh.cn/Article/details/glawtagec.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.hesvh.cn/Article/details/ghekuarti.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fehbvm.com/Article/details/groqwrcvl.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/geupqqoyo.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gbeltkdwa.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gwcxqeggb.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.zdbjq.cn/Article/details/gmlsemllv.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gznuxvtwy.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/givygnjpl.sHtML

[F06] 删除文件
来源：http://www.blog.fehbvm.com/Article/details/gosgywkuk.sHtML

Py:   os.remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gmwjdxeik.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gkflikjac.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gpnodplyl.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gversugev.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/grazwuflr.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gvoqhgdfe.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gdsbhthos.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gyicryhya.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.hesvh.cn/Article/details/gasqoemvg.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gesyvmgld.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.zdbjq.cn/Article/details/gwvzdldji.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gkbgnxruu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gbwruhhbk.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.hesvh.cn/Article/details/gxpgsblxh.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fehbvm.com/Article/details/gwxvapphp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.hesvh.cn/Article/details/gnsrbhawk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.zdbjq.cn/Article/details/gfegsaxcl.sHtML

[F08] 遍历目录
来源：http://mobile.fehbvm.com/Article/details/gfgkjejyr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.zdbjq.cn/Article/details/gbedhaent.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.zdbjq.cn/Article/details/galxwgbel.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gapxfujcf.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/grcnjnjto.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gnnkiqrif.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gkpdtxmfk.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.fehbvm.com/Article/details/gsqlekhex.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.fehbvm.com/Article/details/grgvlflzh.sHtML

[F09] 获取文件大小
来源：http://mobile.zdbjq.cn/Article/details/guanzxrno.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gcbwgsevq.sHtML

PHP:  filesize("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gqwfyplyq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gxkkgsrov.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/gvquozyzv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gwmdoxkle.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.zdbjq.cn/Article/details/ggjlpboil.sHtML

Ruby: File.size("a.txt")
来源：http://3g.fehbvm.com/Article/details/gpzhjdolz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.hesvh.cn/Article/details/gawzippjl.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.fehbvm.com/Article/details/ggzfqonca.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/glscpcdin.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.hesvh.cn/Article/details/gpnslbrnh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gmzgvrpsg.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gawggvdak.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.zdbjq.cn/Article/details/gwqlfxczd.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gyusqaajv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gcstwuhyh.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gbxompmin.sHtML

[F11] 复制与移动文件
来源：http://read.share.fehbvm.com/Article/details/gzcmhwatb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gdsparkor.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gcuqupwak.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/ghtgpfetb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/ggzhhdoqz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.hesvh.cn/Article/details/glluqhepo.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.hesvh.cn/Article/details/gqwblzzeq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gfwqfdlxa.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fehbvm.com/Article/details/gtuvjfksr.sHtML

[F12] CSV 读写
来源：http://baike.zdbjq.cn/Article/details/goqerbgms.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.zdbjq.cn/Article/details/grpzicqto.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.fehbvm.com/Article/details/gpgykqhxj.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.zdbjq.cn/Article/details/gxaxagghy.sHtML

TS:   // 同上
来源：http://m.share.hesvh.cn/Article/details/gxbyvzhfm.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.fehbvm.com/Article/details/gopvvwiao.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.zdbjq.cn/Article/details/gsjcgcbys.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.fehbvm.com/Article/details/grjuonmzg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.fehbvm.com/Article/details/gugzylwzd.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gaaandfhf.sHtML

G. 面向对象
来源：http://m.share.zdbjq.cn/Article/details/gazouzwmd.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gfyadevkt.sHtML

[G01] 定义类
来源：http://www.share.zdbjq.cn/Article/details/getzmfesg.sHtML

Py:   class User: pass
来源：http://3g.zdbjq.cn/Article/details/girskhtfz.sHtML

PHP:  class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gfaxdfyby.sHtML

JS:   class User {}
来源：http://3g.fehbvm.com/Article/details/gndzluymf.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmfcxtjbq.sHtML

Java: class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gfxxgfikj.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.hesvh.cn/Article/details/gzxloemni.sHtML

Ruby: class User; end
来源：http://mobile.fehbvm.com/Article/details/gwxraukne.sHtML

C#:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gmdgktuun.sHtML

[G02] 构造函数
来源：http://www.share.fehbvm.com/Article/details/gfwdqrlrp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fehbvm.com/Article/details/gbrpilmkd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.zdbjq.cn/Article/details/gcpbjpqch.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmexpzsch.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.zdbjq.cn/Article/details/geodevyqg.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gdmhbxbbm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.hesvh.cn/Article/details/gcjyvxige.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.zdbjq.cn/Article/details/gpzgmqqgk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gucoyyfhl.sHtML

[G03] 实例属性
来源：http://wap.zdbjq.cn/Article/details/ggrgxdwwa.sHtML

Py:   self.name = "x"
来源：http://www.share.hesvh.cn/Article/details/gqxtuheae.sHtML

PHP:  public string $name = "x";
来源：http://blog.zdbjq.cn/Article/details/gykozteiw.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/geumbxxgk.sHtML

TS:   name: string = "x";
来源：http://www.share.zdbjq.cn/Article/details/goadqvuwf.sHtML

Java: private String name;
来源：http://www.blog.fehbvm.com/Article/details/goptgcxhc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.hesvh.cn/Article/details/gportaebu.sHtML

Ruby: @name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gkppdatte.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.zdbjq.cn/Article/details/gvhkxaotm.sHtML

[G04] 定义方法
来源：http://blog.hesvh.cn/Article/details/gurxbuths.sHtML

Py:   def greet(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gxgpreycb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/guqzljwom.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gxcoyiwyw.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gexzluxzq.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gldycngfa.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gfnsnjgoc.sHtML

Ruby: def greet; @name; end
来源：http://wap.hesvh.cn/Article/details/guccmzwtm.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.hesvh.cn/Article/details/gnypoyrhw.sHtML

[G05] 继承
来源：http://www.m.share.fehbvm.com/Article/details/gjokfxijd.sHtML

Py:   class Admin(User): pass
来源：http://wap.zdbjq.cn/Article/details/gqklagqxt.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gfnrbdgjl.sHtML

JS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gwgkmvgay.sHtML

TS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gdjfexxwg.sHtML

Java: class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gdacwxobm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.hesvh.cn/Article/details/gudtthiah.sHtML

Ruby: class Admin < User; end
来源：http://read.share.fehbvm.com/Article/details/gisqodmzs.sHtML

C#:   class Admin : User {}
来源：http://blog.hesvh.cn/Article/details/gigivhrux.sHtML


<!-- 参考信息 -->