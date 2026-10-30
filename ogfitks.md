代发 wailian999

[E06] 替换子串
来源：http://read.share.fehbvm.com/Article/details/gpwsclfms.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/gvqmtxtid.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.fehbvm.com/Article/details/guposlwfa.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gbmchrekx.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gzytkbmjq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gwmyddikk.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/ggodtdyov.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gmkzigreu.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fehbvm.com/Article/details/gemvccaaz.sHtML

[E07] 按分隔符拆分
来源：http://read.share.zdbjq.cn/Article/details/giqundjxi.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.hesvh.cn/Article/details/gcfiyzhap.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.zdbjq.cn/Article/details/ghkhhpjjb.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.hesvh.cn/Article/details/gjrecrwmd.sHtML

TS:   s.split(",")
来源：http://www.blog.fehbvm.com/Article/details/gkaqdldfu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.hesvh.cn/Article/details/gsnoixwya.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.fehbvm.com/Article/details/gnwhatfdf.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.zdbjq.cn/Article/details/gdswnzdrq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.zdbjq.cn/Article/details/gqwouvnap.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.fehbvm.com/Article/details/gtlufxfrt.sHtML

Py:   ",".join(items)
来源：http://mobile.hesvh.cn/Article/details/gmscgzzre.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.fehbvm.com/Article/details/gzdpuyjvd.sHtML

JS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/gsiynrogd.sHtML

TS:   items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gutdpnvie.sHtML

Java: String.join(",", items)
来源：http://blog.zdbjq.cn/Article/details/gvrwsbsuv.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.hesvh.cn/Article/details/ghawkdwus.sHtML

Ruby: items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gplsmwsnx.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/glaeftplp.sHtML

[E09] 去除所有空白字符
来源：http://baike.hesvh.cn/Article/details/gqzmvcsqb.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.hesvh.cn/Article/details/gnxwzosil.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gfizjpifp.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/gvccjjmbx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.fehbvm.com/Article/details/gkiqgfewi.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.hesvh.cn/Article/details/gmabqrrom.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.hesvh.cn/Article/details/gaqfvnjso.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.zdbjq.cn/Article/details/gshokjcpe.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/goivkbdes.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.hesvh.cn/Article/details/grxuiutdl.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/glannwkti.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.fehbvm.com/Article/details/gwzounjmj.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/godbmdvnr.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gwabwyhsn.sHtML

Java: String.format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gnhtreaxi.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gnmxtaytq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/glqhaynim.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.zdbjq.cn/Article/details/gzecvcdnt.sHtML

[E11] 反转字符串
来源：http://read.share.zdbjq.cn/Article/details/gihptpnwh.sHtML

Py:   s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gmforfckz.sHtML

PHP:  strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gkqanmvyb.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gmokrmnmb.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gwjqgmegt.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.hesvh.cn/Article/details/gfmdfkrsf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.hesvh.cn/Article/details/gnjeinfup.sHtML

Ruby: s.reverse
来源：http://wap.fehbvm.com/Article/details/gtodpdvry.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/gjrveqxhu.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.fehbvm.com/Article/details/gyafwbaun.sHtML

Py:   s.count("a")
来源：http://www.share.fehbvm.com/Article/details/ghsekgbrj.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.hesvh.cn/Article/details/gopbvomcs.sHtML

JS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/gojgkxcki.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/gpbhenoqr.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.fehbvm.com/Article/details/gonuzakut.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.fehbvm.com/Article/details/gjwujnaqb.sHtML

Ruby: s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gagemlsed.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.hesvh.cn/Article/details/glprxewql.sHtML

[E13] 逐字符遍历
来源：http://baike.hesvh.cn/Article/details/gdtyikvns.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.hesvh.cn/Article/details/gahbysyrd.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.zdbjq.cn/Article/details/gnkanaxkr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gbgawsayp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/ghzeldhdb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gepulncit.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.hesvh.cn/Article/details/gjprwdnzs.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.zdbjq.cn/Article/details/gsutqrnwh.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gaytqhavk.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.zdbjq.cn/Article/details/gcuahlrgy.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.zdbjq.cn/Article/details/gibhnvdsr.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.hesvh.cn/Article/details/grzsthzhs.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.fehbvm.com/Article/details/gkurwgmim.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.fehbvm.com/Article/details/gugavhkwp.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.zdbjq.cn/Article/details/gpqwgvpxt.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.fehbvm.com/Article/details/glkdedynj.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.zdbjq.cn/Article/details/goeqzgpbm.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.fehbvm.com/Article/details/gsaihygmj.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.fehbvm.com/Article/details/ghuxosywx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.fehbvm.com/Article/details/gkhkuwznm.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.hesvh.cn/Article/details/gekiludwe.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.fehbvm.com/Article/details/gjbyqfsfr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.fehbvm.com/Article/details/gwpnbyajz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.hesvh.cn/Article/details/gwzvkyjdf.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.hesvh.cn/Article/details/gatwgtaog.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.zdbjq.cn/Article/details/gizgexwgm.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.hesvh.cn/Article/details/gzzfkrptb.sHtML

[E16] 数字千分位
来源：http://read.share.fehbvm.com/Article/details/gkjckgexm.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.zdbjq.cn/Article/details/gzdbkyvqj.sHtML

PHP:  number_format(1234567);
来源：http://blog.zdbjq.cn/Article/details/gtwynuwve.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gsvblsjch.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/gecwhhyrw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/gppemkpvb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.fehbvm.com/Article/details/gkdroyzne.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.zdbjq.cn/Article/details/ggkkjfxjq.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.hesvh.cn/Article/details/gljcyjzdh.sHtML

[E17] 首字母大写
来源：http://www.m.share.fehbvm.com/Article/details/guzkmsovk.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.zdbjq.cn/Article/details/gottvxvqd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fehbvm.com/Article/details/gbfvpoayb.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gcniwffed.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gkpmzdtvh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.hesvh.cn/Article/details/gaaqqlzqq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.fehbvm.com/Article/details/gkejnrakb.sHtML

Ruby: s.capitalize
来源：http://baike.hesvh.cn/Article/details/gisffmkmt.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fehbvm.com/Article/details/gvxweryhl.sHtML

[E18] 模板占位符替换
来源：http://blog.fehbvm.com/Article/details/gaazkuxjk.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.fehbvm.com/Article/details/gmoehlgvd.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.hesvh.cn/Article/details/gzvwyspze.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gvnuzldbe.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gulakrauo.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gyybpgeta.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gmfwzqrzm.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.hesvh.cn/Article/details/gekujalnc.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.hesvh.cn/Article/details/gkadvgcjl.sHtML

[E19] 多行文本按行拆分
来源：http://wap.hesvh.cn/Article/details/gabaaiuze.sHtML

Py:   s.splitlines()
来源：http://read.share.fehbvm.com/Article/details/ggnbjpedq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gebequkyg.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/grzaslifu.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/gwpxnibof.sHtML

Java: s.lines().toList()
来源：http://blog.fehbvm.com/Article/details/goywryiuc.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.hesvh.cn/Article/details/gmlcmsowd.sHtML

Ruby: s.lines
来源：http://read.share.fehbvm.com/Article/details/gguuflahr.sHtML

C#:   s.Split('\n')
来源：http://m.share.fehbvm.com/Article/details/grhondcuq.sHtML

[E20] 判断字符串是否为空
来源：http://baike.zdbjq.cn/Article/details/gktaxywlp.sHtML

Py:   if not s:
来源：http://baike.zdbjq.cn/Article/details/geusavnex.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fehbvm.com/Article/details/gnnpaqyae.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.zdbjq.cn/Article/details/gghfmopvw.sHtML

TS:   if (s === "") {}
来源：http://www.share.fehbvm.com/Article/details/gpxtisbal.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gxmqkazoo.sHtML

Go:   if s == "" {}
来源：http://www.m.share.zdbjq.cn/Article/details/gaxekwrne.sHtML

Ruby: if s.empty?
来源：http://3g.fehbvm.com/Article/details/ggkrcbdiu.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.fehbvm.com/Article/details/glrolrsyu.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fehbvm.com/Article/details/gtcergcnw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.hesvh.cn/Article/details/gkaazzzys.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/glceydqnr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gnvhkrzgn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gmeolncep.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gntwpijgf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.fehbvm.com/Article/details/giaumjnqz.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gxkypmaxy.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/guobywqbq.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.hesvh.cn/Article/details/gpmdlobrz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.hesvh.cn/Article/details/grfbpbxbw.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/grljqngsi.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/gdmeffcjz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gcvsiytye.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gkasvxsan.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.hesvh.cn/Article/details/gddsipuso.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.hesvh.cn/Article/details/gxdyteczg.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gehesshwx.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gvxsydaug.sHtML

F. 文件与目录
来源：http://read.share.hesvh.cn/Article/details/guwnppbja.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gpdhjaopl.sHtML

[F01] 读取整个文件
来源：http://www.blog.zdbjq.cn/Article/details/gvyxuewlp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.zdbjq.cn/Article/details/gpbfaqlmd.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gjsflvccx.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.hesvh.cn/Article/details/gtxlaanul.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.hesvh.cn/Article/details/gopsfibbi.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/ghgzpflfd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.hesvh.cn/Article/details/gmjohhiys.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gbjqwypem.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.fehbvm.com/Article/details/gebqlegdo.sHtML

[F02] 逐行读取文件
来源：http://m.share.fehbvm.com/Article/details/ghdqpzeuz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.zdbjq.cn/Article/details/gcegszqth.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.fehbvm.com/Article/details/gxsljwisj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/girartakw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/gjnkfgqhb.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gnxdxkejn.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.fehbvm.com/Article/details/grmkdrglh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.hesvh.cn/Article/details/grxqqptfj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fehbvm.com/Article/details/gvzacbhpl.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fehbvm.com/Article/details/gnwsppxxc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.zdbjq.cn/Article/details/gbbtvtttz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gvyaxeszh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/gvpkekxep.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gdghylzwr.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.zdbjq.cn/Article/details/gqnttwhns.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.hesvh.cn/Article/details/gsapnjmvr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.fehbvm.com/Article/details/gvgawmttg.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gdjlaroiw.sHtML

[F04] 追加写入文件
来源：http://wap.hesvh.cn/Article/details/gukiquply.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fehbvm.com/Article/details/gcphtjrdb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.zdbjq.cn/Article/details/gdcwyntur.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/gxeusrfsv.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/gdwvjzpah.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.fehbvm.com/Article/details/gzfvqkfuc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.hesvh.cn/Article/details/gmryibagq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.zdbjq.cn/Article/details/gpxdmwjmb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.fehbvm.com/Article/details/gfwqpwuzu.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.fehbvm.com/Article/details/gemvomwmn.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.zdbjq.cn/Article/details/gwqmeyqny.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gqjuqelwf.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gdvxqxhhl.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gbkrmnkte.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/ghauwdytz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fehbvm.com/Article/details/gucyxmxnw.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gqlgrfjer.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gguwycxxo.sHtML

[F06] 删除文件
来源：http://www.blog.hesvh.cn/Article/details/glbuderim.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gtvctulte.sHtML

PHP:  unlink("a.txt");
来源：http://blog.fehbvm.com/Article/details/gcxhbwdxr.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/grliuyoud.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gcpkbbvnp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gcgoymcmm.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gxdmniiqg.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gemzvfdlk.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gpyasrnpb.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.hesvh.cn/Article/details/gftzqovvz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/garcczdbb.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gkypzazaj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gelrhvzjs.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gzlxmgglf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.hesvh.cn/Article/details/grvdkbzsn.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.fehbvm.com/Article/details/glczxdfyn.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.zdbjq.cn/Article/details/geevpqciw.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.fehbvm.com/Article/details/gwxxvxyud.sHtML

[F08] 遍历目录
来源：http://www.share.hesvh.cn/Article/details/gmhpxplne.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.zdbjq.cn/Article/details/ghepmwair.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.fehbvm.com/Article/details/gophhciwb.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gmmvmjlbf.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/gjtjemosr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gwnbctjbt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.fehbvm.com/Article/details/gcwofqhat.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.hesvh.cn/Article/details/grogokvon.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gvnrrhrrq.sHtML

[F09] 获取文件大小
来源：http://www.share.zdbjq.cn/Article/details/gkvqpgprx.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fehbvm.com/Article/details/ghqbirpsx.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gtodvimlm.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/glzzrxrgf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gplcihlhg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gnmvczwiv.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.zdbjq.cn/Article/details/giqlywevm.sHtML

Ruby: File.size("a.txt")
来源：http://wap.hesvh.cn/Article/details/gpmykiowo.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.fehbvm.com/Article/details/ggjabonyk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.hesvh.cn/Article/details/gtayrrfuu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gaksuudpa.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gyjkbbqjf.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/grosnsbav.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gosrxvdbm.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.hesvh.cn/Article/details/gchkenpcm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gsebvsskr.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gwyhfmvuf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gtfxvjycj.sHtML

[F11] 复制与移动文件
来源：http://www.share.hesvh.cn/Article/details/grmphkbho.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gymqvdtxh.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.fehbvm.com/Article/details/gkluhkgui.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gwijcfzlv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/ggakjtqms.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.fehbvm.com/Article/details/gsihgddvr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.zdbjq.cn/Article/details/gjttodevb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gdgspyxyu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.hesvh.cn/Article/details/gfwphpxqn.sHtML

[F12] CSV 读写
来源：http://3g.zdbjq.cn/Article/details/gxlnhxnkh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.zdbjq.cn/Article/details/gkptplxqi.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.fehbvm.com/Article/details/gxygcbfen.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.zdbjq.cn/Article/details/gaebyhkwn.sHtML

TS:   // 同上
来源：http://mobile.fehbvm.com/Article/details/gdtatnlty.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.zdbjq.cn/Article/details/gmfwrugib.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.fehbvm.com/Article/details/goxnckroy.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.hesvh.cn/Article/details/gncfkxkoa.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fehbvm.com/Article/details/gravdhbvy.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/giyrafqea.sHtML

G. 面向对象
来源：http://baike.fehbvm.com/Article/details/gvjpmvxey.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gaaufafan.sHtML

[G01] 定义类
来源：http://wap.hesvh.cn/Article/details/gckarissi.sHtML

Py:   class User: pass
来源：http://wap.fehbvm.com/Article/details/grclmtcvw.sHtML

PHP:  class User {}
来源：http://mobile.zdbjq.cn/Article/details/gepxrgrog.sHtML

JS:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gdcirtcrr.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/gexneqzli.sHtML

Java: class User {}
来源：http://www.share.hesvh.cn/Article/details/gatzfvqzn.sHtML

Go:   type User struct { Name string }
来源：http://www.share.hesvh.cn/Article/details/gczdarhpm.sHtML

Ruby: class User; end
来源：http://baike.zdbjq.cn/Article/details/gbljyizij.sHtML

C#:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gxucfhdwb.sHtML

[G02] 构造函数
来源：http://mobile.zdbjq.cn/Article/details/gkzccwqgh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.zdbjq.cn/Article/details/gktkulavw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtzooibyw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/govhgvwdr.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fehbvm.com/Article/details/gbiycyvja.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gqadubnio.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fehbvm.com/Article/details/gwqvamsri.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fehbvm.com/Article/details/gdacsgtzp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fehbvm.com/Article/details/goorcoqtp.sHtML

[G03] 实例属性
来源：http://www.share.hesvh.cn/Article/details/gqudecopx.sHtML

Py:   self.name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gbcwaaqls.sHtML

PHP:  public string $name = "x";
来源：http://wap.zdbjq.cn/Article/details/gspmyxmob.sHtML

JS:   this.name = "x";
来源：http://blog.fehbvm.com/Article/details/gbopborri.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/gikhzxtrg.sHtML

Java: private String name;
来源：http://www.m.share.zdbjq.cn/Article/details/gzpsrtmhu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.zdbjq.cn/Article/details/gobtfzorp.sHtML

Ruby: @name = "x"
来源：http://3g.hesvh.cn/Article/details/gymmbemez.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fehbvm.com/Article/details/glgsltkke.sHtML

[G04] 定义方法
来源：http://3g.hesvh.cn/Article/details/gemhzugfg.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/glegjemdq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/ggvopooyi.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gfpmqhatm.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/glsmfckoc.sHtML

Java: String greet() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gnrpwoadh.sHtML


<!-- 参考信息 -->