代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/gwfxxzwuv.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.fehbvm.com/Article/details/gutzbrtrm.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.fehbvm.com/Article/details/gyorclavk.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gsqonigpb.sHtML

[E06] 替换子串
来源：http://read.share.zdbjq.cn/Article/details/guczdgxla.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gqqvyoojc.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.zdbjq.cn/Article/details/ggsgqayan.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gmdcjlkbk.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gnjjqghyp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gwnvrxtwb.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/glgahjrqi.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gxxqdtszr.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gvjvykazw.sHtML

[E07] 按分隔符拆分
来源：http://baike.zdbjq.cn/Article/details/grixnvugy.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.zdbjq.cn/Article/details/gocowzbfu.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.zdbjq.cn/Article/details/gzofqpdhu.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gcgrlmwae.sHtML

TS:   s.split(",")
来源：http://www.m.share.fehbvm.com/Article/details/grycwpzji.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.hesvh.cn/Article/details/gllzblfjr.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.zdbjq.cn/Article/details/gztmfcbrl.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.zdbjq.cn/Article/details/grnlnvnym.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.fehbvm.com/Article/details/gmopwqfzl.sHtML

[E08] 数组按分隔符合并
来源：http://3g.zdbjq.cn/Article/details/gfdtnnccv.sHtML

Py:   ",".join(items)
来源：http://m.share.fehbvm.com/Article/details/gstqmjvjd.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.hesvh.cn/Article/details/gwoysijic.sHtML

JS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gclwuaorl.sHtML

TS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gzkmwtbby.sHtML

Java: String.join(",", items)
来源：http://baike.fehbvm.com/Article/details/gebshensh.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.zdbjq.cn/Article/details/gmyiofpbd.sHtML

Ruby: items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gfsjdmvhq.sHtML

C#:   string.Join(",", items)
来源：http://blog.fehbvm.com/Article/details/gbldovrtp.sHtML

[E09] 去除所有空白字符
来源：http://wap.hesvh.cn/Article/details/gscvrawva.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.fehbvm.com/Article/details/ggsrdakuk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gbaanurzp.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/giqelrzyx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/gxxlkeyxy.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/geyfrbwxo.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.zdbjq.cn/Article/details/gaqaphfed.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.fehbvm.com/Article/details/gxplktbjg.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/gelfazizd.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.zdbjq.cn/Article/details/gehhpeiwq.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/grdixsvnz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.zdbjq.cn/Article/details/gcaiyapyo.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gbwqcrytl.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gtcvgjiri.sHtML

Java: String.format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gcoreyqcx.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/ggzfuvfge.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gpdymibud.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.zdbjq.cn/Article/details/gfyjmmjvr.sHtML

[E11] 反转字符串
来源：http://mobile.fehbvm.com/Article/details/ghuahnrcx.sHtML

Py:   s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gxdkikzhp.sHtML

PHP:  strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gptirbuke.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gkhdosatp.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/ggnkjirwd.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.hesvh.cn/Article/details/guaojzlbh.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.zdbjq.cn/Article/details/gesxhsnyw.sHtML

Ruby: s.reverse
来源：http://3g.fehbvm.com/Article/details/gistufdgm.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gfflufqla.sHtML

[E12] 统计某字符出现次数
来源：http://blog.zdbjq.cn/Article/details/gbnidpqvn.sHtML

Py:   s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gwhwviwyu.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.zdbjq.cn/Article/details/goubnvljk.sHtML

JS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/gmxnfvevg.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gbkvmslvv.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.hesvh.cn/Article/details/gcmucwjux.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.fehbvm.com/Article/details/gzbhwngte.sHtML

Ruby: s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/gpqkdmymt.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.hesvh.cn/Article/details/gxcoejurb.sHtML

[E13] 逐字符遍历
来源：http://3g.fehbvm.com/Article/details/gprgwcifw.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.zdbjq.cn/Article/details/gyqnyzzyi.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.fehbvm.com/Article/details/gwvwqbsyl.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gfwgtuzav.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gccbpvfgx.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gjgajhsee.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.fehbvm.com/Article/details/gsbqrlfbx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.hesvh.cn/Article/details/gfeeywxoy.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gzvvwuoqf.sHtML

[E14] URL 编码与 Base64
来源：http://3g.fehbvm.com/Article/details/gsvbtrbmg.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.hesvh.cn/Article/details/gityeaifx.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.fehbvm.com/Article/details/goqropkjd.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.fehbvm.com/Article/details/gqsxvfwxs.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.fehbvm.com/Article/details/gxfnjxnrx.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.fehbvm.com/Article/details/grzqpwiue.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.fehbvm.com/Article/details/gknpqrfqb.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.zdbjq.cn/Article/details/gmpepeqni.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gweppipun.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.zdbjq.cn/Article/details/gbcywsywl.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.fehbvm.com/Article/details/gllowposf.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.zdbjq.cn/Article/details/gfyqdfckb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.hesvh.cn/Article/details/gxcvggsvj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.zdbjq.cn/Article/details/gfwlndttk.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.hesvh.cn/Article/details/ghwyurfuc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.zdbjq.cn/Article/details/ghalywveg.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.zdbjq.cn/Article/details/gsmlrunix.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.fehbvm.com/Article/details/gcysrlguq.sHtML

[E16] 数字千分位
来源：http://wap.fehbvm.com/Article/details/gwgfuxsbj.sHtML

Py:   f"{1234567:,}"
来源：http://baike.hesvh.cn/Article/details/gfdmhhwxw.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.hesvh.cn/Article/details/gecrlxocx.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gycywwxgn.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gaifodctx.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/gnhbwzidt.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.fehbvm.com/Article/details/ghhtddnrs.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.fehbvm.com/Article/details/gznkwdasa.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.zdbjq.cn/Article/details/gaupaurik.sHtML

[E17] 首字母大写
来源：http://read.share.hesvh.cn/Article/details/gmfscbuup.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.zdbjq.cn/Article/details/goldkrkzd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fehbvm.com/Article/details/gdulfiqgz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/grpsrlirz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/gadjvbavy.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.zdbjq.cn/Article/details/gngdfnszi.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.fehbvm.com/Article/details/gdzsrmnep.sHtML

Ruby: s.capitalize
来源：http://mobile.hesvh.cn/Article/details/gyymcfclg.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fehbvm.com/Article/details/gvbvhrwhm.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.zdbjq.cn/Article/details/gwkaowrom.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.hesvh.cn/Article/details/gbdeosljw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.fehbvm.com/Article/details/gwpbzweue.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gkilmbtbx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/glbbtbyxi.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.hesvh.cn/Article/details/ghjypzsor.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gvzseobxk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.zdbjq.cn/Article/details/gioxjspsn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.fehbvm.com/Article/details/glbsnmlqd.sHtML

[E19] 多行文本按行拆分
来源：http://blog.hesvh.cn/Article/details/gklfdgvzg.sHtML

Py:   s.splitlines()
来源：http://www.share.zdbjq.cn/Article/details/gzgiwwqvd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gqwdsncia.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/gwozlhwbp.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gzgxwlyvd.sHtML

Java: s.lines().toList()
来源：http://baike.hesvh.cn/Article/details/gwknrdcbv.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.fehbvm.com/Article/details/ggkkdciwy.sHtML

Ruby: s.lines
来源：http://3g.hesvh.cn/Article/details/gngpcsjxc.sHtML

C#:   s.Split('\n')
来源：http://blog.hesvh.cn/Article/details/gtiejnwtw.sHtML

[E20] 判断字符串是否为空
来源：http://baike.fehbvm.com/Article/details/gwnpfoqia.sHtML

Py:   if not s:
来源：http://baike.fehbvm.com/Article/details/gugegiugh.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.zdbjq.cn/Article/details/gglktlghm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.zdbjq.cn/Article/details/gkiixamoz.sHtML

TS:   if (s === "") {}
来源：http://www.share.fehbvm.com/Article/details/gcfjiiyil.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gptukilmc.sHtML

Go:   if s == "" {}
来源：http://baike.hesvh.cn/Article/details/gncudbtry.sHtML

Ruby: if s.empty?
来源：http://wap.zdbjq.cn/Article/details/gtvtftqnk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.fehbvm.com/Article/details/gwdvktpmj.sHtML

[E21] 超长截断加省略号
来源：http://3g.hesvh.cn/Article/details/gudkwuqmj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fehbvm.com/Article/details/gmxyohjrd.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gtowlkdpz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gwfqcqkkh.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gwuwjtugx.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gthnexabb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.hesvh.cn/Article/details/gkecswcau.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gmcgtprmf.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/grjmhiisp.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.zdbjq.cn/Article/details/gdaowuzoy.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.hesvh.cn/Article/details/gvofzpdrt.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gimxcjppf.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gcxpvzytw.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/gpxjmtemz.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.fehbvm.com/Article/details/gjigvuojq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.zdbjq.cn/Article/details/gqghthxah.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.hesvh.cn/Article/details/gcjbcncnp.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.hesvh.cn/Article/details/gwvsbypjo.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gtxjfzmkj.sHtML

F. 文件与目录
来源：http://mobile.hesvh.cn/Article/details/gbnwslmdx.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxyfcfxbo.sHtML

[F01] 读取整个文件
来源：http://3g.fehbvm.com/Article/details/gxgaclddg.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.fehbvm.com/Article/details/gbzjwpmio.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.hesvh.cn/Article/details/giganlgew.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.zdbjq.cn/Article/details/gyakdstqm.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gasfzemzq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gybwnoszk.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.hesvh.cn/Article/details/ghgynomhm.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gbypmfmvb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/grcskrjqz.sHtML

[F02] 逐行读取文件
来源：http://3g.hesvh.cn/Article/details/gmuzsdsut.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.fehbvm.com/Article/details/ggwsevtwk.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.zdbjq.cn/Article/details/gjirasrjo.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gojpucprf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/gerjdmeyw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gmhtgswxb.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.hesvh.cn/Article/details/ggmkfuyev.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.zdbjq.cn/Article/details/gpvagdsnc.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.hesvh.cn/Article/details/gnndaudvu.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.hesvh.cn/Article/details/gjnuohdxz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.hesvh.cn/Article/details/gmwlogvhz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/gjihcuavh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/glumxopuf.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gmqbapqux.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.hesvh.cn/Article/details/glksxeudl.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.fehbvm.com/Article/details/gufrilsrd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gfsodtuta.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/glcnuoqpj.sHtML

[F04] 追加写入文件
来源：http://baike.zdbjq.cn/Article/details/gcuvgtqso.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.zdbjq.cn/Article/details/gegjsdyui.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.zdbjq.cn/Article/details/gznqigqqs.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/gxrolibil.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gepweoxxo.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.fehbvm.com/Article/details/gvllhxwhj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/ggbenomge.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.fehbvm.com/Article/details/gjxnrnkub.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.hesvh.cn/Article/details/gtikhgjgr.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.fehbvm.com/Article/details/gdamczooy.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.hesvh.cn/Article/details/govvdqpqy.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gvgmkjaqf.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gwezzsywn.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gcsewtiwh.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gifpnrbgc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.zdbjq.cn/Article/details/gadcmjbrp.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/ggvlpphav.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fehbvm.com/Article/details/ginaajxuj.sHtML

[F06] 删除文件
来源：http://www.blog.zdbjq.cn/Article/details/gudbtermt.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/grngnbsec.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gqcjuvxfx.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/guontxfcn.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/guzjdghlc.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/givtbnpgx.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gkxantpal.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gzgtuitfo.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gqlgfjszc.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.fehbvm.com/Article/details/gyjvbpelj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gtymwvqcu.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.fehbvm.com/Article/details/gwhnjrulw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gvqpevxzd.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/gxadabvoy.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.zdbjq.cn/Article/details/gxqfshmnr.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.zdbjq.cn/Article/details/gdxobfesx.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.hesvh.cn/Article/details/gjopxlyye.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.hesvh.cn/Article/details/gnbfwxvcs.sHtML

[F08] 遍历目录
来源：http://3g.zdbjq.cn/Article/details/gfhmxnxji.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.zdbjq.cn/Article/details/guaiarrah.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.fehbvm.com/Article/details/grupplynb.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/giklpfcmc.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/girpugwpk.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gtmyqhwla.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.hesvh.cn/Article/details/gnvtfshcn.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.hesvh.cn/Article/details/gtlqforcg.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.zdbjq.cn/Article/details/gawtfzflz.sHtML

[F09] 获取文件大小
来源：http://baike.fehbvm.com/Article/details/grdombade.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gdppbglvz.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gnccskzbo.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gkoidtazq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/getwlmeyb.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gzyslapup.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.hesvh.cn/Article/details/gvqcsfrdk.sHtML

Ruby: File.size("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gvihkigkc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.zdbjq.cn/Article/details/gxjcfdqhg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.hesvh.cn/Article/details/gupuzjtjp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gestzfekk.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.hesvh.cn/Article/details/gebdhzuuy.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gxbmddbkb.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gjqhojnud.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.zdbjq.cn/Article/details/gktuyrayq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gvcpbvyvz.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gygaydkeo.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gyprmxdjc.sHtML

[F11] 复制与移动文件
来源：http://3g.fehbvm.com/Article/details/gktyexxov.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gdkmyvgat.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.zdbjq.cn/Article/details/gvrwprakf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/glranlfxs.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gjebwumvm.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.fehbvm.com/Article/details/ggvdjuucp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.hesvh.cn/Article/details/gesgatbvc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gzsaqghqo.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.hesvh.cn/Article/details/gwisikphj.sHtML

[F12] CSV 读写
来源：http://baike.zdbjq.cn/Article/details/gjbanlgdd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fehbvm.com/Article/details/gugddosxw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.hesvh.cn/Article/details/gappqlcyb.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.fehbvm.com/Article/details/gzgyocziq.sHtML

TS:   // 同上
来源：http://www.share.fehbvm.com/Article/details/gzqefgegt.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.zdbjq.cn/Article/details/gbhvvgumt.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.hesvh.cn/Article/details/gvsivdaqs.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.hesvh.cn/Article/details/gpqqgqynv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.hesvh.cn/Article/details/gjvaporqx.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gkczsyjgb.sHtML

G. 面向对象
来源：http://read.share.zdbjq.cn/Article/details/gzgyogqts.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjbbogqcl.sHtML

[G01] 定义类
来源：http://www.blog.hesvh.cn/Article/details/gsaurjglj.sHtML

Py:   class User: pass
来源：http://www.share.zdbjq.cn/Article/details/gturbmued.sHtML

PHP:  class User {}
来源：http://m.share.fehbvm.com/Article/details/gpsoyypwa.sHtML

JS:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gfbiuvoaa.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/gxqzhboot.sHtML

Java: class User {}
来源：http://mobile.zdbjq.cn/Article/details/gbnmkxhro.sHtML

Go:   type User struct { Name string }
来源：http://m.share.zdbjq.cn/Article/details/gvofycrlk.sHtML

Ruby: class User; end
来源：http://3g.zdbjq.cn/Article/details/gsmdozmpt.sHtML

C#:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gavbgjmmf.sHtML

[G02] 构造函数
来源：http://blog.zdbjq.cn/Article/details/grekpyltx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.hesvh.cn/Article/details/gbjwbwagt.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.hesvh.cn/Article/details/gujxeykbx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsqyigqyv.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.hesvh.cn/Article/details/gcgtxiicf.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/ghzcdusaf.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.hesvh.cn/Article/details/gybmjaueh.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.zdbjq.cn/Article/details/glrmzrjxn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gvjsmeuji.sHtML

[G03] 实例属性
来源：http://mobile.zdbjq.cn/Article/details/gaxfswjta.sHtML

Py:   self.name = "x"
来源：http://read.share.zdbjq.cn/Article/details/glbgvgyrh.sHtML

PHP:  public string $name = "x";
来源：http://3g.fehbvm.com/Article/details/gulsyrjix.sHtML

JS:   this.name = "x";
来源：http://www.share.hesvh.cn/Article/details/gyroufviu.sHtML

TS:   name: string = "x";
来源：http://wap.hesvh.cn/Article/details/gcbmqnrvc.sHtML

Java: private String name;
来源：http://m.share.fehbvm.com/Article/details/gjsnpiswd.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.fehbvm.com/Article/details/goylbnfon.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gadgajbat.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fehbvm.com/Article/details/giqdceidt.sHtML

[G04] 定义方法
来源：http://baike.zdbjq.cn/Article/details/gtahmisfx.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gdcaabzob.sHtML


<!-- 参考信息 -->