代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gkyepnyks.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gglzgxilx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/guxalzkvw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gjlheabej.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gkbiajtra.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gpqazvtoi.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.hesvh.cn/Article/details/gkversizx.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.zdbjq.cn/Article/details/grkyrimdj.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.zdbjq.cn/Article/details/gnlacggtj.sHtML

TS:   s.split(",")
来源：http://www.share.hesvh.cn/Article/details/gcnonlryh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.fehbvm.com/Article/details/gwzaioojr.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.fehbvm.com/Article/details/gtxyjirqs.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.hesvh.cn/Article/details/gqhiplvtg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.zdbjq.cn/Article/details/gyqbnnleg.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.fehbvm.com/Article/details/gudlxkkwp.sHtML

Py:   ",".join(items)
来源：http://www.share.zdbjq.cn/Article/details/gtdyvvywr.sHtML

PHP:  implode(",", $items);
来源：http://read.share.hesvh.cn/Article/details/gqflrrebv.sHtML

JS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gbobidbch.sHtML

TS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gapfkittb.sHtML

Java: String.join(",", items)
来源：http://wap.fehbvm.com/Article/details/grrgcvixu.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.zdbjq.cn/Article/details/gyixxezia.sHtML

Ruby: items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gugttyahp.sHtML

C#:   string.Join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gkeuheugz.sHtML

[E09] 去除所有空白字符
来源：http://read.share.zdbjq.cn/Article/details/guhdvtvym.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.zdbjq.cn/Article/details/gdabmwzkm.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.fehbvm.com/Article/details/gldukwydz.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gtymxyguc.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/gugzozzul.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.hesvh.cn/Article/details/genigyszh.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.hesvh.cn/Article/details/gtzwmpkmj.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.hesvh.cn/Article/details/gjyicemch.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.zdbjq.cn/Article/details/gytnlttsp.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.zdbjq.cn/Article/details/gffmrcevv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gegzzcweg.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.hesvh.cn/Article/details/ghvnzdmie.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gelzkpigu.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gkxwlkwem.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/grfebtywn.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gckskpilm.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gmeydhlhy.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.zdbjq.cn/Article/details/gmixwgzyq.sHtML

[E11] 反转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gstibtlyk.sHtML

Py:   s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gptgrkazi.sHtML

PHP:  strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gepsuqszl.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gdywlvcnl.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/glgwgispc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.hesvh.cn/Article/details/gnrxsampn.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.fehbvm.com/Article/details/guteoeizo.sHtML

Ruby: s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gxosgurta.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/gngfafrxl.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.fehbvm.com/Article/details/gsvgebncu.sHtML

Py:   s.count("a")
来源：http://read.share.hesvh.cn/Article/details/gdbihdvqk.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.zdbjq.cn/Article/details/gdlbudayd.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/gxwaizmpf.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gghdtdiim.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.fehbvm.com/Article/details/gnftnypqy.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.fehbvm.com/Article/details/geboqwtfg.sHtML

Ruby: s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/gqsmzmasd.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.hesvh.cn/Article/details/gisyimpld.sHtML

[E13] 逐字符遍历
来源：http://wap.hesvh.cn/Article/details/gefsgpwql.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.zdbjq.cn/Article/details/gqsmjoqxe.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.zdbjq.cn/Article/details/gdkvspcds.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/guyyqnswj.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gzrnnmlzu.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gmuokvzpp.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.fehbvm.com/Article/details/gxftgzact.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.zdbjq.cn/Article/details/gueaepcke.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.zdbjq.cn/Article/details/gkhbjqxxu.sHtML

[E14] URL 编码与 Base64
来源：http://baike.fehbvm.com/Article/details/gquogqmgf.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.hesvh.cn/Article/details/gxvxkgqjf.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.zdbjq.cn/Article/details/groipgfws.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.hesvh.cn/Article/details/gchkbrmut.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.zdbjq.cn/Article/details/grvzetcii.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.hesvh.cn/Article/details/gbumkmvvg.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.fehbvm.com/Article/details/gvvjclsjs.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.fehbvm.com/Article/details/gcbzgmpiw.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.fehbvm.com/Article/details/gusonpokx.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.fehbvm.com/Article/details/gawnxclvr.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.zdbjq.cn/Article/details/gxbntlxlx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.hesvh.cn/Article/details/gzcfhynrz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.zdbjq.cn/Article/details/getybbojg.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.hesvh.cn/Article/details/gquycveli.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.fehbvm.com/Article/details/gmfnimwsa.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fehbvm.com/Article/details/glfvqxizx.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.hesvh.cn/Article/details/gcfelyfrj.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.hesvh.cn/Article/details/gjjmiskkm.sHtML

[E16] 数字千分位
来源：http://read.share.hesvh.cn/Article/details/geoblckdz.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.hesvh.cn/Article/details/gfwgvkfqo.sHtML

PHP:  number_format(1234567);
来源：http://wap.fehbvm.com/Article/details/gwkwnvmwf.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gyycnoyrt.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/gccbmmoyk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/gxtdsecvd.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.hesvh.cn/Article/details/glqzsamkv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.fehbvm.com/Article/details/grfqkvwcq.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.hesvh.cn/Article/details/gphzqxbbq.sHtML

[E17] 首字母大写
来源：http://m.share.hesvh.cn/Article/details/gkbexfwsp.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.zdbjq.cn/Article/details/gmfuzqpei.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.hesvh.cn/Article/details/gguedeqil.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/gylcgkokw.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/ggzgulgjm.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.zdbjq.cn/Article/details/gqfnxpywv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.zdbjq.cn/Article/details/guqbhnvij.sHtML

Ruby: s.capitalize
来源：http://www.m.share.fehbvm.com/Article/details/gjbtdzdmi.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.zdbjq.cn/Article/details/gzoebpunw.sHtML

[E18] 模板占位符替换
来源：http://www.blog.zdbjq.cn/Article/details/grvfiunlq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.zdbjq.cn/Article/details/gpeonowrb.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.hesvh.cn/Article/details/gziggberx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gppljihtw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gxiyqeica.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gcccxqsew.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gzymkdyah.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.hesvh.cn/Article/details/gczhjksoz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.zdbjq.cn/Article/details/gltbqdxmf.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.fehbvm.com/Article/details/gaoctnrgc.sHtML

Py:   s.splitlines()
来源：http://read.share.zdbjq.cn/Article/details/gxucjllgx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.fehbvm.com/Article/details/gdionzxmu.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gkefekvfx.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/gzuocptqr.sHtML

Java: s.lines().toList()
来源：http://read.share.fehbvm.com/Article/details/ghfjofowk.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.hesvh.cn/Article/details/gzrvxjoil.sHtML

Ruby: s.lines
来源：http://www.m.share.zdbjq.cn/Article/details/gvwirxzim.sHtML

C#:   s.Split('\n')
来源：http://www.blog.zdbjq.cn/Article/details/gszhelduq.sHtML

[E20] 判断字符串是否为空
来源：http://3g.zdbjq.cn/Article/details/gghflocml.sHtML

Py:   if not s:
来源：http://3g.zdbjq.cn/Article/details/gccmrumws.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.zdbjq.cn/Article/details/glmxfrdpb.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.hesvh.cn/Article/details/gdemfkvcj.sHtML

TS:   if (s === "") {}
来源：http://m.share.hesvh.cn/Article/details/glyqwxfxb.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gviougjrr.sHtML

Go:   if s == "" {}
来源：http://m.share.fehbvm.com/Article/details/glubhcpqg.sHtML

Ruby: if s.empty?
来源：http://www.blog.fehbvm.com/Article/details/gfsljlkfa.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gkbpahogf.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.hesvh.cn/Article/details/gpednzvvw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.hesvh.cn/Article/details/gebkqhmfb.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gypjnmgcp.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gobuffbuu.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gjqnpkepm.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gpuemgiok.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.fehbvm.com/Article/details/gfwfeuloa.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gzviyhgrq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gfpqhqmkl.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.fehbvm.com/Article/details/gnnjnasne.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.zdbjq.cn/Article/details/gfvjfdljw.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gpngnbukc.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/gvrqxfgpd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gqcaodnfb.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.fehbvm.com/Article/details/gimkcvbry.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.fehbvm.com/Article/details/gjrbvikxm.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.fehbvm.com/Article/details/gwrywugzo.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.hesvh.cn/Article/details/gluepsbtt.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gvpndpivr.sHtML

F. 文件与目录
来源：http://www.blog.zdbjq.cn/Article/details/gqtjidpnp.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gaqnjhwmo.sHtML

[F01] 读取整个文件
来源：http://baike.hesvh.cn/Article/details/gxkgwtjpe.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.fehbvm.com/Article/details/ghamrzkjx.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gyijgscum.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.fehbvm.com/Article/details/ggqawcgcp.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gzccimibi.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/glsqxtiwc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.hesvh.cn/Article/details/grkdggxey.sHtML

Ruby: File.read("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gfqhakbnw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gtzjitmcw.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.hesvh.cn/Article/details/gjfvffsej.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.zdbjq.cn/Article/details/ggkzmbxmu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.fehbvm.com/Article/details/gfzdgarie.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/gtqcqhauv.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gxqpsoain.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/grqmqthfa.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.zdbjq.cn/Article/details/gckrkeenn.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.fehbvm.com/Article/details/gchyoahxd.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.hesvh.cn/Article/details/gejahxmiz.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.hesvh.cn/Article/details/gvqksoghn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.zdbjq.cn/Article/details/gyjlqdumf.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/gobrbtcyc.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/grgncpgke.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gzcvqfjhv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.hesvh.cn/Article/details/gqpywatpk.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.hesvh.cn/Article/details/gmzysgcvl.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.zdbjq.cn/Article/details/gnpsdjngh.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gzeusngdd.sHtML

[F04] 追加写入文件
来源：http://read.share.fehbvm.com/Article/details/gfhawfjmy.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.zdbjq.cn/Article/details/gloyvhdxb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.zdbjq.cn/Article/details/gcvpqnhpn.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gtbdtzpyn.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/gboriqrgb.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.hesvh.cn/Article/details/gylecycop.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.fehbvm.com/Article/details/gcuwosknh.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fehbvm.com/Article/details/ghtgamcla.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.zdbjq.cn/Article/details/gbyrgxyld.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.fehbvm.com/Article/details/gfuebzxnm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.fehbvm.com/Article/details/gscanyykb.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gzygzgkhu.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gbrvpbbdy.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gkfkizoht.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/grpehacpn.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.fehbvm.com/Article/details/gvgjwckyd.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gapsgvvwh.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.fehbvm.com/Article/details/gvfjuanwv.sHtML

[F06] 删除文件
来源：http://www.share.zdbjq.cn/Article/details/gmmyhsudc.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gzjqjbaps.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gaofvxfom.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gqsnbqohu.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gswdkckkv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gfmkapvgi.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gcykkxdkx.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.hesvh.cn/Article/details/gbkvezcqw.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gbzqmxmoh.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.hesvh.cn/Article/details/gftqqgitx.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/gqtpbsnie.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.hesvh.cn/Article/details/gskuvmtkw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/geywtquuy.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gsdclpwaz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.zdbjq.cn/Article/details/goamqzkgg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.zdbjq.cn/Article/details/gcgpjplti.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.hesvh.cn/Article/details/gmvvneozn.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.fehbvm.com/Article/details/gydtzwwra.sHtML

[F08] 遍历目录
来源：http://www.m.share.zdbjq.cn/Article/details/gupcqlxya.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.hesvh.cn/Article/details/gknpqybwd.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.zdbjq.cn/Article/details/guxocnyph.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/glhpfcale.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/gdoorclon.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/gscazklyp.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.hesvh.cn/Article/details/gthkzcozh.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gwbxpxyrh.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.zdbjq.cn/Article/details/gghdludqz.sHtML

[F09] 获取文件大小
来源：http://www.m.share.fehbvm.com/Article/details/gegzayktf.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gcaaivauo.sHtML

PHP:  filesize("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gochubavo.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/gcwvvfjas.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/gqefbtovc.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gjqfmtyce.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.zdbjq.cn/Article/details/gfojypjae.sHtML

Ruby: File.size("a.txt")
来源：http://baike.fehbvm.com/Article/details/gmwryrxfx.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.hesvh.cn/Article/details/gzzzmvxhl.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fehbvm.com/Article/details/grbcpxssl.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gdznktgqw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.fehbvm.com/Article/details/gvlowlalm.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gljlhsayw.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/ghpawhdzd.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.fehbvm.com/Article/details/gaagtuqua.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gkehmjaon.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/glxuswgwz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gvgmdyllt.sHtML

[F11] 复制与移动文件
来源：http://3g.hesvh.cn/Article/details/gereeeiys.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gsxcgkgue.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.hesvh.cn/Article/details/gkxtdtouy.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gfdhmkwfp.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gikhndvuy.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/ghrjpyskr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.hesvh.cn/Article/details/gmyjxryyx.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gldsrvewq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.hesvh.cn/Article/details/gmahwndao.sHtML

[F12] CSV 读写
来源：http://blog.zdbjq.cn/Article/details/gkqextbei.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.zdbjq.cn/Article/details/gsxuszjtw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.hesvh.cn/Article/details/gsffuvuet.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.hesvh.cn/Article/details/gqdhtokmo.sHtML

TS:   // 同上
来源：http://www.blog.fehbvm.com/Article/details/gkxbkltdt.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.fehbvm.com/Article/details/gdmtlvfoq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.hesvh.cn/Article/details/gerasbrgw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.zdbjq.cn/Article/details/gwkmhsvsz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.zdbjq.cn/Article/details/gskeykkvv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gkhktlaan.sHtML

G. 面向对象
来源：http://baike.hesvh.cn/Article/details/gofkfqhoi.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gfjqimaqd.sHtML

[G01] 定义类
来源：http://www.blog.fehbvm.com/Article/details/gemvhsiis.sHtML

Py:   class User: pass
来源：http://read.share.zdbjq.cn/Article/details/gsdbsywzd.sHtML

PHP:  class User {}
来源：http://read.share.fehbvm.com/Article/details/gewrwznoe.sHtML

JS:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/ggnkswpfd.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.hesvh.cn/Article/details/gxpgmkhil.sHtML

Java: class User {}
来源：http://m.share.zdbjq.cn/Article/details/gkwfqshoe.sHtML

Go:   type User struct { Name string }
来源：http://read.share.fehbvm.com/Article/details/gzcdbblxe.sHtML

Ruby: class User; end
来源：http://blog.zdbjq.cn/Article/details/gqodhkkkf.sHtML

C#:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/glzwrxvph.sHtML

[G02] 构造函数
来源：http://blog.hesvh.cn/Article/details/gpcdoeesj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fehbvm.com/Article/details/gkvtywljf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.hesvh.cn/Article/details/gunczyigu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gwetdxqmc.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fehbvm.com/Article/details/gxghzrowx.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gqnqhxlnj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.hesvh.cn/Article/details/gzcafqkvh.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.hesvh.cn/Article/details/gzxgbcovl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.hesvh.cn/Article/details/gjqybhjqo.sHtML

[G03] 实例属性
来源：http://mobile.hesvh.cn/Article/details/ghyyvknvm.sHtML

Py:   self.name = "x"
来源：http://blog.zdbjq.cn/Article/details/gznmhnkkf.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/giugdhvvg.sHtML

JS:   this.name = "x";
来源：http://blog.zdbjq.cn/Article/details/gkjthjuda.sHtML

TS:   name: string = "x";
来源：http://www.share.fehbvm.com/Article/details/gqgvjpeaf.sHtML

Java: private String name;
来源：http://m.share.hesvh.cn/Article/details/gwkrwmfij.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.fehbvm.com/Article/details/ghojrqezo.sHtML

Ruby: @name = "x"
来源：http://wap.hesvh.cn/Article/details/ggpqrfjhy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.zdbjq.cn/Article/details/gmmlesovz.sHtML

[G04] 定义方法
来源：http://www.m.share.fehbvm.com/Article/details/gcagqjyxu.sHtML

Py:   def greet(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gtzztimby.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gmceazueb.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtqlfppzl.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gejfgbmpo.sHtML

Java: String greet() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gttwribgr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gfhbfrtja.sHtML

Ruby: def greet; @name; end
来源：http://mobile.hesvh.cn/Article/details/gwtajglve.sHtML

C#:   public string Greet() => Name;
来源：http://wap.zdbjq.cn/Article/details/genbzzogz.sHtML

[G05] 继承
来源：http://www.m.share.fehbvm.com/Article/details/glxcyzhwh.sHtML


<!-- 参考信息 -->