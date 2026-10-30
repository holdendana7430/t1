代发 wailian999

C#:   s.Replace("a", "b")
来源：http://baike.hesvh.cn/Article/details/grdawvedd.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.fehbvm.com/Article/details/gubpbdsaq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.zdbjq.cn/Article/details/ghumnavdb.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.fehbvm.com/Article/details/graacopto.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.hesvh.cn/Article/details/gmvtpdwtb.sHtML

TS:   s.split(",")
来源：http://www.blog.fehbvm.com/Article/details/gnhmvcdvc.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.hesvh.cn/Article/details/gjddbpwgd.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.fehbvm.com/Article/details/gjzvzytev.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.fehbvm.com/Article/details/gslmnzxvb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.hesvh.cn/Article/details/gcfignrty.sHtML

[E08] 数组按分隔符合并
来源：http://wap.zdbjq.cn/Article/details/ggehumurv.sHtML

Py:   ",".join(items)
来源：http://blog.fehbvm.com/Article/details/gqmejqpoq.sHtML

PHP:  implode(",", $items);
来源：http://m.share.zdbjq.cn/Article/details/gnzwvjcoa.sHtML

JS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gozzrfxwy.sHtML

TS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gylypbmcu.sHtML

Java: String.join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gthmghrpa.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.fehbvm.com/Article/details/gxjuqawpa.sHtML

Ruby: items.join(",")
来源：http://blog.fehbvm.com/Article/details/gdkdvjgwt.sHtML

C#:   string.Join(",", items)
来源：http://3g.fehbvm.com/Article/details/gjyaayxnn.sHtML

[E09] 去除所有空白字符
来源：http://m.share.hesvh.cn/Article/details/gdmpwmczv.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.zdbjq.cn/Article/details/gjbesbbsz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.zdbjq.cn/Article/details/gczbyhshv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/gqfqhaclx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gysprkwwc.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/ggfexhgoj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.fehbvm.com/Article/details/gihdgydzg.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.fehbvm.com/Article/details/gdfdoazdg.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gjgnuzprn.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.hesvh.cn/Article/details/ggsqovzhp.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/grcfkuady.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.hesvh.cn/Article/details/gcbyyhqlz.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gserototj.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/ghciuogir.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gozqqbsyo.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gbxhbnaxh.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gyttaibmc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.zdbjq.cn/Article/details/ghwqpfavx.sHtML

[E11] 反转字符串
来源：http://www.share.fehbvm.com/Article/details/gmiudkgjo.sHtML

Py:   s[::-1]
来源：http://wap.zdbjq.cn/Article/details/gvkqvdswh.sHtML

PHP:  strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gjsqisscm.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gsuagvryk.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gopptzmuz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.hesvh.cn/Article/details/gjhzgctaf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.hesvh.cn/Article/details/gmhlillat.sHtML

Ruby: s.reverse
来源：http://wap.hesvh.cn/Article/details/ghqbowuhi.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/ghxmcaezc.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.hesvh.cn/Article/details/gkjzijieq.sHtML

Py:   s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gvkxmersy.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.hesvh.cn/Article/details/geunuzvep.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gjwrqgcvc.sHtML

TS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/gexlkzprv.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.hesvh.cn/Article/details/guatqbyng.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.hesvh.cn/Article/details/gvhmuxcyz.sHtML

Ruby: s.count("a")
来源：http://blog.hesvh.cn/Article/details/gbkpcthqn.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.zdbjq.cn/Article/details/gxxztkijh.sHtML

[E13] 逐字符遍历
来源：http://m.share.zdbjq.cn/Article/details/giyudwhbc.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.fehbvm.com/Article/details/gvdandttd.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.zdbjq.cn/Article/details/grakixkoi.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/glktuwqxy.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/gqmulpbxr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.zdbjq.cn/Article/details/gkmtxoaqf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.hesvh.cn/Article/details/gjhywptly.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.zdbjq.cn/Article/details/gwauyrzfr.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.fehbvm.com/Article/details/ghwqrgvan.sHtML

[E14] URL 编码与 Base64
来源：http://baike.hesvh.cn/Article/details/gaydkvcje.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.zdbjq.cn/Article/details/gddzarthd.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.hesvh.cn/Article/details/gibxpzwig.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.hesvh.cn/Article/details/gktebnobv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.hesvh.cn/Article/details/ghncoseti.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.hesvh.cn/Article/details/gggyxdezu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.hesvh.cn/Article/details/gydmsoehp.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.zdbjq.cn/Article/details/gucidescq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.fehbvm.com/Article/details/gamuiecia.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.fehbvm.com/Article/details/guunsdgfn.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.zdbjq.cn/Article/details/gnuobhzwx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.hesvh.cn/Article/details/giffvzsgc.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.zdbjq.cn/Article/details/gstuammdx.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.zdbjq.cn/Article/details/gqaffiyzx.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.hesvh.cn/Article/details/grdkpmjew.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.fehbvm.com/Article/details/grokcfajm.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.zdbjq.cn/Article/details/gqklplzbc.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.hesvh.cn/Article/details/ginjoccnw.sHtML

[E16] 数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/gkmezogbi.sHtML

Py:   f"{1234567:,}"
来源：http://wap.fehbvm.com/Article/details/gvyquuecy.sHtML

PHP:  number_format(1234567);
来源：http://mobile.zdbjq.cn/Article/details/gwzlxeovw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gpluyxspm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/gwvyycjvb.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.hesvh.cn/Article/details/gcgcbzymg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.hesvh.cn/Article/details/gumrzyzhj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.zdbjq.cn/Article/details/gvihncdzu.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.hesvh.cn/Article/details/gkgidekoc.sHtML

[E17] 首字母大写
来源：http://mobile.fehbvm.com/Article/details/gbvhtskbp.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.zdbjq.cn/Article/details/gcpenzfaw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.zdbjq.cn/Article/details/gjzbhzeug.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gsnhjtyjs.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/gtzopmwgn.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.hesvh.cn/Article/details/gdsplojfx.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.hesvh.cn/Article/details/gfkfojaju.sHtML

Ruby: s.capitalize
来源：http://www.blog.hesvh.cn/Article/details/gcdgiyheb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.fehbvm.com/Article/details/gfyccqezx.sHtML

[E18] 模板占位符替换
来源：http://3g.hesvh.cn/Article/details/gqbgkhuyp.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.zdbjq.cn/Article/details/gkfyjfute.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.fehbvm.com/Article/details/gaaqledkb.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gsbgvpwxx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gaxxmsfbm.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gpdwikfjn.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/ghqfojjnl.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.zdbjq.cn/Article/details/gqqwxvozv.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.hesvh.cn/Article/details/gjpmcqshs.sHtML

[E19] 多行文本按行拆分
来源：http://wap.hesvh.cn/Article/details/grsrbrowg.sHtML

Py:   s.splitlines()
来源：http://m.share.zdbjq.cn/Article/details/gwrofjixp.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.hesvh.cn/Article/details/gbjuwgvvx.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gzfxepcxz.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/gqswehfex.sHtML

Java: s.lines().toList()
来源：http://www.blog.fehbvm.com/Article/details/gmqokqosu.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.zdbjq.cn/Article/details/gklxurnsq.sHtML

Ruby: s.lines
来源：http://www.blog.zdbjq.cn/Article/details/ghxkfjtoz.sHtML

C#:   s.Split('\n')
来源：http://m.share.hesvh.cn/Article/details/geisyqbvn.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.hesvh.cn/Article/details/gfyuqhwly.sHtML

Py:   if not s:
来源：http://www.share.fehbvm.com/Article/details/guhnuxfid.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.fehbvm.com/Article/details/gwtdwlibr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.fehbvm.com/Article/details/ggbibfszs.sHtML

TS:   if (s === "") {}
来源：http://www.share.fehbvm.com/Article/details/gjkyckbqr.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gwhiyolht.sHtML

Go:   if s == "" {}
来源：http://www.blog.hesvh.cn/Article/details/gubhrxzoy.sHtML

Ruby: if s.empty?
来源：http://www.m.share.zdbjq.cn/Article/details/gwdcjkuyz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcfjzycxl.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.fehbvm.com/Article/details/gpqzkokmb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fehbvm.com/Article/details/glgzrcyrh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gvsuufshy.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/grzettffs.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gonggavbs.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gzavuyydx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.hesvh.cn/Article/details/gxbztymum.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gebatwhdc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gdhtfkahj.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.hesvh.cn/Article/details/gdcdpkszr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.zdbjq.cn/Article/details/gggvdrpax.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gqhwvvzyb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/ghvrtbyaf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/gksxjcdat.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.hesvh.cn/Article/details/gigxgauid.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fehbvm.com/Article/details/gkanunjpe.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.hesvh.cn/Article/details/glyednoxk.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.fehbvm.com/Article/details/ggtrtzufa.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gbeywnywb.sHtML

F. 文件与目录
来源：http://wap.hesvh.cn/Article/details/grqyoaawx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gnduvwjao.sHtML

[F01] 读取整个文件
来源：http://blog.zdbjq.cn/Article/details/goimekhsx.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.hesvh.cn/Article/details/gzyqfilli.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.hesvh.cn/Article/details/ggsfwavwe.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.fehbvm.com/Article/details/gzcqzwpqv.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gsqtodswn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gjuvcsmte.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.hesvh.cn/Article/details/grxndskly.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.hesvh.cn/Article/details/giwabfsnr.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gocdkrlvt.sHtML

[F02] 逐行读取文件
来源：http://wap.zdbjq.cn/Article/details/girvvaflf.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.zdbjq.cn/Article/details/gcszulnld.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.zdbjq.cn/Article/details/gcdcncyyc.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/gdjpcuucg.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gznvnrwsr.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/gpnjcaaod.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.hesvh.cn/Article/details/gburtpnve.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.fehbvm.com/Article/details/gwiteyyrt.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.fehbvm.com/Article/details/ghubnpzpw.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.fehbvm.com/Article/details/gtwxudkyn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.fehbvm.com/Article/details/gxtzecvhu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/gbcwzipnq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/gsijsrykb.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gtwuepuib.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.zdbjq.cn/Article/details/ghuzwrbys.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fehbvm.com/Article/details/gpannnsat.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.fehbvm.com/Article/details/gxzrgsmvy.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gnuiolvye.sHtML

[F04] 追加写入文件
来源：http://www.blog.zdbjq.cn/Article/details/gftbauaza.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.fehbvm.com/Article/details/gqshftsyi.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.zdbjq.cn/Article/details/gxbpfpoje.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/glucpgevf.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gtcbdizxb.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.fehbvm.com/Article/details/gybavfqhc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fehbvm.com/Article/details/gswdmoqsc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.hesvh.cn/Article/details/gxisfodpp.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.zdbjq.cn/Article/details/gfaaissvy.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.zdbjq.cn/Article/details/gfhpfkrhr.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.zdbjq.cn/Article/details/gfdremtav.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.hesvh.cn/Article/details/glvcotwkg.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gfdsuiatl.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gsfbemkjc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gxwlasesb.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.zdbjq.cn/Article/details/gzzldowye.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.hesvh.cn/Article/details/gfkvzunpa.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gnmlmgnbf.sHtML

[F06] 删除文件
来源：http://read.share.hesvh.cn/Article/details/gpukqqckx.sHtML

Py:   os.remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/ghsfdxcyf.sHtML

PHP:  unlink("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gmckoyzkr.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/guklntmns.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gxnazipqv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gumuxqvyb.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gsreubikz.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gvwbexklu.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gdenbuems.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.hesvh.cn/Article/details/gxtirnnux.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gajmavqlx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.fehbvm.com/Article/details/gnzkmnfut.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gfpdpclsb.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/gubmidlal.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fehbvm.com/Article/details/gsagvfpmg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fehbvm.com/Article/details/ganvhkums.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.hesvh.cn/Article/details/gjmxoblcy.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.fehbvm.com/Article/details/gllqsevhd.sHtML

[F08] 遍历目录
来源：http://m.share.zdbjq.cn/Article/details/guaazbxdu.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.zdbjq.cn/Article/details/gubfnrocl.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fehbvm.com/Article/details/gbetgfefq.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/guhzyxjra.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/gpdxepwxp.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gyzoykdnw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.zdbjq.cn/Article/details/gshbkrvqd.sHtML

Ruby: Dir.children("dir")
来源：http://blog.zdbjq.cn/Article/details/gtwrxddxh.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.zdbjq.cn/Article/details/glbdhpxif.sHtML

[F09] 获取文件大小
来源：http://www.share.hesvh.cn/Article/details/gjdrghdsh.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.zdbjq.cn/Article/details/ghiesvwmc.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.fehbvm.com/Article/details/grfrhumct.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gyzvczyhk.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gvnhreikt.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/galclupuq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.zdbjq.cn/Article/details/gbqfqgnip.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gkahlgtwt.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.hesvh.cn/Article/details/gekubvbmm.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.zdbjq.cn/Article/details/gtpbgssbu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/glrefiohi.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.zdbjq.cn/Article/details/gqpswtlaa.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/ggmobvaum.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gdhnvthzo.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.zdbjq.cn/Article/details/gipxbooya.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gmdtkrsnl.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gjxqxrglw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gnqyffufj.sHtML

[F11] 复制与移动文件
来源：http://read.share.hesvh.cn/Article/details/gunsifbke.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/grwrotouv.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gepkeqywk.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gcndwzxti.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gkikhxuzs.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.zdbjq.cn/Article/details/gkwrhkbni.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.zdbjq.cn/Article/details/ggsyzikwm.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gdhekxxnz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.zdbjq.cn/Article/details/gmzymizda.sHtML

[F12] CSV 读写
来源：http://wap.zdbjq.cn/Article/details/gxcsckxyd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.hesvh.cn/Article/details/gwuagmmex.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.hesvh.cn/Article/details/gqqeqcawy.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.zdbjq.cn/Article/details/gchecsldz.sHtML

TS:   // 同上
来源：http://www.blog.zdbjq.cn/Article/details/guryovwig.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.fehbvm.com/Article/details/grgaqjkad.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.hesvh.cn/Article/details/gdtcbdxem.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.fehbvm.com/Article/details/ggkoxdisc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.hesvh.cn/Article/details/ggwijhyen.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gnobjqavp.sHtML

G. 面向对象
来源：http://www.blog.fehbvm.com/Article/details/gbdnywscj.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gwcrfdcos.sHtML

[G01] 定义类
来源：http://www.blog.hesvh.cn/Article/details/gqxzpibky.sHtML

Py:   class User: pass
来源：http://www.m.share.hesvh.cn/Article/details/geoeylpgp.sHtML

PHP:  class User {}
来源：http://read.share.zdbjq.cn/Article/details/garocaior.sHtML

JS:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gwkwxkjte.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.zdbjq.cn/Article/details/gndsohvim.sHtML

Java: class User {}
来源：http://mobile.hesvh.cn/Article/details/gtezckeds.sHtML

Go:   type User struct { Name string }
来源：http://3g.fehbvm.com/Article/details/gzrerdogy.sHtML

Ruby: class User; end
来源：http://read.share.hesvh.cn/Article/details/gtvyyxtau.sHtML

C#:   class User {}
来源：http://blog.fehbvm.com/Article/details/gredvnkdc.sHtML

[G02] 构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gbphjjvby.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.fehbvm.com/Article/details/gnnvgorsf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.zdbjq.cn/Article/details/gybcbjzbo.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gfhorfgsg.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.hesvh.cn/Article/details/giqhdqjrb.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gyrokmrru.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.hesvh.cn/Article/details/gkgvfdzui.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.hesvh.cn/Article/details/ggrbsljyo.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.fehbvm.com/Article/details/gcnuyhgpx.sHtML

[G03] 实例属性
来源：http://blog.fehbvm.com/Article/details/gfvvwxikm.sHtML

Py:   self.name = "x"
来源：http://read.share.hesvh.cn/Article/details/gidhqstip.sHtML

PHP:  public string $name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gxpvtwupa.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/gpismltip.sHtML

TS:   name: string = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gifaxxdhd.sHtML

Java: private String name;
来源：http://www.share.zdbjq.cn/Article/details/grbkpwudj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.hesvh.cn/Article/details/gjxhwlfvh.sHtML

Ruby: @name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gaforubxg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.zdbjq.cn/Article/details/glyoprnio.sHtML

[G04] 定义方法
来源：http://read.share.fehbvm.com/Article/details/gkbyepjab.sHtML

Py:   def greet(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gqucraktm.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/grnwpvbnm.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/ghdtkcfgw.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/grtkdzlip.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/grlsqpyqr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gfqechkxh.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gebaqhfsj.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.hesvh.cn/Article/details/gqdfymshv.sHtML

[G05] 继承
来源：http://wap.hesvh.cn/Article/details/gvxrbpsjq.sHtML

Py:   class Admin(User): pass
来源：http://m.share.hesvh.cn/Article/details/gvfgxqwgs.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjfirthgq.sHtML

JS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/ggnfplhfz.sHtML

TS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gausfcskj.sHtML


<!-- 参考信息 -->