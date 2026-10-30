代发 wailian999

[E06] 替换子串
来源：http://m.share.hesvh.cn/Article/details/gkbuefkxo.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/gseupcdln.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.fehbvm.com/Article/details/gknnnrdse.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gvejgikah.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gtamzgmvs.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gmxhdxmog.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/gtftqllgi.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gczdzrwgb.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gxhcqipco.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gbaunbhjs.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.zdbjq.cn/Article/details/gpjlkgaqw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.hesvh.cn/Article/details/gatfhwfcq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.fehbvm.com/Article/details/gqwidgmiz.sHtML

TS:   s.split(",")
来源：http://wap.fehbvm.com/Article/details/gkiaagjfo.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.hesvh.cn/Article/details/gelcvtine.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.zdbjq.cn/Article/details/gqafgfwge.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.fehbvm.com/Article/details/gmvrccuch.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.hesvh.cn/Article/details/gbkwsqfif.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.zdbjq.cn/Article/details/gshqpvcih.sHtML

Py:   ",".join(items)
来源：http://baike.zdbjq.cn/Article/details/gvwymxqua.sHtML

PHP:  implode(",", $items);
来源：http://mobile.hesvh.cn/Article/details/gjerondqr.sHtML

JS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gtwaepnzo.sHtML

TS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gkybdamcv.sHtML

Java: String.join(",", items)
来源：http://mobile.fehbvm.com/Article/details/gyrmbwagv.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.hesvh.cn/Article/details/gkhcnbqry.sHtML

Ruby: items.join(",")
来源：http://baike.hesvh.cn/Article/details/grwztyhfe.sHtML

C#:   string.Join(",", items)
来源：http://mobile.fehbvm.com/Article/details/gueyladjp.sHtML

[E09] 去除所有空白字符
来源：http://3g.zdbjq.cn/Article/details/gwizmdkig.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.hesvh.cn/Article/details/gnztabdrk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.fehbvm.com/Article/details/gmjddxchy.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/guiiqxikn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/gfrggjsnk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/gdxhtwjun.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.zdbjq.cn/Article/details/glkphpavc.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.zdbjq.cn/Article/details/gatfiivvl.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.zdbjq.cn/Article/details/gsssoosmy.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.zdbjq.cn/Article/details/gpezuzwff.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.hesvh.cn/Article/details/gsjgsplft.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.fehbvm.com/Article/details/gbhvvinpi.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gsorpozcw.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gwoqasils.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gwkuxxpur.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gkbloubtc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gcpqfcrue.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.zdbjq.cn/Article/details/glpaiwwel.sHtML

[E11] 反转字符串
来源：http://3g.hesvh.cn/Article/details/gtmrhzcxh.sHtML

Py:   s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gkukjfcgx.sHtML

PHP:  strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gldzvcopa.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/guzcrvfgm.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gfzardmbs.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.hesvh.cn/Article/details/gkmhhlois.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.hesvh.cn/Article/details/gxxlszylr.sHtML

Ruby: s.reverse
来源：http://mobile.hesvh.cn/Article/details/gdhjjekod.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gcqmhalim.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.hesvh.cn/Article/details/gnfgswsvq.sHtML

Py:   s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gjvvrosoi.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.zdbjq.cn/Article/details/gowwimong.sHtML

JS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/gffkrvupq.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/gjxipjlhu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.fehbvm.com/Article/details/gdssxpzkk.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.fehbvm.com/Article/details/gkbbwfcgv.sHtML

Ruby: s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/gpdgvucfh.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.zdbjq.cn/Article/details/gxfczkqwa.sHtML

[E13] 逐字符遍历
来源：http://www.share.zdbjq.cn/Article/details/gylqfsxsq.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.hesvh.cn/Article/details/gqacnobuv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.zdbjq.cn/Article/details/gpruqvkmh.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gfbhkdfza.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/gcwxztujr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gtpjzvidj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.fehbvm.com/Article/details/ghdyryijv.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.fehbvm.com/Article/details/grnexhhsh.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.fehbvm.com/Article/details/gwzgpcmtj.sHtML

[E14] URL 编码与 Base64
来源：http://wap.fehbvm.com/Article/details/gduwiswkb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.hesvh.cn/Article/details/gakyuhpfh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.zdbjq.cn/Article/details/gekjnbcoa.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.zdbjq.cn/Article/details/gmdtcgnkz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.fehbvm.com/Article/details/gmcjgmyai.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gpcinppre.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.fehbvm.com/Article/details/geuamfxmz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.hesvh.cn/Article/details/griiicinx.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gezynradb.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.hesvh.cn/Article/details/gozxqlqjp.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fehbvm.com/Article/details/gqtclzylw.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fehbvm.com/Article/details/gnztxnwjw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.zdbjq.cn/Article/details/gntbqzxel.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.hesvh.cn/Article/details/gxxgltckr.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.hesvh.cn/Article/details/gkaovrryo.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.fehbvm.com/Article/details/gugqidkjq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.zdbjq.cn/Article/details/gspxyqbil.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.hesvh.cn/Article/details/gvrytsfbp.sHtML

[E16] 数字千分位
来源：http://baike.fehbvm.com/Article/details/ggrdahecz.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.hesvh.cn/Article/details/gfayapslo.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.fehbvm.com/Article/details/gunsuerxi.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gbixhngdy.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/gtfaiyyxf.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gwhtwwxyj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.fehbvm.com/Article/details/gfqezmhyc.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.fehbvm.com/Article/details/gtvnmebgu.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.fehbvm.com/Article/details/geczziolj.sHtML

[E17] 首字母大写
来源：http://mobile.zdbjq.cn/Article/details/geqlezvuv.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.zdbjq.cn/Article/details/gdsaiolvv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.hesvh.cn/Article/details/gfrqrpnsb.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gosmaukky.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gcdqlhdjh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.hesvh.cn/Article/details/gqfnjjcxz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.fehbvm.com/Article/details/gjvvinxxr.sHtML

Ruby: s.capitalize
来源：http://www.share.zdbjq.cn/Article/details/gsfgnvpyn.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.zdbjq.cn/Article/details/gpsawyktl.sHtML

[E18] 模板占位符替换
来源：http://m.share.fehbvm.com/Article/details/gnoaxjxay.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.zdbjq.cn/Article/details/gmtsxurxr.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.zdbjq.cn/Article/details/glxkfjghb.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/glyibildn.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gtcdvrhih.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.hesvh.cn/Article/details/ggoxzbksd.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.zdbjq.cn/Article/details/guivjyfrp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.fehbvm.com/Article/details/gxzxauxsk.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.hesvh.cn/Article/details/gfviozwgk.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.hesvh.cn/Article/details/girrlujaq.sHtML

Py:   s.splitlines()
来源：http://blog.fehbvm.com/Article/details/gpdketuei.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.zdbjq.cn/Article/details/gxsbxjadr.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/goxlbboqw.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/gbthipqbp.sHtML

Java: s.lines().toList()
来源：http://3g.hesvh.cn/Article/details/gdugzezhq.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.fehbvm.com/Article/details/gibwicqgl.sHtML

Ruby: s.lines
来源：http://wap.fehbvm.com/Article/details/ghavjiacl.sHtML

C#:   s.Split('\n')
来源：http://www.blog.fehbvm.com/Article/details/gdpfcdxzg.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fehbvm.com/Article/details/gupxoscfr.sHtML

Py:   if not s:
来源：http://wap.fehbvm.com/Article/details/guwfukfcw.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.zdbjq.cn/Article/details/gorhnxwis.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.zdbjq.cn/Article/details/gklknevgg.sHtML

TS:   if (s === "") {}
来源：http://mobile.fehbvm.com/Article/details/gwvqfbblq.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/ggiqcanht.sHtML

Go:   if s == "" {}
来源：http://www.share.fehbvm.com/Article/details/gnicoxoxi.sHtML

Ruby: if s.empty?
来源：http://www.m.share.hesvh.cn/Article/details/gyjgqhyyx.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.zdbjq.cn/Article/details/gkwrlcmyv.sHtML

[E21] 超长截断加省略号
来源：http://read.share.fehbvm.com/Article/details/gzeuyuxlf.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.zdbjq.cn/Article/details/gewzbnhki.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gigcivkup.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gzmqcjtwn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/grkxbrbkn.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gqoqnvhpx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.hesvh.cn/Article/details/gwgopfohq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gdodhfruy.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/glftoregd.sHtML

[E22] 字节长度与字符长度
来源：http://wap.hesvh.cn/Article/details/gsuhsvolk.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.fehbvm.com/Article/details/ghaajlbpi.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/guqwjbmdw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gcxfduijf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gvdgeflvl.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.fehbvm.com/Article/details/gpfsqfask.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.hesvh.cn/Article/details/gdlwcosro.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.fehbvm.com/Article/details/gvthszzbh.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.fehbvm.com/Article/details/gfzzjdhbp.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/grzorbzzs.sHtML

F. 文件与目录
来源：http://blog.hesvh.cn/Article/details/ggoaojadf.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gfofpkdxs.sHtML

[F01] 读取整个文件
来源：http://baike.hesvh.cn/Article/details/gneyiyrwm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.hesvh.cn/Article/details/gdksjchqe.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gyexoywdc.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.zdbjq.cn/Article/details/guclaieda.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gqlemafzu.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/geiyjswmc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.hesvh.cn/Article/details/gqmubkruq.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gxcqjqmat.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gdzrtufae.sHtML

[F02] 逐行读取文件
来源：http://3g.zdbjq.cn/Article/details/gbvnqnfvb.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.fehbvm.com/Article/details/gjmxruxpw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.hesvh.cn/Article/details/gefxskrxr.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/gmhshhjid.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/gjxszsput.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gdciidyps.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.hesvh.cn/Article/details/gyywvvnfx.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.hesvh.cn/Article/details/gldcujcyg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.zdbjq.cn/Article/details/ggmwwjavx.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.hesvh.cn/Article/details/gvqagckah.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.zdbjq.cn/Article/details/gffwycyap.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gutqawzcq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gwljggowh.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gunwqrxun.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gxzkaallc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.hesvh.cn/Article/details/gzqfiyfpz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.fehbvm.com/Article/details/guogoyvpu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gkploobno.sHtML

[F04] 追加写入文件
来源：http://mobile.fehbvm.com/Article/details/gorjfaodk.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.zdbjq.cn/Article/details/gcwxdcjhy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.zdbjq.cn/Article/details/ggrwwslry.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gvwrfuzao.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/gfardciuc.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.zdbjq.cn/Article/details/gmrifgvzq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/glupcrkem.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.zdbjq.cn/Article/details/gxybowjol.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.hesvh.cn/Article/details/gnnlrnkfk.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.fehbvm.com/Article/details/guuusdlav.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.zdbjq.cn/Article/details/ggtjfoezh.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gwjwgtecf.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gibciejeo.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gicmjsqnu.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gbuesvlhw.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.zdbjq.cn/Article/details/gxfgyjvmf.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fehbvm.com/Article/details/guqyptfne.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gcaqeigkp.sHtML

[F06] 删除文件
来源：http://www.blog.hesvh.cn/Article/details/gbonzxrbn.sHtML

Py:   os.remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/graxbyqcw.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gksylgzgr.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gmzbforqg.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gajtekhwx.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/guzkcoulz.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gyscnjfno.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.fehbvm.com/Article/details/gtclxqyme.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gbgvjttaf.sHtML

[F07] 创建目录（含多级）
来源：http://wap.hesvh.cn/Article/details/gtqmcbcpk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gzvuurdwd.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.hesvh.cn/Article/details/gxeaamtrw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gkanawete.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gcnghwrvq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.hesvh.cn/Article/details/ggukdasrc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.hesvh.cn/Article/details/guafhwham.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.fehbvm.com/Article/details/gopwczkqn.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.fehbvm.com/Article/details/gxzyhqfmh.sHtML

[F08] 遍历目录
来源：http://read.share.zdbjq.cn/Article/details/ggyutfvwr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.fehbvm.com/Article/details/gdnjekzhw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.hesvh.cn/Article/details/ggqlxwsdh.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/gtyauqfcp.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gktuyrkeu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/gsblabavp.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.fehbvm.com/Article/details/gvxonayhq.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gmxomsamn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gnnuurwzu.sHtML

[F09] 获取文件大小
来源：http://baike.fehbvm.com/Article/details/gslvveihq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gxrxqvuwz.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gdrydgocn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gyqedvrcy.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/glzttqseq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/guufruhuh.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.zdbjq.cn/Article/details/gocyutnoz.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gdijtfnva.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.zdbjq.cn/Article/details/gykribyuh.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.zdbjq.cn/Article/details/giveqmuma.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gppxpsjtg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gdpuhxjij.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gllrpyaou.sHtML

TS:   path.extname("a.txt")
来源：http://blog.hesvh.cn/Article/details/gzzhrwbqm.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.hesvh.cn/Article/details/gwpnbsuyn.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gtzjglbdd.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gdwmdkeym.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gowndsmfe.sHtML

[F11] 复制与移动文件
来源：http://read.share.hesvh.cn/Article/details/gdsvqlbwd.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gucxctosz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.zdbjq.cn/Article/details/gbbutwtfm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gzhocvpac.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gdvfrczxo.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gcbuftkpl.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fehbvm.com/Article/details/gtoxzvkfg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gfyybywqt.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.hesvh.cn/Article/details/gsrnkmvoz.sHtML

[F12] CSV 读写
来源：http://wap.zdbjq.cn/Article/details/gkewfnfsf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.zdbjq.cn/Article/details/gewmpbycw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.zdbjq.cn/Article/details/glcmgqeof.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.hesvh.cn/Article/details/gjfklqsvj.sHtML

TS:   // 同上
来源：http://wap.hesvh.cn/Article/details/grajjwnyy.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.hesvh.cn/Article/details/ghvxgyhek.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.fehbvm.com/Article/details/gbjfckton.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.hesvh.cn/Article/details/gpbofkpts.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fehbvm.com/Article/details/gmmblkdsa.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gnhhckaxx.sHtML

G. 面向对象
来源：http://www.share.zdbjq.cn/Article/details/gjgjhzgho.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gphfkzicf.sHtML

[G01] 定义类
来源：http://3g.fehbvm.com/Article/details/gkpsejccw.sHtML

Py:   class User: pass
来源：http://wap.fehbvm.com/Article/details/gbfkwawrx.sHtML

PHP:  class User {}
来源：http://3g.zdbjq.cn/Article/details/gwmavnkxb.sHtML

JS:   class User {}
来源：http://3g.fehbvm.com/Article/details/gzrdgmvdn.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.hesvh.cn/Article/details/gxqgtwsah.sHtML

Java: class User {}
来源：http://www.share.zdbjq.cn/Article/details/gklsyshmq.sHtML

Go:   type User struct { Name string }
来源：http://baike.fehbvm.com/Article/details/gajojpesu.sHtML

Ruby: class User; end
来源：http://mobile.fehbvm.com/Article/details/gvyuckjry.sHtML

C#:   class User {}
来源：http://baike.hesvh.cn/Article/details/gnmqivmag.sHtML

[G02] 构造函数
来源：http://www.share.zdbjq.cn/Article/details/gyaisskyd.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.hesvh.cn/Article/details/ggjgdqdch.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.zdbjq.cn/Article/details/ggqlnasvr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gyyvkthyn.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.zdbjq.cn/Article/details/grbmrqbsr.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gmiitmsgn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.fehbvm.com/Article/details/gojzgplal.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fehbvm.com/Article/details/ggvatwvlq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gvtrxwhvz.sHtML

[G03] 实例属性
来源：http://www.m.share.zdbjq.cn/Article/details/geflzqjnc.sHtML

Py:   self.name = "x"
来源：http://blog.fehbvm.com/Article/details/gknfajtjv.sHtML

PHP:  public string $name = "x";
来源：http://blog.fehbvm.com/Article/details/gpmqvmubt.sHtML

JS:   this.name = "x";
来源：http://3g.hesvh.cn/Article/details/glprbtrmx.sHtML

TS:   name: string = "x";
来源：http://m.share.zdbjq.cn/Article/details/gpsmpxcoa.sHtML

Java: private String name;
来源：http://wap.fehbvm.com/Article/details/gmeytjcye.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fehbvm.com/Article/details/gwtmqcdrh.sHtML

Ruby: @name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gxcxwwoky.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/ghgiddidz.sHtML

[G04] 定义方法
来源：http://blog.fehbvm.com/Article/details/gohalhuxr.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gvkrlqxzf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/ghuediwcm.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/giqpinjnr.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/grawebkho.sHtML

Java: String greet() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gabwaxxdk.sHtML


<!-- 参考信息 -->