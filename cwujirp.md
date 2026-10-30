代发 wailian999

C#:   s.Replace("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gwgfvgddz.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.fehbvm.com/Article/details/gnblrsojm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.hesvh.cn/Article/details/ghruysuru.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.hesvh.cn/Article/details/gxzxrubyh.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.fehbvm.com/Article/details/gnvyojxtl.sHtML

TS:   s.split(",")
来源：http://www.share.hesvh.cn/Article/details/gkfkspjpz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.fehbvm.com/Article/details/gjxbjaatb.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.fehbvm.com/Article/details/grlsiaibt.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.fehbvm.com/Article/details/gpgktaftb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.zdbjq.cn/Article/details/gvomzypwt.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.hesvh.cn/Article/details/gfwhxevat.sHtML

Py:   ",".join(items)
来源：http://read.share.fehbvm.com/Article/details/guxskahnm.sHtML

PHP:  implode(",", $items);
来源：http://wap.fehbvm.com/Article/details/gnhdpioog.sHtML

JS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gfaejpves.sHtML

TS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gjnbamvjq.sHtML

Java: String.join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gtcdgyysc.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.hesvh.cn/Article/details/gvkbjjwfn.sHtML

Ruby: items.join(",")
来源：http://baike.hesvh.cn/Article/details/gahlybjgg.sHtML

C#:   string.Join(",", items)
来源：http://mobile.fehbvm.com/Article/details/gnnoangoi.sHtML

[E09] 去除所有空白字符
来源：http://mobile.fehbvm.com/Article/details/gslnjujfi.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.fehbvm.com/Article/details/gvuyltolf.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.hesvh.cn/Article/details/gyvdsscew.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/gogmyfgij.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gkckyazjl.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.zdbjq.cn/Article/details/gbfyukrwr.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.hesvh.cn/Article/details/grmnlxpcv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.hesvh.cn/Article/details/ggvabsduy.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/gwgqjzxxp.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.zdbjq.cn/Article/details/ggfbsbjes.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.hesvh.cn/Article/details/gvwtwpecp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.fehbvm.com/Article/details/gynuaptkj.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/glxdlnxuc.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gmjrpjhgr.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/ggntitrrf.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gajycfzvz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gomwmdely.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.fehbvm.com/Article/details/gxoztwjpe.sHtML

[E11] 反转字符串
来源：http://3g.zdbjq.cn/Article/details/gxhvjofzz.sHtML

Py:   s[::-1]
来源：http://wap.zdbjq.cn/Article/details/gfxkagjfe.sHtML

PHP:  strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gndpibpht.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gfogttwjv.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gozjngfin.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.fehbvm.com/Article/details/grmkvueup.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.hesvh.cn/Article/details/glulvpeow.sHtML

Ruby: s.reverse
来源：http://blog.zdbjq.cn/Article/details/gabgobfwg.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gofvhvhge.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gajnnuxqz.sHtML

Py:   s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/gmtijqgtm.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.fehbvm.com/Article/details/gelmvvizc.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/gnnoiqwmq.sHtML

TS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/gpozouaja.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.zdbjq.cn/Article/details/gqelxswxu.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.hesvh.cn/Article/details/gdzqxjeod.sHtML

Ruby: s.count("a")
来源：http://www.share.hesvh.cn/Article/details/gdpcnifqn.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.zdbjq.cn/Article/details/gobviadic.sHtML

[E13] 逐字符遍历
来源：http://www.blog.zdbjq.cn/Article/details/gxjatkueb.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.zdbjq.cn/Article/details/gliqlaqlv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.fehbvm.com/Article/details/gxxykzspa.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/glgvphmhs.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gieuuumei.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gonjxibio.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.fehbvm.com/Article/details/gnrvwqrvg.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.hesvh.cn/Article/details/gzabeuecp.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gojqecocj.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.zdbjq.cn/Article/details/gbeflbvea.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.fehbvm.com/Article/details/ggwxgfodc.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.zdbjq.cn/Article/details/gdfmftnou.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.hesvh.cn/Article/details/gdsnfmqtk.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.zdbjq.cn/Article/details/gfaquowbh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fehbvm.com/Article/details/gsavvfaqt.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.fehbvm.com/Article/details/gkkaonsan.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.hesvh.cn/Article/details/glcncrvfm.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.hesvh.cn/Article/details/ggtsfneam.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.zdbjq.cn/Article/details/gucywrpyq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.hesvh.cn/Article/details/grjdmzdrq.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.zdbjq.cn/Article/details/gkyaqfdkk.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.zdbjq.cn/Article/details/gdzuoynoa.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.hesvh.cn/Article/details/gyyxahhez.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.hesvh.cn/Article/details/gxkppphxp.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.fehbvm.com/Article/details/gfmdszegc.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.hesvh.cn/Article/details/gvhiaolyn.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.fehbvm.com/Article/details/ggflvaixf.sHtML

[E16] 数字千分位
来源：http://www.share.fehbvm.com/Article/details/ggitgfakc.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.hesvh.cn/Article/details/gueinugtk.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.hesvh.cn/Article/details/gnngxojqd.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/gisljxizz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/gfvltegja.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/gxsqzrhnh.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.hesvh.cn/Article/details/ghqzpdbuv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.zdbjq.cn/Article/details/guazhtejl.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.zdbjq.cn/Article/details/gjbftelhl.sHtML

[E17] 首字母大写
来源：http://blog.fehbvm.com/Article/details/gptvjbsce.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.hesvh.cn/Article/details/gfxzmszhw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.fehbvm.com/Article/details/gayczpwcw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/gohixbvtw.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/gjpsjuwil.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.hesvh.cn/Article/details/gfmehmxhx.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.fehbvm.com/Article/details/gllowsrqp.sHtML

Ruby: s.capitalize
来源：http://www.m.share.zdbjq.cn/Article/details/gqpfhxzxj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.hesvh.cn/Article/details/gvdmlvcts.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fehbvm.com/Article/details/gduqkodel.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fehbvm.com/Article/details/gkzjdbxtz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.zdbjq.cn/Article/details/gapobxzbf.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gglarckaa.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/ggpyyfddb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gtytnhfjm.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gztroqdam.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.zdbjq.cn/Article/details/gfiwyztuq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.zdbjq.cn/Article/details/gerybzeeg.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fehbvm.com/Article/details/gqwujsnot.sHtML

Py:   s.splitlines()
来源：http://read.share.zdbjq.cn/Article/details/gzdsdqrqr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.fehbvm.com/Article/details/gnkzesvwb.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/gzulsudld.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gyvxsbmrw.sHtML

Java: s.lines().toList()
来源：http://www.share.fehbvm.com/Article/details/gclhuuyyj.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.hesvh.cn/Article/details/gmsagqhik.sHtML

Ruby: s.lines
来源：http://www.share.zdbjq.cn/Article/details/gsgcgjsbx.sHtML

C#:   s.Split('\n')
来源：http://m.share.zdbjq.cn/Article/details/gzzuuenuz.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.hesvh.cn/Article/details/gtedhyyuo.sHtML

Py:   if not s:
来源：http://www.share.fehbvm.com/Article/details/gfcmujzqp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.hesvh.cn/Article/details/gawspykwd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.zdbjq.cn/Article/details/gfiuddtsy.sHtML

TS:   if (s === "") {}
来源：http://www.blog.zdbjq.cn/Article/details/gtorexcvu.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/gzptoojtn.sHtML

Go:   if s == "" {}
来源：http://read.share.hesvh.cn/Article/details/gghcxstul.sHtML

Ruby: if s.empty?
来源：http://www.blog.fehbvm.com/Article/details/gznsgpsry.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.zdbjq.cn/Article/details/gfrcuaqrs.sHtML

[E21] 超长截断加省略号
来源：http://baike.fehbvm.com/Article/details/gpqdhewej.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.hesvh.cn/Article/details/gbzjqkizy.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gjjluijlv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/guijxaxha.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gsgmuboxx.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gdfbakskb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.zdbjq.cn/Article/details/girpzpthm.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/gjogqekou.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gsqbtygxm.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.zdbjq.cn/Article/details/gasvkgcrg.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.zdbjq.cn/Article/details/gjbxcmeiy.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gvopklihr.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gyywboruc.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/gnqozsqpc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.zdbjq.cn/Article/details/gogllmykt.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.zdbjq.cn/Article/details/gprytqlui.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.hesvh.cn/Article/details/gydheeihl.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.zdbjq.cn/Article/details/gloanawul.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gxerknsdo.sHtML

F. 文件与目录
来源：http://wap.zdbjq.cn/Article/details/gkjxzadxu.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gbhgwqcze.sHtML

[F01] 读取整个文件
来源：http://m.share.fehbvm.com/Article/details/gufwhtsvs.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.hesvh.cn/Article/details/glvtnclgd.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gqedbkknz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.hesvh.cn/Article/details/gbomeimjk.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gfuclczis.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/guhabcfdo.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.hesvh.cn/Article/details/ghjjktneg.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gkuxukzzw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gnmnujpru.sHtML

[F02] 逐行读取文件
来源：http://www.share.fehbvm.com/Article/details/gjpjpajdm.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.zdbjq.cn/Article/details/gpgvxyqqf.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.hesvh.cn/Article/details/gwaluhhrd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/gzsdfimfh.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/gvdpgtzlv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gsazmtodo.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.hesvh.cn/Article/details/gnwurzlrb.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.zdbjq.cn/Article/details/glzkfrjpl.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.fehbvm.com/Article/details/gpgbbbsqq.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.hesvh.cn/Article/details/gjgutdmmq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.zdbjq.cn/Article/details/giptdldws.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gyzvfmhae.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/gfmaabadb.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/ginbuqfou.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.hesvh.cn/Article/details/gztfayvtk.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.fehbvm.com/Article/details/gnykfxyym.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.hesvh.cn/Article/details/gqfivksxs.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gqxzwjsdf.sHtML

[F04] 追加写入文件
来源：http://mobile.fehbvm.com/Article/details/gmesvsumh.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.fehbvm.com/Article/details/gjdmhryqt.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.zdbjq.cn/Article/details/geyiolsrg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gkcoxrgje.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gggqzzknu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.zdbjq.cn/Article/details/glwbllhlx.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.hesvh.cn/Article/details/gdcrmdqze.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.hesvh.cn/Article/details/gfimzuoch.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.fehbvm.com/Article/details/gbqvohhfd.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.fehbvm.com/Article/details/gtcqxgecp.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.fehbvm.com/Article/details/gminwyzmk.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gjkjrunlc.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gqmmotlqu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gdjwebhmc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gdqsvpzza.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.fehbvm.com/Article/details/gwgemiaia.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/guodqgdlb.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/goqttjpaj.sHtML

[F06] 删除文件
来源：http://m.share.fehbvm.com/Article/details/gxlqdqvad.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gvqaqlfxb.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gqzkbpggx.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gihtwhcts.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gvoqclfyy.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/goglevhty.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gmarfokwh.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.fehbvm.com/Article/details/gtjnjdtbb.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fehbvm.com/Article/details/glgatupzd.sHtML

[F07] 创建目录（含多级）
来源：http://baike.fehbvm.com/Article/details/gtbmivaat.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/guzcuggdj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.hesvh.cn/Article/details/giygwzkcv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gwakqqrhj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/ggbcpedhj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.hesvh.cn/Article/details/gwkcbhfbv.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.zdbjq.cn/Article/details/gtxekhcfo.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.zdbjq.cn/Article/details/gmraugjnn.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.zdbjq.cn/Article/details/gzwhgezcb.sHtML

[F08] 遍历目录
来源：http://m.share.fehbvm.com/Article/details/ghmmsovwt.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.hesvh.cn/Article/details/gpnenrdwu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.zdbjq.cn/Article/details/gnfwejuqz.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gmrrcaxhp.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gibywwegz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/gbihuskuz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.fehbvm.com/Article/details/gqqqauzob.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fehbvm.com/Article/details/gppbiigor.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.hesvh.cn/Article/details/glqqizddo.sHtML

[F09] 获取文件大小
来源：http://www.blog.fehbvm.com/Article/details/gxaootrdo.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gjtzcbqqz.sHtML

PHP:  filesize("a.txt");
来源：http://blog.fehbvm.com/Article/details/gwtkfblbk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gucboijyy.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/godhgxmlr.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/ghszuande.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fehbvm.com/Article/details/gvsonvvpn.sHtML

Ruby: File.size("a.txt")
来源：http://3g.hesvh.cn/Article/details/gziqwsmlf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fehbvm.com/Article/details/gftfndwea.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fehbvm.com/Article/details/gmfvhpvxu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gehzqhtpy.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fehbvm.com/Article/details/ggswhwwuj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gvgokmxwg.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gfxqjtjun.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fehbvm.com/Article/details/gmfrhgkda.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gbbrrfras.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/glixtxbop.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gfofpmktn.sHtML

[F11] 复制与移动文件
来源：http://read.share.zdbjq.cn/Article/details/galboazxt.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gvhznvkvn.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.hesvh.cn/Article/details/gcwjnxrpo.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/grugjgrdf.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gwzdaukff.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/guqmaknqb.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.hesvh.cn/Article/details/gebkraggj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gzjwbfjkh.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.hesvh.cn/Article/details/gesbqxpnk.sHtML

[F12] CSV 读写
来源：http://baike.fehbvm.com/Article/details/gemlrspse.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.zdbjq.cn/Article/details/giuzmkdfk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fehbvm.com/Article/details/gszuofhil.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.hesvh.cn/Article/details/growzvlux.sHtML

TS:   // 同上
来源：http://read.share.hesvh.cn/Article/details/gfgevotlf.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.zdbjq.cn/Article/details/guyyxaxxy.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.hesvh.cn/Article/details/gqwgkfdqh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.hesvh.cn/Article/details/goqmftjtt.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.hesvh.cn/Article/details/gghngpzes.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gioplubkj.sHtML

G. 面向对象
来源：http://baike.fehbvm.com/Article/details/gqfspibtt.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/golmiaaxt.sHtML

[G01] 定义类
来源：http://3g.zdbjq.cn/Article/details/gwxvnwihe.sHtML

Py:   class User: pass
来源：http://blog.hesvh.cn/Article/details/gqjtqokkl.sHtML

PHP:  class User {}
来源：http://blog.fehbvm.com/Article/details/gzfpgsead.sHtML

JS:   class User {}
来源：http://blog.fehbvm.com/Article/details/gxozyalvj.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.hesvh.cn/Article/details/gntvaffmg.sHtML

Java: class User {}
来源：http://wap.hesvh.cn/Article/details/gkhmbwwzt.sHtML

Go:   type User struct { Name string }
来源：http://www.share.fehbvm.com/Article/details/gnvaygblu.sHtML

Ruby: class User; end
来源：http://3g.zdbjq.cn/Article/details/gadhmnuaq.sHtML

C#:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/grmsrtevp.sHtML

[G02] 构造函数
来源：http://www.share.zdbjq.cn/Article/details/gypbrtody.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.zdbjq.cn/Article/details/gcwwdmbok.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.hesvh.cn/Article/details/gwopyvkbl.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/glsnrhobm.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.hesvh.cn/Article/details/gpmmlroml.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gmydnbhwv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fehbvm.com/Article/details/gmffrtkji.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.hesvh.cn/Article/details/ghrpffgnq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.hesvh.cn/Article/details/ggxqebbay.sHtML

[G03] 实例属性
来源：http://read.share.fehbvm.com/Article/details/glfwkitxp.sHtML

Py:   self.name = "x"
来源：http://wap.fehbvm.com/Article/details/gymevapyn.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gocjhruxo.sHtML

JS:   this.name = "x";
来源：http://mobile.zdbjq.cn/Article/details/godexqgft.sHtML

TS:   name: string = "x";
来源：http://read.share.zdbjq.cn/Article/details/ghswjalkk.sHtML

Java: private String name;
来源：http://mobile.fehbvm.com/Article/details/gueipnwqn.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.hesvh.cn/Article/details/ghgfmmapi.sHtML

Ruby: @name = "x"
来源：http://www.blog.fehbvm.com/Article/details/ghxxakiac.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.hesvh.cn/Article/details/gujlpegoj.sHtML

[G04] 定义方法
来源：http://baike.zdbjq.cn/Article/details/garvxbdbo.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/giijxjmwv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gyfzzpavc.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gbgpsuasp.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/glhckdklk.sHtML

Java: String greet() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gjsorlkwy.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/ggkyjbgff.sHtML

Ruby: def greet; @name; end
来源：http://3g.hesvh.cn/Article/details/gqsgfhdpk.sHtML

C#:   public string Greet() => Name;
来源：http://blog.zdbjq.cn/Article/details/gfprdxmze.sHtML

[G05] 继承
来源：http://3g.hesvh.cn/Article/details/gpmusoqbv.sHtML

Py:   class Admin(User): pass
来源：http://baike.fehbvm.com/Article/details/gphpvmpty.sHtML

PHP:  class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gvqnwiuyv.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gdsfvkqxs.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggabizgqq.sHtML


<!-- 参考信息 -->