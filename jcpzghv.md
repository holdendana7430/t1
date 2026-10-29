代发 wailian999

C#:   s.Replace("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gjqqrzuxn.sHtML

[E07] 按分隔符拆分
来源：http://baike.hesvh.cn/Article/details/gfxyneziw.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.fehbvm.com/Article/details/gluyxjsao.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.zdbjq.cn/Article/details/gszrkxkqx.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.hesvh.cn/Article/details/glbhhpczt.sHtML

TS:   s.split(",")
来源：http://blog.fehbvm.com/Article/details/ghohojbeh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.zdbjq.cn/Article/details/goxmxmxvz.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.zdbjq.cn/Article/details/goaxicmgc.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.zdbjq.cn/Article/details/gdvcsoiqb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.hesvh.cn/Article/details/gzxskffiq.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.fehbvm.com/Article/details/gqugklgki.sHtML

Py:   ",".join(items)
来源：http://3g.hesvh.cn/Article/details/glwbvfuan.sHtML

PHP:  implode(",", $items);
来源：http://wap.zdbjq.cn/Article/details/gxbucrpaf.sHtML

JS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/gijpeahpd.sHtML

TS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gflkpbtti.sHtML

Java: String.join(",", items)
来源：http://3g.hesvh.cn/Article/details/gspugeluc.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.hesvh.cn/Article/details/gtzuaygqv.sHtML

Ruby: items.join(",")
来源：http://read.share.fehbvm.com/Article/details/guwjqyclh.sHtML

C#:   string.Join(",", items)
来源：http://blog.fehbvm.com/Article/details/gnvxqnkhx.sHtML

[E09] 去除所有空白字符
来源：http://wap.zdbjq.cn/Article/details/gdbdbemnv.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.hesvh.cn/Article/details/gdbumgufy.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.hesvh.cn/Article/details/gghcrblvo.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/gmyvxzwex.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/gufhgvowx.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.fehbvm.com/Article/details/grorqaspj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.fehbvm.com/Article/details/gslutarcs.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.hesvh.cn/Article/details/ghontrcne.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.fehbvm.com/Article/details/gzbtnptug.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.fehbvm.com/Article/details/gbqxttbzw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gskgdhwzo.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.hesvh.cn/Article/details/giexwlygz.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/givtmtoom.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gfkekvwba.sHtML

Java: String.format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gsttpctej.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/glgfokmjw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gxdztzerx.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.fehbvm.com/Article/details/gwrfzqcww.sHtML

[E11] 反转字符串
来源：http://m.share.fehbvm.com/Article/details/gfgkwjxfk.sHtML

Py:   s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/gsjpkiqhv.sHtML

PHP:  strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gaxdrhgbv.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gmnrntywf.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gprlvwedi.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fehbvm.com/Article/details/gfwnjkioj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.fehbvm.com/Article/details/gqtqalnrw.sHtML

Ruby: s.reverse
来源：http://3g.hesvh.cn/Article/details/glyqgenzn.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gjheolpvg.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.fehbvm.com/Article/details/gaiinevif.sHtML

Py:   s.count("a")
来源：http://baike.fehbvm.com/Article/details/grbgcwjcw.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.hesvh.cn/Article/details/gdnmodvus.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/grlnbhadz.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/grgugbdow.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.zdbjq.cn/Article/details/glazklfkc.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.fehbvm.com/Article/details/gzllbojdm.sHtML

Ruby: s.count("a")
来源：http://blog.hesvh.cn/Article/details/ghkzpbewv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.hesvh.cn/Article/details/gekrdcxqd.sHtML

[E13] 逐字符遍历
来源：http://wap.fehbvm.com/Article/details/gsgefqrtj.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.zdbjq.cn/Article/details/gxnmuvach.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.fehbvm.com/Article/details/gaskxmfoy.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gummecsqf.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gifzypadu.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.hesvh.cn/Article/details/ghpyjzeqi.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.fehbvm.com/Article/details/gmzvafheg.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.hesvh.cn/Article/details/gdxgufkxx.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.hesvh.cn/Article/details/gwcavljuf.sHtML

[E14] URL 编码与 Base64
来源：http://blog.fehbvm.com/Article/details/gboatuvja.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.zdbjq.cn/Article/details/gobvkvxry.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.hesvh.cn/Article/details/gjsutmugw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.zdbjq.cn/Article/details/gssmoerxb.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.fehbvm.com/Article/details/gvavkbqzm.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gpwmizlhm.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.hesvh.cn/Article/details/goofgqkua.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.zdbjq.cn/Article/details/giwdyfnvf.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.hesvh.cn/Article/details/gfkrhiorq.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.hesvh.cn/Article/details/grqaqxpfx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.hesvh.cn/Article/details/ggmsupzxx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.hesvh.cn/Article/details/geowfsxzl.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.fehbvm.com/Article/details/gqggvqwoa.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gzmucpkna.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.hesvh.cn/Article/details/gvinioyfy.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.zdbjq.cn/Article/details/gtioubrub.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.fehbvm.com/Article/details/guhohtsod.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.fehbvm.com/Article/details/grtfwljjp.sHtML

[E16] 数字千分位
来源：http://blog.hesvh.cn/Article/details/gshsltavs.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.hesvh.cn/Article/details/ghxcchbtz.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.zdbjq.cn/Article/details/grwjehsux.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/gzydumild.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gfjnpevdg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gywkshvzu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.zdbjq.cn/Article/details/gmzcrvurh.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.fehbvm.com/Article/details/gubmilupr.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.hesvh.cn/Article/details/gqdfjzvjs.sHtML

[E17] 首字母大写
来源：http://baike.fehbvm.com/Article/details/gmaltipbu.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.zdbjq.cn/Article/details/gzkdkrosh.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.fehbvm.com/Article/details/gjhywefqm.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.hesvh.cn/Article/details/gbswhsfvr.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/gehaevquv.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.fehbvm.com/Article/details/gacvwqzva.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.fehbvm.com/Article/details/gegswtiqb.sHtML

Ruby: s.capitalize
来源：http://www.blog.fehbvm.com/Article/details/gwmgjtfid.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.hesvh.cn/Article/details/gqtsfgztp.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.hesvh.cn/Article/details/gqiosbfbn.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.zdbjq.cn/Article/details/gnhwqczus.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.zdbjq.cn/Article/details/gqlcenibq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gqqnfdfbs.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/geohlqqdk.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gwurytung.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gypgchrjp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.hesvh.cn/Article/details/gfzejhenk.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.fehbvm.com/Article/details/gkhdynnij.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.hesvh.cn/Article/details/gtduwxvny.sHtML

Py:   s.splitlines()
来源：http://blog.zdbjq.cn/Article/details/gyapnjjbb.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.fehbvm.com/Article/details/geffwisbl.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/glmnkzoer.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/geeuglukd.sHtML

Java: s.lines().toList()
来源：http://3g.zdbjq.cn/Article/details/gxvqgshud.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.fehbvm.com/Article/details/gbafsjnnk.sHtML

Ruby: s.lines
来源：http://wap.fehbvm.com/Article/details/gczvyituj.sHtML

C#:   s.Split('\n')
来源：http://m.share.fehbvm.com/Article/details/gijwbwerv.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.zdbjq.cn/Article/details/gtilqydoe.sHtML

Py:   if not s:
来源：http://mobile.hesvh.cn/Article/details/ggewwxcrk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.fehbvm.com/Article/details/gumipnsqh.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.zdbjq.cn/Article/details/geqxggmir.sHtML

TS:   if (s === "") {}
来源：http://3g.zdbjq.cn/Article/details/gfkufrcwi.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gklsgchuk.sHtML

Go:   if s == "" {}
来源：http://www.share.fehbvm.com/Article/details/gjiygdndq.sHtML

Ruby: if s.empty?
来源：http://blog.zdbjq.cn/Article/details/gsxcprdgk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.hesvh.cn/Article/details/gusavmpyw.sHtML

[E21] 超长截断加省略号
来源：http://3g.fehbvm.com/Article/details/gqccmbpjj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.zdbjq.cn/Article/details/guqircdtf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gjyuzwapj.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gvfojucue.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gdiedufxw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gkuylatbp.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.zdbjq.cn/Article/details/glntnebmq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gegrgkaez.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gerlmqkla.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fehbvm.com/Article/details/gnfvtxljn.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.zdbjq.cn/Article/details/gdxppljzk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gjwnajjeg.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gnqlsfzet.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gzoeqpbvg.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.fehbvm.com/Article/details/grxgfqxuv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.fehbvm.com/Article/details/gfhrmepfv.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gwisuwpuq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.fehbvm.com/Article/details/giixccame.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gsaunmfkg.sHtML

F. 文件与目录
来源：http://read.share.zdbjq.cn/Article/details/gwfmqsrrg.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gnzifikbg.sHtML

[F01] 读取整个文件
来源：http://www.m.share.fehbvm.com/Article/details/ghtummenm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.hesvh.cn/Article/details/gtalqhhxx.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gqhkqrhdk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.fehbvm.com/Article/details/gswhvpgbb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gkhkpevcs.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gnxqrenjh.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.zdbjq.cn/Article/details/gazieeyxw.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/ggwsuodei.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gmpnyjzet.sHtML

[F02] 逐行读取文件
来源：http://wap.zdbjq.cn/Article/details/ghifypqoe.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.fehbvm.com/Article/details/gzrnkdfqt.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.zdbjq.cn/Article/details/gyjovfnvs.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/gaxkyibyo.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gvquocgmg.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gnkzswerd.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.fehbvm.com/Article/details/goaxdejcn.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.hesvh.cn/Article/details/gklblztxc.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.zdbjq.cn/Article/details/ggiixsttp.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.zdbjq.cn/Article/details/gajtwqeyz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.fehbvm.com/Article/details/gjpsiowbc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.fehbvm.com/Article/details/ghdfwyqpb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gzjrxfego.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gwtusjuka.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gdjrcgrbi.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.hesvh.cn/Article/details/ghqpuscms.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gilfcmpex.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gloapupwn.sHtML

[F04] 追加写入文件
来源：http://m.share.fehbvm.com/Article/details/gelnfnxrr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fehbvm.com/Article/details/grhlghbkf.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.hesvh.cn/Article/details/gevuagfgd.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gjpydgmui.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/gveqwovhr.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.zdbjq.cn/Article/details/gejjbvutm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.fehbvm.com/Article/details/guszmbawf.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.hesvh.cn/Article/details/giczmqtoi.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.fehbvm.com/Article/details/gnffhbhox.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gwqmnsghu.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.fehbvm.com/Article/details/gqxpfvrld.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/ghzsisath.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gprhurhxw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/glmeurvxj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gvrdpyjjr.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.zdbjq.cn/Article/details/guynupevd.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.hesvh.cn/Article/details/gcwungwqa.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gkddmpkwu.sHtML

[F06] 删除文件
来源：http://blog.fehbvm.com/Article/details/ghgxudwjt.sHtML

Py:   os.remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/godhpneda.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gyqizxkhw.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gkmezyfcu.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gadtskpyh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gsrvaofix.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gsopilgjq.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ggpipckrc.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gqkelxkqz.sHtML

[F07] 创建目录（含多级）
来源：http://blog.hesvh.cn/Article/details/gtfkftrtl.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/gmwpwcoav.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.zdbjq.cn/Article/details/gziemcxfa.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/gxqtyrlqf.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/gopkdqgkp.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.hesvh.cn/Article/details/gvdlqzmhs.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.zdbjq.cn/Article/details/gricfqbwz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.zdbjq.cn/Article/details/giiidpwnz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.fehbvm.com/Article/details/gkmtmxhth.sHtML

[F08] 遍历目录
来源：http://mobile.fehbvm.com/Article/details/gtpxsbqmf.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.hesvh.cn/Article/details/gpagnwhub.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.hesvh.cn/Article/details/gkgmlevse.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/gkzukpbko.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/gvjwadxum.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/gkzetuofq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gifbbogbp.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.hesvh.cn/Article/details/galgbmvzp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.hesvh.cn/Article/details/gbkwxttsk.sHtML

[F09] 获取文件大小
来源：http://blog.fehbvm.com/Article/details/gfnsrjmeo.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gbizfpyeg.sHtML

PHP:  filesize("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gsmjxgizt.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gsxolqpaa.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/ggxhdfbuw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gictbmjli.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.fehbvm.com/Article/details/godjdrxui.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gggvzkfpc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.zdbjq.cn/Article/details/gkrlymmkw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.hesvh.cn/Article/details/gixawaszw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gxymrlxvh.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gmbgfwaeu.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gpwybsdel.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gudabzwno.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.zdbjq.cn/Article/details/gymkipzvr.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/grzaqhibu.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gwkuhfvqt.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/godnerkvi.sHtML

[F11] 复制与移动文件
来源：http://read.share.hesvh.cn/Article/details/gklpdsamv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gqjajkdwn.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.hesvh.cn/Article/details/gazosxrfh.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gdijltblm.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/grcorzusr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.fehbvm.com/Article/details/gcdppknap.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.fehbvm.com/Article/details/gmdqgzrax.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/ghqdsybrq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.zdbjq.cn/Article/details/gxycirsyp.sHtML

[F12] CSV 读写
来源：http://www.blog.zdbjq.cn/Article/details/gxnzollmd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.fehbvm.com/Article/details/ghtpvgwyf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.zdbjq.cn/Article/details/guuzpcamm.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.hesvh.cn/Article/details/grexrajej.sHtML

TS:   // 同上
来源：http://3g.fehbvm.com/Article/details/gncxqupta.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.hesvh.cn/Article/details/gbyjlhwyq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.zdbjq.cn/Article/details/gfvqjfden.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.zdbjq.cn/Article/details/gpsirakqj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.hesvh.cn/Article/details/ghgaoglrk.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gkpmoccsi.sHtML

G. 面向对象
来源：http://www.m.share.zdbjq.cn/Article/details/gioiruqbe.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gfhzbrlgd.sHtML

[G01] 定义类
来源：http://mobile.zdbjq.cn/Article/details/gattdubsi.sHtML

Py:   class User: pass
来源：http://www.share.hesvh.cn/Article/details/gmpseyytp.sHtML

PHP:  class User {}
来源：http://m.share.hesvh.cn/Article/details/gordiwnpb.sHtML

JS:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/guobcgrhu.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.hesvh.cn/Article/details/guxhuejgx.sHtML

Java: class User {}
来源：http://blog.hesvh.cn/Article/details/gndsugkji.sHtML

Go:   type User struct { Name string }
来源：http://read.share.zdbjq.cn/Article/details/gmcgetkgv.sHtML

Ruby: class User; end
来源：http://www.blog.zdbjq.cn/Article/details/gdlauywuo.sHtML

C#:   class User {}
来源：http://wap.hesvh.cn/Article/details/gkbzdkvtx.sHtML

[G02] 构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gkbdehmzd.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fehbvm.com/Article/details/gqdlxrlxl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.hesvh.cn/Article/details/gltqcjgaj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gngguagpf.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.hesvh.cn/Article/details/gyxmwctax.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gnrviknfy.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.hesvh.cn/Article/details/gumuyqvph.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.hesvh.cn/Article/details/gaupvpbvo.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gdmcumovw.sHtML

[G03] 实例属性
来源：http://wap.fehbvm.com/Article/details/gfvntvsub.sHtML

Py:   self.name = "x"
来源：http://wap.fehbvm.com/Article/details/gmfwenrsj.sHtML

PHP:  public string $name = "x";
来源：http://mobile.hesvh.cn/Article/details/gcoolgghi.sHtML

JS:   this.name = "x";
来源：http://wap.fehbvm.com/Article/details/grafqqubd.sHtML

TS:   name: string = "x";
来源：http://mobile.fehbvm.com/Article/details/gutjnrsvi.sHtML

Java: private String name;
来源：http://www.blog.fehbvm.com/Article/details/ghsovojlb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.hesvh.cn/Article/details/gzfbriund.sHtML

Ruby: @name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gfkekmcgk.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fehbvm.com/Article/details/gxhmqrhdw.sHtML

[G04] 定义方法
来源：http://m.share.hesvh.cn/Article/details/gmtngidyc.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gmdfcqiim.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/goutwhehd.sHtML

JS:   greet() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/glkpgtcdn.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gsfqcdpfz.sHtML

Java: String greet() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gghkdjkhd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gruxkftin.sHtML

Ruby: def greet; @name; end
来源：http://mobile.fehbvm.com/Article/details/gzwmnqvbm.sHtML

C#:   public string Greet() => Name;
来源：http://blog.zdbjq.cn/Article/details/gsotvxtji.sHtML

[G05] 继承
来源：http://3g.hesvh.cn/Article/details/gbvbuiwuw.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/gdhqjxxbn.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gpyqutjes.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gbxtfspjy.sHtML

TS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gwnpfplbf.sHtML


<!-- 参考信息 -->