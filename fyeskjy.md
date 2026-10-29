代发 wailian999

[E06] 替换子串
来源：http://mobile.hesvh.cn/Article/details/gwhexpbrk.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gwnvntlcf.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.hesvh.cn/Article/details/gcznboaca.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gemnzdozm.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gkqnifspg.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gbttoslpl.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gofwsnwyg.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gmdwjylox.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gzxlswcsq.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.zdbjq.cn/Article/details/gajgbxtoz.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.hesvh.cn/Article/details/grmkeytuf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.hesvh.cn/Article/details/gnyauosjz.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.zdbjq.cn/Article/details/gqzxjeqto.sHtML

TS:   s.split(",")
来源：http://baike.hesvh.cn/Article/details/gwbwnsing.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.zdbjq.cn/Article/details/getrwrifv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.hesvh.cn/Article/details/gwfnvdklu.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.fehbvm.com/Article/details/glosbulvq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.hesvh.cn/Article/details/gjneeeqcx.sHtML

[E08] 数组按分隔符合并
来源：http://blog.fehbvm.com/Article/details/gafonvgyz.sHtML

Py:   ",".join(items)
来源：http://www.m.share.fehbvm.com/Article/details/goevgmhif.sHtML

PHP:  implode(",", $items);
来源：http://3g.hesvh.cn/Article/details/gyyprufbh.sHtML

JS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gmxpjxxyp.sHtML

TS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gzfrfzvyg.sHtML

Java: String.join(",", items)
来源：http://wap.hesvh.cn/Article/details/gpohkihas.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.fehbvm.com/Article/details/gyruthgtt.sHtML

Ruby: items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gawbvziwl.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/gnkcfcdes.sHtML

[E09] 去除所有空白字符
来源：http://mobile.fehbvm.com/Article/details/gzqnhajwz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.fehbvm.com/Article/details/gutdcfmbg.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.hesvh.cn/Article/details/gwbdamfsx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/gwysjuwxl.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gjxtsgpwt.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.fehbvm.com/Article/details/ggyuoojje.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.hesvh.cn/Article/details/gomwdemss.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.fehbvm.com/Article/details/gmxxovkbm.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.fehbvm.com/Article/details/gnzwpvyaa.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.fehbvm.com/Article/details/gkvtduszu.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gejncwjgh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.hesvh.cn/Article/details/gvaoynndb.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/godnqyjai.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gvrwuthhm.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/ggsfxqpfl.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/ghqcdhadm.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gpgzfsamv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.fehbvm.com/Article/details/gjjdwuiaf.sHtML

[E11] 反转字符串
来源：http://wap.fehbvm.com/Article/details/gfgveeghi.sHtML

Py:   s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gfxcirrpx.sHtML

PHP:  strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gkhznfqpo.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gxcwdvqzq.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gbegbbvly.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.fehbvm.com/Article/details/gozeqrwag.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.fehbvm.com/Article/details/gjnkdtxhn.sHtML

Ruby: s.reverse
来源：http://wap.fehbvm.com/Article/details/gwahhupzh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gjrzwnplw.sHtML

[E12] 统计某字符出现次数
来源：http://3g.zdbjq.cn/Article/details/gwtetfvbh.sHtML

Py:   s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gkdlxkjtg.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.hesvh.cn/Article/details/gxfyzkimn.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gaovbilzq.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gpvwibnue.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.zdbjq.cn/Article/details/gyecowfme.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.zdbjq.cn/Article/details/gqrhijlny.sHtML

Ruby: s.count("a")
来源：http://m.share.hesvh.cn/Article/details/glesgqvzz.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.hesvh.cn/Article/details/ggjpaixoj.sHtML

[E13] 逐字符遍历
来源：http://www.blog.zdbjq.cn/Article/details/gnowyntzp.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.hesvh.cn/Article/details/gtuilmxcr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.zdbjq.cn/Article/details/gcebrnixk.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gpqgzeogw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gwdbwwhwm.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.hesvh.cn/Article/details/gfbrilljt.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gzenwoaqe.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.zdbjq.cn/Article/details/gujxhyshy.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.fehbvm.com/Article/details/gvogmsnam.sHtML

[E14] URL 编码与 Base64
来源：http://baike.fehbvm.com/Article/details/gkhmzftev.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fehbvm.com/Article/details/ghewprris.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.fehbvm.com/Article/details/gmfrikjas.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.fehbvm.com/Article/details/giykfhqtb.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gjbqxsovm.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.fehbvm.com/Article/details/gzldxyazq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.fehbvm.com/Article/details/ghshkobte.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.hesvh.cn/Article/details/gaptfkuyw.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.hesvh.cn/Article/details/gtupfvhyf.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.fehbvm.com/Article/details/goojuatrp.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fehbvm.com/Article/details/glvrdgfcy.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.fehbvm.com/Article/details/ghzmbfcrd.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.zdbjq.cn/Article/details/gbguemusp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.fehbvm.com/Article/details/gatkbaymn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.fehbvm.com/Article/details/gpazjvvra.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.hesvh.cn/Article/details/gttlqmcqa.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.hesvh.cn/Article/details/gwupcuhlv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gltmxgmnu.sHtML

[E16] 数字千分位
来源：http://m.share.hesvh.cn/Article/details/gpxubrnpx.sHtML

Py:   f"{1234567:,}"
来源：http://blog.fehbvm.com/Article/details/gyahtjtss.sHtML

PHP:  number_format(1234567);
来源：http://m.share.fehbvm.com/Article/details/gwqkmdhku.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/glcmpqepr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gbpafcikv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gkavlsrgo.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.hesvh.cn/Article/details/gxgxlinre.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.zdbjq.cn/Article/details/gkqorsenp.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.hesvh.cn/Article/details/gvzywsgsn.sHtML

[E17] 首字母大写
来源：http://3g.hesvh.cn/Article/details/ghdxloxvf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.fehbvm.com/Article/details/gktdlnnnd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.fehbvm.com/Article/details/gskwpjsed.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/gvplfegzw.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/gjrlamzsq.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.zdbjq.cn/Article/details/gkfiaeszb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.hesvh.cn/Article/details/gmntfkfcz.sHtML

Ruby: s.capitalize
来源：http://m.share.hesvh.cn/Article/details/guzaaikcc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.zdbjq.cn/Article/details/gpzsrrxom.sHtML

[E18] 模板占位符替换
来源：http://www.share.fehbvm.com/Article/details/gpmbcffog.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.zdbjq.cn/Article/details/glacurrvy.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.hesvh.cn/Article/details/gnagxyeyv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/ghagorxag.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gtizpcrii.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.hesvh.cn/Article/details/geoexvlrb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gpuyyifzn.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.fehbvm.com/Article/details/gvauyrjoo.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.zdbjq.cn/Article/details/gdpbpdosu.sHtML

[E19] 多行文本按行拆分
来源：http://blog.zdbjq.cn/Article/details/gzrutjoea.sHtML

Py:   s.splitlines()
来源：http://baike.fehbvm.com/Article/details/gusktaetn.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.fehbvm.com/Article/details/gsevhscez.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gtlsuyrou.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/gkddxclfr.sHtML

Java: s.lines().toList()
来源：http://www.blog.zdbjq.cn/Article/details/gfdkruwkb.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.zdbjq.cn/Article/details/gkhknxhfn.sHtML

Ruby: s.lines
来源：http://baike.fehbvm.com/Article/details/ghgpssxeu.sHtML

C#:   s.Split('\n')
来源：http://blog.fehbvm.com/Article/details/geadiykov.sHtML

[E20] 判断字符串是否为空
来源：http://wap.hesvh.cn/Article/details/gfsbctjrp.sHtML

Py:   if not s:
来源：http://www.m.share.zdbjq.cn/Article/details/glrnazmzd.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.zdbjq.cn/Article/details/gyymmvblp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.hesvh.cn/Article/details/gmrvsiiyk.sHtML

TS:   if (s === "") {}
来源：http://3g.hesvh.cn/Article/details/gtufsmdnd.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/ggcqspuyw.sHtML

Go:   if s == "" {}
来源：http://3g.hesvh.cn/Article/details/glsouqgjd.sHtML

Ruby: if s.empty?
来源：http://read.share.zdbjq.cn/Article/details/gubmhrkkp.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.zdbjq.cn/Article/details/gaeuihqnj.sHtML

[E21] 超长截断加省略号
来源：http://read.share.fehbvm.com/Article/details/ghqbrcnnq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.hesvh.cn/Article/details/gnepihdeu.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gjnhhzvjj.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gkkwqovlw.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/giclvsyny.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gvwlhwihl.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.zdbjq.cn/Article/details/gbrsjdzmp.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gpvfaoegg.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gauwowage.sHtML

[E22] 字节长度与字符长度
来源：http://wap.fehbvm.com/Article/details/gabqhmmxj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.hesvh.cn/Article/details/gruniurqd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/giraqrrwe.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/gmnjlzqee.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/glxnnicfn.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.zdbjq.cn/Article/details/gxqovavuv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.fehbvm.com/Article/details/gqtytjzjx.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fehbvm.com/Article/details/gazsmlqhh.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.fehbvm.com/Article/details/grtrxswtu.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gymzhxgyr.sHtML

F. 文件与目录
来源：http://www.blog.zdbjq.cn/Article/details/gvgwdkedi.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gsjfwkjgk.sHtML

[F01] 读取整个文件
来源：http://blog.hesvh.cn/Article/details/gmhrqfozz.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.hesvh.cn/Article/details/gvogqaqay.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.fehbvm.com/Article/details/gainysxyn.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.fehbvm.com/Article/details/gsjmicadx.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gwwjmvhoe.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/glvpppzyj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.fehbvm.com/Article/details/gfbjcwvfn.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gwkeioecz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.hesvh.cn/Article/details/gvlawlcpp.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.zdbjq.cn/Article/details/guwcggsup.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.zdbjq.cn/Article/details/gtptvuggs.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.hesvh.cn/Article/details/gktslsiif.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gbrchpdmp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gnxxgzsda.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gghqqggus.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.hesvh.cn/Article/details/gduqfzlng.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.fehbvm.com/Article/details/gtqcvuoei.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.zdbjq.cn/Article/details/gdfiydjxi.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.fehbvm.com/Article/details/gnqaxntfa.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.zdbjq.cn/Article/details/gwcwzjpdt.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/gplajbssf.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gmxkdgigr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gbznphjql.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.fehbvm.com/Article/details/gtgeqzhdg.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.fehbvm.com/Article/details/gktcjxzqw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.zdbjq.cn/Article/details/gqbvzqndv.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gjonmwxyo.sHtML

[F04] 追加写入文件
来源：http://www.share.hesvh.cn/Article/details/gviyiwysc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.zdbjq.cn/Article/details/gfjttzjak.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.zdbjq.cn/Article/details/gslremmgp.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/gbvqbtean.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gjxurqcsl.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.zdbjq.cn/Article/details/gnuarhjjp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gksiqkrja.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.fehbvm.com/Article/details/gxxmpwihp.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fehbvm.com/Article/details/gpfohqsxi.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.zdbjq.cn/Article/details/gqomfevke.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.zdbjq.cn/Article/details/gdmscxgxc.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/ggwmnblbn.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gnlelpvou.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gjavovncv.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/grxoojhlz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.hesvh.cn/Article/details/gpvfntizh.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gfsktxdxo.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.hesvh.cn/Article/details/gclmyotyk.sHtML

[F06] 删除文件
来源：http://wap.fehbvm.com/Article/details/gtqgxgdxu.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/ghwfbgbjn.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fehbvm.com/Article/details/gzqfduflo.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gzbxyruci.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ggdryiasz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gplqvnlum.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gryvwiltr.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gwtfgjrmt.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gvhtaldjb.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.hesvh.cn/Article/details/gizqsytne.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/gotceaysw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.fehbvm.com/Article/details/gbiqefuyk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gbnbkhwun.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/gbmgbevfe.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.fehbvm.com/Article/details/gwruvnkiv.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.hesvh.cn/Article/details/geqqcyzdw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.zdbjq.cn/Article/details/gtdxbghne.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.hesvh.cn/Article/details/gyrxoqyoz.sHtML

[F08] 遍历目录
来源：http://read.share.hesvh.cn/Article/details/gefwuzjbf.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.fehbvm.com/Article/details/ggntvyvwb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.zdbjq.cn/Article/details/gynsnzxnu.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gjlgrnwdi.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gynqxspch.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gdivkcugy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gzgjaecqh.sHtML

Ruby: Dir.children("dir")
来源：http://blog.zdbjq.cn/Article/details/gutqcqful.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.zdbjq.cn/Article/details/gtygwglgj.sHtML

[F09] 获取文件大小
来源：http://3g.zdbjq.cn/Article/details/gitmckuay.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gehnchtyc.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/guuhccbvu.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gvwhzxeev.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/gafmbfckp.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gahktlvjo.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.fehbvm.com/Article/details/gkxasspqh.sHtML

Ruby: File.size("a.txt")
来源：http://baike.hesvh.cn/Article/details/givttdsqe.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.hesvh.cn/Article/details/gpkjfuteb.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.hesvh.cn/Article/details/gliydtkuu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gzzbhlesq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.zdbjq.cn/Article/details/grgjruqta.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/ggnfaaivg.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gjkvgzfpv.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.fehbvm.com/Article/details/gmmfgvksn.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/geoyxpbdw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gggmbmdkz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gzaedcfzx.sHtML

[F11] 复制与移动文件
来源：http://www.share.hesvh.cn/Article/details/gdgowmnls.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gnjywwufd.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.hesvh.cn/Article/details/gnwaaakkm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gwtxkjkvd.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gtrjgqpnc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.hesvh.cn/Article/details/geqodhbeo.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.hesvh.cn/Article/details/gmelmikba.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gkrtmmfbt.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.hesvh.cn/Article/details/guiypygwn.sHtML

[F12] CSV 读写
来源：http://blog.zdbjq.cn/Article/details/gjlzwviot.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.hesvh.cn/Article/details/gnuoponyy.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.fehbvm.com/Article/details/gawsgjfop.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.fehbvm.com/Article/details/gycpzbagy.sHtML

TS:   // 同上
来源：http://baike.fehbvm.com/Article/details/gzafekbmp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.zdbjq.cn/Article/details/gfzzasldt.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.zdbjq.cn/Article/details/gjaziikvu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.zdbjq.cn/Article/details/gjxwdmmoz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.fehbvm.com/Article/details/gczqgrswh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gphnmtkeb.sHtML

G. 面向对象
来源：http://m.share.fehbvm.com/Article/details/gpsbtwjjk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gqvgmzhwr.sHtML

[G01] 定义类
来源：http://mobile.fehbvm.com/Article/details/gpdtaraor.sHtML

Py:   class User: pass
来源：http://wap.zdbjq.cn/Article/details/gojfcnbli.sHtML

PHP:  class User {}
来源：http://wap.zdbjq.cn/Article/details/gerkrgtgi.sHtML

JS:   class User {}
来源：http://wap.fehbvm.com/Article/details/gfciztpsy.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.hesvh.cn/Article/details/gdcersinf.sHtML

Java: class User {}
来源：http://m.share.hesvh.cn/Article/details/ghmftkqmi.sHtML

Go:   type User struct { Name string }
来源：http://blog.hesvh.cn/Article/details/gdhfvogfy.sHtML

Ruby: class User; end
来源：http://www.blog.zdbjq.cn/Article/details/guaatuavb.sHtML

C#:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gqnrxbiyx.sHtML

[G02] 构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gbmqhncfd.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.hesvh.cn/Article/details/ginbfeiyb.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.zdbjq.cn/Article/details/gbukmoorc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gigntryvv.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/gdqgohnbq.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gevydaslu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fehbvm.com/Article/details/gefddtult.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.hesvh.cn/Article/details/gfkcnkovx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/guuvurqyj.sHtML

[G03] 实例属性
来源：http://wap.fehbvm.com/Article/details/gawwhyroy.sHtML

Py:   self.name = "x"
来源：http://mobile.fehbvm.com/Article/details/ggfiuktdj.sHtML

PHP:  public string $name = "x";
来源：http://3g.fehbvm.com/Article/details/guijsmkvz.sHtML

JS:   this.name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gdzagnfqt.sHtML

TS:   name: string = "x";
来源：http://read.share.hesvh.cn/Article/details/gufkcjtki.sHtML

Java: private String name;
来源：http://www.share.zdbjq.cn/Article/details/gxibefmoc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.zdbjq.cn/Article/details/gfxypydre.sHtML

Ruby: @name = "x"
来源：http://mobile.fehbvm.com/Article/details/gulfcifoe.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.hesvh.cn/Article/details/gahpsaxbq.sHtML

[G04] 定义方法
来源：http://www.m.share.hesvh.cn/Article/details/ggjgznrry.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/ghrnujcgm.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gopqrcvet.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gdzxtfvta.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gldmvmicm.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gkqqytdjd.sHtML


<!-- 参考信息 -->