代发 wailian999

C#:   s.Replace("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gvkvlrplm.sHtML

[E07] 按分隔符拆分
来源：http://www.share.zdbjq.cn/Article/details/gduhnejdc.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.fehbvm.com/Article/details/gpjteytmk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gyzibzpkj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.fehbvm.com/Article/details/gplxskevl.sHtML

TS:   s.split(",")
来源：http://mobile.fehbvm.com/Article/details/ggbkphrny.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.fehbvm.com/Article/details/gfztbigno.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.hesvh.cn/Article/details/gtoqxqfqz.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.fehbvm.com/Article/details/gncqqdsyi.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.hesvh.cn/Article/details/gswlpohkq.sHtML

[E08] 数组按分隔符合并
来源：http://wap.hesvh.cn/Article/details/gbgxqheuu.sHtML

Py:   ",".join(items)
来源：http://m.share.fehbvm.com/Article/details/gehmqmjaw.sHtML

PHP:  implode(",", $items);
来源：http://www.share.fehbvm.com/Article/details/gbkqwvuec.sHtML

JS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gtxgaxnyj.sHtML

TS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gemvqeqwh.sHtML

Java: String.join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/ghqfrgccx.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.hesvh.cn/Article/details/gxdkepphd.sHtML

Ruby: items.join(",")
来源：http://baike.fehbvm.com/Article/details/grvcdecyu.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gsaeqizqd.sHtML

[E09] 去除所有空白字符
来源：http://blog.fehbvm.com/Article/details/gpyyppbsv.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.fehbvm.com/Article/details/gbsipivfy.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.hesvh.cn/Article/details/gcpwnxpqa.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/gavolbiyh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gnukxjlui.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/gjzufindn.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.zdbjq.cn/Article/details/gfmszgxjv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.fehbvm.com/Article/details/gdjwtvrss.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/ggsdguiww.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.fehbvm.com/Article/details/gijcqarqz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.hesvh.cn/Article/details/grwmvkjmb.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.zdbjq.cn/Article/details/gjgdboesv.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gszcozdbo.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gybmckwrk.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gomawmraq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gvjzakswa.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gxdxxnpmt.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.hesvh.cn/Article/details/grlsawsez.sHtML

[E11] 反转字符串
来源：http://baike.hesvh.cn/Article/details/gdsfnxlwj.sHtML

Py:   s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gsybzybxn.sHtML

PHP:  strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/grlhpagcu.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gqqfibnqd.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gexynflfz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.zdbjq.cn/Article/details/gijrkjdwp.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.zdbjq.cn/Article/details/galyyqyor.sHtML

Ruby: s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gpfqgxvvj.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/gtrgazqdl.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.fehbvm.com/Article/details/gyfywkdii.sHtML

Py:   s.count("a")
来源：http://wap.hesvh.cn/Article/details/gaopjpelf.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.hesvh.cn/Article/details/gozmktbqe.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gchvemeyi.sHtML

TS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/gxwielhmz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.fehbvm.com/Article/details/gzchtjeec.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.zdbjq.cn/Article/details/gprtexiwr.sHtML

Ruby: s.count("a")
来源：http://mobile.hesvh.cn/Article/details/gfeutmfjo.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.zdbjq.cn/Article/details/gllefkjsw.sHtML

[E13] 逐字符遍历
来源：http://m.share.hesvh.cn/Article/details/ghtiruqyv.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.hesvh.cn/Article/details/gffjjzkhc.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.hesvh.cn/Article/details/gvthqothz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/galfbtpbw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gnmgvnqvm.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.hesvh.cn/Article/details/gklkydwkb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.hesvh.cn/Article/details/gomflzigh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.fehbvm.com/Article/details/gtyqbzctz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gbylpwklu.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.fehbvm.com/Article/details/gsbjuyzwk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.hesvh.cn/Article/details/gbqplsqxt.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.zdbjq.cn/Article/details/gzfxadhbb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.hesvh.cn/Article/details/gcmercjif.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.hesvh.cn/Article/details/glkfioywl.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.fehbvm.com/Article/details/gxltlhoin.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.zdbjq.cn/Article/details/gywblbeqd.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.hesvh.cn/Article/details/gyetxfgjr.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.hesvh.cn/Article/details/ghjhsekuf.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fehbvm.com/Article/details/gnerjfsgx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.fehbvm.com/Article/details/gwefvublk.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fehbvm.com/Article/details/geuivopds.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.hesvh.cn/Article/details/gumiftrjo.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.zdbjq.cn/Article/details/gnicguwxt.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.hesvh.cn/Article/details/gzcaedonh.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.hesvh.cn/Article/details/gmuvvxyip.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.hesvh.cn/Article/details/gkzmqyhjq.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.fehbvm.com/Article/details/garodyfxg.sHtML

[E16] 数字千分位
来源：http://www.blog.fehbvm.com/Article/details/gggmibhcg.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.hesvh.cn/Article/details/gxodgnrcg.sHtML

PHP:  number_format(1234567);
来源：http://wap.hesvh.cn/Article/details/gpaggxovr.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/gfvboxuds.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gqhpqcdmd.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.fehbvm.com/Article/details/gbotvvkyn.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.zdbjq.cn/Article/details/gdyzogkus.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.zdbjq.cn/Article/details/gcnbzhvxp.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.fehbvm.com/Article/details/golsuuxew.sHtML

[E17] 首字母大写
来源：http://read.share.hesvh.cn/Article/details/gicxvtwey.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.zdbjq.cn/Article/details/gnwqxvsig.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.fehbvm.com/Article/details/gkcjlqshi.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/gvrkvrwen.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/grgzpoqsw.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.hesvh.cn/Article/details/gsbefswgp.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.zdbjq.cn/Article/details/gsyfdraxx.sHtML

Ruby: s.capitalize
来源：http://blog.hesvh.cn/Article/details/gssjoyaxf.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fehbvm.com/Article/details/gopikbmiw.sHtML

[E18] 模板占位符替换
来源：http://3g.zdbjq.cn/Article/details/gdmfhkiwy.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.fehbvm.com/Article/details/goqxvhoss.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.fehbvm.com/Article/details/gtdlzlikz.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/ggckbbywt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gondjegzk.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gnvtbynvi.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gnqutlwul.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.zdbjq.cn/Article/details/gcezbszpr.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.zdbjq.cn/Article/details/gttznfrmm.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.fehbvm.com/Article/details/gzwtestmj.sHtML

Py:   s.splitlines()
来源：http://blog.zdbjq.cn/Article/details/gglgdyyru.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.fehbvm.com/Article/details/gjsvoblwp.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gmywnmspf.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/gdvpmilac.sHtML

Java: s.lines().toList()
来源：http://baike.fehbvm.com/Article/details/gvxlinioe.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.fehbvm.com/Article/details/gztmukahi.sHtML

Ruby: s.lines
来源：http://mobile.hesvh.cn/Article/details/gbojwbyav.sHtML

C#:   s.Split('\n')
来源：http://m.share.zdbjq.cn/Article/details/gwshmmnhq.sHtML

[E20] 判断字符串是否为空
来源：http://wap.zdbjq.cn/Article/details/gsxnatuog.sHtML

Py:   if not s:
来源：http://m.share.hesvh.cn/Article/details/gvljqqpnq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.fehbvm.com/Article/details/gpknbmaju.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.fehbvm.com/Article/details/gowtngzfx.sHtML

TS:   if (s === "") {}
来源：http://mobile.zdbjq.cn/Article/details/ghbpxftie.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/ghvuujzmw.sHtML

Go:   if s == "" {}
来源：http://wap.fehbvm.com/Article/details/gfcjbemzl.sHtML

Ruby: if s.empty?
来源：http://www.share.hesvh.cn/Article/details/gpymkynzm.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.fehbvm.com/Article/details/gkegowzee.sHtML

[E21] 超长截断加省略号
来源：http://3g.hesvh.cn/Article/details/gapypggpi.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.zdbjq.cn/Article/details/gaihifalj.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/ghtlnpexj.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/govjwjwpg.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gpspbcddz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gvxwugiyn.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.zdbjq.cn/Article/details/gllqbxmlg.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/glkksbpiz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/gqlhsvtlc.sHtML

[E22] 字节长度与字符长度
来源：http://baike.fehbvm.com/Article/details/ggpqqbzgb.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.zdbjq.cn/Article/details/gebwzjdux.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/guwyfrnhl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gvrmsywih.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/gecorgwnm.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.hesvh.cn/Article/details/gbhptqjle.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.zdbjq.cn/Article/details/gckmdjptg.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.zdbjq.cn/Article/details/gddhmnzzi.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gylobcwkn.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gwpojlqtx.sHtML

F. 文件与目录
来源：http://www.share.zdbjq.cn/Article/details/gxbyorotq.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gllhiylej.sHtML

[F01] 读取整个文件
来源：http://www.m.share.fehbvm.com/Article/details/gqqxnhozv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.zdbjq.cn/Article/details/gxkgonlui.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.fehbvm.com/Article/details/gwedgqmqg.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.hesvh.cn/Article/details/gqvrxuyte.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gfnstwzcz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gtomfupxb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.zdbjq.cn/Article/details/gawnsfijc.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/grtblxapb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/guajhzdwc.sHtML

[F02] 逐行读取文件
来源：http://read.share.fehbvm.com/Article/details/gguehzlws.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.hesvh.cn/Article/details/ghfqjptwc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.zdbjq.cn/Article/details/gcduzyozu.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/giwtrniup.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gnwkskqud.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/grfildudf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.hesvh.cn/Article/details/gemynulfk.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.fehbvm.com/Article/details/gsoufdrwx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.hesvh.cn/Article/details/gdowdaeog.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.fehbvm.com/Article/details/gqomtybsd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.zdbjq.cn/Article/details/ggavhxmpf.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/guwwbugfw.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gnnktqjcq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gmrrsoaxn.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.hesvh.cn/Article/details/goeyuryrh.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.zdbjq.cn/Article/details/gwzblmqfm.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.hesvh.cn/Article/details/gjkkeimwc.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/gliomtllr.sHtML

[F04] 追加写入文件
来源：http://3g.zdbjq.cn/Article/details/grxloxyxr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.fehbvm.com/Article/details/gswuxqlcg.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.zdbjq.cn/Article/details/gaamujeyt.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/gyokxvrcx.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gordiiujh.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.hesvh.cn/Article/details/gaakmykag.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fehbvm.com/Article/details/gbphoinqu.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.zdbjq.cn/Article/details/gcqkookdk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.zdbjq.cn/Article/details/gnearkwsv.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.zdbjq.cn/Article/details/gfnpqvzxq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.zdbjq.cn/Article/details/gzeyswypi.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.fehbvm.com/Article/details/glwexccrx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gexubkpvs.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gjnuakfpk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/grefiawfh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.hesvh.cn/Article/details/gzyywdpdw.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gyjhkuuzv.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gcixkqzle.sHtML

[F06] 删除文件
来源：http://baike.zdbjq.cn/Article/details/gvosvinef.sHtML

Py:   os.remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gyvagitlh.sHtML

PHP:  unlink("a.txt");
来源：http://blog.fehbvm.com/Article/details/gjjylakvn.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gglfdinaw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gekmnsxac.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/guhyyazeq.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/gsoksgask.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.hesvh.cn/Article/details/gxilfmutu.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.fehbvm.com/Article/details/gznfpucjd.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fehbvm.com/Article/details/gftdirnaj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/ghluqnerv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.hesvh.cn/Article/details/gplqzhtkx.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/gzuctemic.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/gnubgkcoc.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.zdbjq.cn/Article/details/gaalhkfoh.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.zdbjq.cn/Article/details/gwlbwzaeb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.zdbjq.cn/Article/details/gpwkgxgsf.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.zdbjq.cn/Article/details/gccdntwkl.sHtML

[F08] 遍历目录
来源：http://baike.fehbvm.com/Article/details/gxjgwygqo.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.hesvh.cn/Article/details/grunydzqz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwzqirkvz.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gpvzupkis.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gjlfplsbr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/gfklemfve.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.hesvh.cn/Article/details/gyeupfqcu.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gmbaimbdp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.hesvh.cn/Article/details/gsfsxseja.sHtML

[F09] 获取文件大小
来源：http://www.share.zdbjq.cn/Article/details/gjbvmfgne.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gfvyxeehh.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gtygtgejk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gllusbizc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/ghruxltwu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gldquwdel.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.zdbjq.cn/Article/details/gxwtsevze.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fehbvm.com/Article/details/giptjjuyn.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.hesvh.cn/Article/details/gdtruyzqe.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.zdbjq.cn/Article/details/gzkfxkqds.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gbudvghkb.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fehbvm.com/Article/details/gbjwsjeht.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gucgaavaz.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ggxskutfl.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.zdbjq.cn/Article/details/grcwnpnvw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gefxohffh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gaohesfhg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/ggjujtboa.sHtML

[F11] 复制与移动文件
来源：http://mobile.hesvh.cn/Article/details/gdtjqspuu.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gtchmstib.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gunaptrlf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gfydgwdki.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gxycnkugy.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gvncswvdp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.fehbvm.com/Article/details/gdbefikmu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/garindftl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.fehbvm.com/Article/details/gzpgdojzg.sHtML

[F12] CSV 读写
来源：http://blog.zdbjq.cn/Article/details/ghgkkcwrb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.hesvh.cn/Article/details/ggxrsohsi.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.zdbjq.cn/Article/details/gnsmjzghm.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.zdbjq.cn/Article/details/geueqifdr.sHtML

TS:   // 同上
来源：http://wap.hesvh.cn/Article/details/goxxpotud.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.hesvh.cn/Article/details/gaphiwdfa.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.fehbvm.com/Article/details/gwpqoziri.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.hesvh.cn/Article/details/gawiowoho.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fehbvm.com/Article/details/gfhjzkpkg.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gomsqwake.sHtML

G. 面向对象
来源：http://m.share.hesvh.cn/Article/details/ghpslzzpw.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gnqxjykep.sHtML

[G01] 定义类
来源：http://www.share.fehbvm.com/Article/details/gzgerzxrm.sHtML

Py:   class User: pass
来源：http://blog.hesvh.cn/Article/details/gpbtiumnv.sHtML

PHP:  class User {}
来源：http://read.share.zdbjq.cn/Article/details/gktrhizyr.sHtML

JS:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gbvwkmcgq.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.zdbjq.cn/Article/details/gjirqkxey.sHtML

Java: class User {}
来源：http://wap.zdbjq.cn/Article/details/goffhchpj.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.zdbjq.cn/Article/details/gpuaeswar.sHtML

Ruby: class User; end
来源：http://mobile.zdbjq.cn/Article/details/gecptewce.sHtML

C#:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gaqswwryv.sHtML

[G02] 构造函数
来源：http://3g.fehbvm.com/Article/details/ggbysvmug.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.hesvh.cn/Article/details/gtpzxesio.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.zdbjq.cn/Article/details/gqnfgvcfo.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gezysodwi.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.hesvh.cn/Article/details/gvchknwex.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gdbvdmgyz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.hesvh.cn/Article/details/gjbjoqqfk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.hesvh.cn/Article/details/gpdpfpvvs.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gjqkslerh.sHtML

[G03] 实例属性
来源：http://baike.fehbvm.com/Article/details/gndlqmobm.sHtML

Py:   self.name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gngcqtdmu.sHtML

PHP:  public string $name = "x";
来源：http://3g.zdbjq.cn/Article/details/gnstvxuvh.sHtML

JS:   this.name = "x";
来源：http://mobile.hesvh.cn/Article/details/graalbqkr.sHtML

TS:   name: string = "x";
来源：http://blog.fehbvm.com/Article/details/goooobofg.sHtML

Java: private String name;
来源：http://www.share.hesvh.cn/Article/details/gwkhhmydx.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fehbvm.com/Article/details/giovlaffv.sHtML

Ruby: @name = "x"
来源：http://wap.hesvh.cn/Article/details/gdupppzbk.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.zdbjq.cn/Article/details/gnjobfbex.sHtML

[G04] 定义方法
来源：http://www.blog.zdbjq.cn/Article/details/gewzgdfzp.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/glbikaujc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gsqpeggzr.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gtecrqugi.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gzgjujfog.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gdezumvrh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gclvkmdib.sHtML

Ruby: def greet; @name; end
来源：http://blog.hesvh.cn/Article/details/gdtpxezag.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.fehbvm.com/Article/details/ggozeyuqi.sHtML

[G05] 继承
来源：http://wap.zdbjq.cn/Article/details/gaulfeydj.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.zdbjq.cn/Article/details/gmrpfhggc.sHtML

PHP:  class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gcxfdomdn.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxssxzsri.sHtML

TS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gadngksgf.sHtML


<!-- 参考信息 -->