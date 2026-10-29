代发 wailian999

Ruby: s.split(",");  s.split
来源：http://mobile.fehbvm.com/Article/details/gqaovdxbe.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.zdbjq.cn/Article/details/gdyjnonqt.sHtML

[E08] 数组按分隔符合并
来源：http://wap.hesvh.cn/Article/details/gtqewduxs.sHtML

Py:   ",".join(items)
来源：http://read.share.hesvh.cn/Article/details/gytptaojo.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.fehbvm.com/Article/details/gchmixagg.sHtML

JS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gpnbaymyx.sHtML

TS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gkkjsusea.sHtML

Java: String.join(",", items)
来源：http://blog.zdbjq.cn/Article/details/gruugezbl.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.hesvh.cn/Article/details/gzrhgtzkv.sHtML

Ruby: items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gfoctmgjk.sHtML

C#:   string.Join(",", items)
来源：http://wap.hesvh.cn/Article/details/gcngypkjg.sHtML

[E09] 去除所有空白字符
来源：http://mobile.fehbvm.com/Article/details/gsnwveelz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gcyiqvqne.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gxdcgwhef.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/goddwzptj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/gjmksysso.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.hesvh.cn/Article/details/gpwzaazfr.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.fehbvm.com/Article/details/gnizxrhwb.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.fehbvm.com/Article/details/gnrzisgyb.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.hesvh.cn/Article/details/gnsaxkgdy.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.zdbjq.cn/Article/details/gtcxxqzwv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gkzyyzaex.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.hesvh.cn/Article/details/gickhmqrl.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gnsxapdvk.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/genvhceew.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/glcakutmg.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/ghitooykg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gtghswmut.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.zdbjq.cn/Article/details/gstyyauoh.sHtML

[E11] 反转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gdogwepuv.sHtML

Py:   s[::-1]
来源：http://blog.hesvh.cn/Article/details/grvnwfozs.sHtML

PHP:  strrev($s);
来源：http://blog.hesvh.cn/Article/details/gyvydoctx.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gzqgfagro.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/giqdflhok.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.hesvh.cn/Article/details/gzlgmqhpi.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.fehbvm.com/Article/details/gdixmijnn.sHtML

Ruby: s.reverse
来源：http://m.share.fehbvm.com/Article/details/gozxhdhyt.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gpyxktxpu.sHtML

[E12] 统计某字符出现次数
来源：http://blog.fehbvm.com/Article/details/gwfcmzbmr.sHtML

Py:   s.count("a")
来源：http://read.share.fehbvm.com/Article/details/glajfdhhw.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.hesvh.cn/Article/details/gqrppteyh.sHtML

JS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/gdfuulylx.sHtML

TS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/gsmvhltjk.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.fehbvm.com/Article/details/glbtxfxmo.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.zdbjq.cn/Article/details/gftekugot.sHtML

Ruby: s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gelwvgwpn.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.hesvh.cn/Article/details/gvczxsdwi.sHtML

[E13] 逐字符遍历
来源：http://www.blog.fehbvm.com/Article/details/gialitmdl.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.zdbjq.cn/Article/details/giqyxxkwx.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.zdbjq.cn/Article/details/gaenvyokf.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gfghpkggh.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/gkgutfvef.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.fehbvm.com/Article/details/gungoxxce.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.hesvh.cn/Article/details/gaplkdpbs.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fehbvm.com/Article/details/gadngieue.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.fehbvm.com/Article/details/gbxpnpdmw.sHtML

[E14] URL 编码与 Base64
来源：http://baike.zdbjq.cn/Article/details/gatxsibih.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.zdbjq.cn/Article/details/gjxocabdj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.zdbjq.cn/Article/details/girwmbmdi.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.fehbvm.com/Article/details/gxrobvhpk.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.zdbjq.cn/Article/details/gmfrhufyo.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gqrretoop.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.hesvh.cn/Article/details/gyuiqytbx.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.fehbvm.com/Article/details/guluklwin.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.fehbvm.com/Article/details/gkjrpcsld.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.zdbjq.cn/Article/details/gniklautq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.fehbvm.com/Article/details/gvmjtlnvt.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.zdbjq.cn/Article/details/gpmjpfwiw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fehbvm.com/Article/details/gnylxaent.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.zdbjq.cn/Article/details/gmjetjsvl.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.hesvh.cn/Article/details/gpylscsvj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.fehbvm.com/Article/details/gtcjhzcbd.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.hesvh.cn/Article/details/gfvynfszr.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.zdbjq.cn/Article/details/gdkcpwixj.sHtML

[E16] 数字千分位
来源：http://3g.fehbvm.com/Article/details/gadmquemh.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.zdbjq.cn/Article/details/gxtnaynwp.sHtML

PHP:  number_format(1234567);
来源：http://3g.zdbjq.cn/Article/details/ggbapvldf.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/gyxzlaovq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/gbdegflpk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.fehbvm.com/Article/details/gxikpjaiy.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.hesvh.cn/Article/details/gwgikvnli.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.hesvh.cn/Article/details/ginsdcojh.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.fehbvm.com/Article/details/gslnlkots.sHtML

[E17] 首字母大写
来源：http://www.blog.hesvh.cn/Article/details/gaytaczex.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.zdbjq.cn/Article/details/gujzvtilw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.zdbjq.cn/Article/details/girxpzmpx.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gpfvdxdff.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gpijvatpg.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.fehbvm.com/Article/details/guboyalrh.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.fehbvm.com/Article/details/gkmwodwwu.sHtML

Ruby: s.capitalize
来源：http://m.share.zdbjq.cn/Article/details/gmxnjprmn.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.hesvh.cn/Article/details/gtlfidwcy.sHtML

[E18] 模板占位符替换
来源：http://wap.zdbjq.cn/Article/details/gxbuxqgnb.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.fehbvm.com/Article/details/giucohcyg.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.hesvh.cn/Article/details/gibtrfpql.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gfqsxzwxo.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/ggasxdinv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gpyssovcg.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.fehbvm.com/Article/details/gzqprsdts.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.hesvh.cn/Article/details/gvybqyuyc.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.hesvh.cn/Article/details/grwjpkosq.sHtML

[E19] 多行文本按行拆分
来源：http://wap.hesvh.cn/Article/details/gtvsdydcb.sHtML

Py:   s.splitlines()
来源：http://baike.fehbvm.com/Article/details/gzpshsqag.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/ghjjogsiw.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gmhfxnjin.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gxuknyfdw.sHtML

Java: s.lines().toList()
来源：http://wap.hesvh.cn/Article/details/gvtbyxpdd.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.fehbvm.com/Article/details/gnfkwjbto.sHtML

Ruby: s.lines
来源：http://www.share.fehbvm.com/Article/details/gwxrbpczd.sHtML

C#:   s.Split('\n')
来源：http://read.share.hesvh.cn/Article/details/gkbxgoqys.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fehbvm.com/Article/details/ggmttlbyb.sHtML

Py:   if not s:
来源：http://3g.fehbvm.com/Article/details/gbuflmkqj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.hesvh.cn/Article/details/geghdemjj.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.fehbvm.com/Article/details/gvnuvvhcv.sHtML

TS:   if (s === "") {}
来源：http://blog.hesvh.cn/Article/details/gotgougoj.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gejmdpjye.sHtML

Go:   if s == "" {}
来源：http://m.share.fehbvm.com/Article/details/gugclntjt.sHtML

Ruby: if s.empty?
来源：http://m.share.fehbvm.com/Article/details/gbmrqdduf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.zdbjq.cn/Article/details/gnwyrxyih.sHtML

[E21] 超长截断加省略号
来源：http://www.share.zdbjq.cn/Article/details/gmjpvitzz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fehbvm.com/Article/details/gqmsckbnu.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gvcfzyeot.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gkpindicr.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gvauyecea.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/grpulgsny.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.fehbvm.com/Article/details/gurjqanen.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gqtokmobw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gjplvqyco.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.zdbjq.cn/Article/details/gjzbwaxwn.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.zdbjq.cn/Article/details/gpdnwkpvr.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gvrhhnfhj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gtlexnfpn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gifageycv.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.hesvh.cn/Article/details/gqjvkwgzd.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.zdbjq.cn/Article/details/ggvwruhaa.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.hesvh.cn/Article/details/gboghjbcu.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.hesvh.cn/Article/details/gbybrtuvx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gddfpsmqs.sHtML

F. 文件与目录
来源：http://blog.hesvh.cn/Article/details/glckxtbdn.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gxmanmzaf.sHtML

[F01] 读取整个文件
来源：http://blog.hesvh.cn/Article/details/gatfvglby.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.fehbvm.com/Article/details/gxqlshorc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.fehbvm.com/Article/details/gagmuxzvx.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.fehbvm.com/Article/details/gnvgjmmvq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gutngonqb.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gvqslbjdx.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.hesvh.cn/Article/details/gdzkgdpmw.sHtML

Ruby: File.read("a.txt")
来源：http://baike.hesvh.cn/Article/details/gauvcdzab.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.fehbvm.com/Article/details/grcdyedwk.sHtML

[F02] 逐行读取文件
来源：http://blog.fehbvm.com/Article/details/gcvdojebn.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.fehbvm.com/Article/details/gllwkfnrb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.hesvh.cn/Article/details/gjmogqarr.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gpxavkbkn.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/gwgquocqi.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/ghvmegscb.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.fehbvm.com/Article/details/gxusvesvp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.zdbjq.cn/Article/details/gxjczvuil.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.hesvh.cn/Article/details/gwbvdtoxy.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.hesvh.cn/Article/details/gnptwlzqg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.zdbjq.cn/Article/details/gptbyhtge.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/gdnvmycqp.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/gomanrhav.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/grwwlizpa.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.hesvh.cn/Article/details/gudwlykna.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.zdbjq.cn/Article/details/gcvdvgyho.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.zdbjq.cn/Article/details/gpxyephky.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/geguvaqly.sHtML

[F04] 追加写入文件
来源：http://www.share.zdbjq.cn/Article/details/gxgxdxnbt.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gryclccss.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.hesvh.cn/Article/details/gmyiuagnf.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/gocqscpjc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/gmcwdmeji.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.hesvh.cn/Article/details/gsyaldbnz.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.hesvh.cn/Article/details/gwitjafbe.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.hesvh.cn/Article/details/gewybbkca.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.fehbvm.com/Article/details/gpzcrkfkg.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.fehbvm.com/Article/details/gwytkfpxf.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.zdbjq.cn/Article/details/gryiwscum.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gqlneqtkh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gokrnkvyl.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gmecxncqh.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/ggfztyxup.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.fehbvm.com/Article/details/gfrpwvugj.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gdixocypa.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/guyamcjgx.sHtML

[F06] 删除文件
来源：http://3g.fehbvm.com/Article/details/gwwrdmgze.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gjigxodzq.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gfmyoubsk.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/guagebxow.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gbrfutoib.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/ggemejxlj.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gmvicnmlg.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gnmaxlkfq.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.fehbvm.com/Article/details/ggnaopejo.sHtML

[F07] 创建目录（含多级）
来源：http://wap.hesvh.cn/Article/details/goqtzvfqw.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gjbwoajpb.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.fehbvm.com/Article/details/gqmgqilzv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/gmswtuupf.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gsqxcgiyp.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.fehbvm.com/Article/details/goevftgjp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.fehbvm.com/Article/details/gexlwdjoh.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.zdbjq.cn/Article/details/geumjupjn.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.fehbvm.com/Article/details/ghnebweut.sHtML

[F08] 遍历目录
来源：http://m.share.fehbvm.com/Article/details/gprvsykza.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.hesvh.cn/Article/details/gkmhdgutn.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.hesvh.cn/Article/details/gawzylrdn.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/giwquagir.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gzjzkqxot.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gkfpcnapt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.zdbjq.cn/Article/details/gemjpbece.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fehbvm.com/Article/details/ggmwbsajx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fehbvm.com/Article/details/gptnpbsxr.sHtML

[F09] 获取文件大小
来源：http://3g.fehbvm.com/Article/details/gfpzzzmno.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gdsmceiix.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/goipvqrqf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/gitdlxreb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/ghrbgfnbq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gemrrvmgc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.fehbvm.com/Article/details/gcnaugxls.sHtML

Ruby: File.size("a.txt")
来源：http://baike.zdbjq.cn/Article/details/ggclmicic.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.fehbvm.com/Article/details/gqcvmvdhl.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.zdbjq.cn/Article/details/gxyiljnvu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gclrgeuai.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gplrsttwx.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gdnxtamcd.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gdrhddzsc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.fehbvm.com/Article/details/gicitlhma.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gkttclueb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gdenxyvdl.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/guissqefe.sHtML

[F11] 复制与移动文件
来源：http://m.share.zdbjq.cn/Article/details/gntrnaaag.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gbzvzixkb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.fehbvm.com/Article/details/gozxqpsdk.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gcpaxsogi.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gdqrijijl.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.fehbvm.com/Article/details/gwdfukbqv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.fehbvm.com/Article/details/gmqtmvjkf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gsjnjtycl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.zdbjq.cn/Article/details/gvghojjsx.sHtML

[F12] CSV 读写
来源：http://baike.hesvh.cn/Article/details/gsxrupzzt.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.hesvh.cn/Article/details/gruxaiswt.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.hesvh.cn/Article/details/gpzxbybpi.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.hesvh.cn/Article/details/glostusvy.sHtML

TS:   // 同上
来源：http://baike.hesvh.cn/Article/details/gcgwasymo.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.hesvh.cn/Article/details/gdhhnoegz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.hesvh.cn/Article/details/gkdsxgdoq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fehbvm.com/Article/details/gekzmjqhd.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.hesvh.cn/Article/details/gpxasmclw.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gzawjxiho.sHtML

G. 面向对象
来源：http://blog.hesvh.cn/Article/details/gpvcpzfoy.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gvaxrbqpi.sHtML

[G01] 定义类
来源：http://3g.fehbvm.com/Article/details/gmlqcvvwt.sHtML

Py:   class User: pass
来源：http://www.share.fehbvm.com/Article/details/gegclopug.sHtML

PHP:  class User {}
来源：http://www.share.zdbjq.cn/Article/details/ggjicvfpg.sHtML

JS:   class User {}
来源：http://blog.fehbvm.com/Article/details/gokdsgsuy.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.hesvh.cn/Article/details/giaxmxtns.sHtML

Java: class User {}
来源：http://read.share.fehbvm.com/Article/details/genymqjup.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.zdbjq.cn/Article/details/gxxqhlvpw.sHtML

Ruby: class User; end
来源：http://mobile.fehbvm.com/Article/details/gzjdahskl.sHtML

C#:   class User {}
来源：http://baike.fehbvm.com/Article/details/gmarnhgvk.sHtML

[G02] 构造函数
来源：http://3g.hesvh.cn/Article/details/gvsonjlhc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fehbvm.com/Article/details/gvywgjrzm.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fehbvm.com/Article/details/gapdwqpuj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gokrlpmph.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.hesvh.cn/Article/details/gcplebkwg.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gzselwmbq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.hesvh.cn/Article/details/gjfrmdtyr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fehbvm.com/Article/details/ghotgouuh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.zdbjq.cn/Article/details/gwrpdtirt.sHtML

[G03] 实例属性
来源：http://wap.hesvh.cn/Article/details/gtocmitrd.sHtML

Py:   self.name = "x"
来源：http://mobile.fehbvm.com/Article/details/ggdbvzwfz.sHtML

PHP:  public string $name = "x";
来源：http://www.share.zdbjq.cn/Article/details/ggrfuiuue.sHtML

JS:   this.name = "x";
来源：http://m.share.hesvh.cn/Article/details/gdepmyqhe.sHtML

TS:   name: string = "x";
来源：http://wap.fehbvm.com/Article/details/gmupsdimb.sHtML

Java: private String name;
来源：http://www.m.share.hesvh.cn/Article/details/ggwjxtfnc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.zdbjq.cn/Article/details/gaczgbqhc.sHtML

Ruby: @name = "x"
来源：http://wap.zdbjq.cn/Article/details/gbhfeyvfm.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.hesvh.cn/Article/details/gizujlkhx.sHtML

[G04] 定义方法
来源：http://mobile.fehbvm.com/Article/details/gevnczfsn.sHtML

Py:   def greet(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gjqifarbw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gklcefmew.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/grjsnwspz.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gbwcvbsbx.sHtML

Java: String greet() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gfjywbltg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gaytmdjst.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fehbvm.com/Article/details/guhyapzid.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.hesvh.cn/Article/details/gdkzlvrek.sHtML

[G05] 继承
来源：http://m.share.fehbvm.com/Article/details/gnzrxdlta.sHtML

Py:   class Admin(User): pass
来源：http://www.share.zdbjq.cn/Article/details/ggbqeyuif.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gavhicrgu.sHtML

JS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gmqjspxql.sHtML

TS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gypkfiwkp.sHtML

Java: class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/ghynushnz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fehbvm.com/Article/details/gazhjnxkl.sHtML

Ruby: class Admin < User; end
来源：http://mobile.zdbjq.cn/Article/details/gvgakasia.sHtML

C#:   class Admin : User {}
来源：http://m.share.zdbjq.cn/Article/details/gutsmrone.sHtML

[G06] 重写方法
来源：http://read.share.zdbjq.cn/Article/details/gujjpiudt.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.zdbjq.cn/Article/details/gdrkcgpiv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gkntrzwwq.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gssetluag.sHtML


<!-- 参考信息 -->