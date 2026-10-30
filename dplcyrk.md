代发 wailian999

[E06] 替换子串
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrqnbohl.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxwtkxan.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmguvztew.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/gevjlvyeb.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbkyelhw.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqwkyfkg.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gpyuwjqld.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.fanxiaobao.xyz/Article/details/gmprhrqhj.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzygmxla.sHtML

[E07] 按分隔符拆分
来源：http://blog.fanxiaobao.xyz/Article/details/gmuislenp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.fanxiaobao.xyz/Article/details/ghkmmcakx.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/gxsmqbehy.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyknhhxhe.sHtML

TS:   s.split(",")
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtwfgyfy.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goryeoccp.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gjoomlayh.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.fanxiaobao.xyz/Article/details/gmldkfkgw.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.fanxiaobao.xyz/Article/details/gskhxlyev.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.fanxiaobao.xyz/Article/details/guhhhjtle.sHtML

Py:   ",".join(items)
来源：http://wap.fanxiaobao.xyz/Article/details/ghbbcrfjv.sHtML

PHP:  implode(",", $items);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvgcxxpx.sHtML

JS:   items.join(",")
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgcyykrr.sHtML

TS:   items.join(",")
来源：http://m.share.fanxiaobao.xyz/Article/details/ggezpttdp.sHtML

Java: String.join(",", items)
来源：http://3g.fanxiaobao.xyz/Article/details/gzcatevca.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gacarsrnz.sHtML

Ruby: items.join(",")
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdweicyr.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvgbghvc.sHtML

[E09] 去除所有空白字符
来源：http://blog.fanxiaobao.xyz/Article/details/gfnvdsgrg.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.fanxiaobao.xyz/Article/details/gdmvfwabr.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmehfafui.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.fanxiaobao.xyz/Article/details/gesaglslf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvoqvohw.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqleafag.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqpwtajt.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.fanxiaobao.xyz/Article/details/gazhspirv.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.fanxiaobao.xyz/Article/details/grgrsymqg.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.fanxiaobao.xyz/Article/details/ggonftcgr.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdfrxknd.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fanxiaobao.xyz/Article/details/ggbzpoxrp.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.fanxiaobao.xyz/Article/details/gtwxicdgc.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbrnsfpa.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gakvlokcm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkjtiypq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.fanxiaobao.xyz/Article/details/gfmbmrweh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.fanxiaobao.xyz/Article/details/gyodvgixz.sHtML

[E11] 反转字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/ghxhoczca.sHtML

Py:   s[::-1]
来源：http://mobile.fanxiaobao.xyz/Article/details/gtyhdpmqw.sHtML

PHP:  strrev($s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfgqtvnv.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvsandkt.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkborflt.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.fanxiaobao.xyz/Article/details/gpzwajupb.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.fanxiaobao.xyz/Article/details/gwtklkxqc.sHtML

Ruby: s.reverse
来源：http://baike.fanxiaobao.xyz/Article/details/ghzqmuity.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjtijlvq.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.fanxiaobao.xyz/Article/details/gngvabycg.sHtML

Py:   s.count("a")
来源：http://blog.fanxiaobao.xyz/Article/details/gefbfqqqy.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.fanxiaobao.xyz/Article/details/guhmtuxqj.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gatgdzszo.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.fanxiaobao.xyz/Article/details/ggszhdihx.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnhnumzo.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.fanxiaobao.xyz/Article/details/gpertwspy.sHtML

Ruby: s.count("a")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gklgwhlwv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtsuveiat.sHtML

[E13] 逐字符遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gplxckxjb.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.fanxiaobao.xyz/Article/details/glbjkugae.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmydesomj.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gaekjkopj.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmnxlvbn.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.fanxiaobao.xyz/Article/details/gbogidcjy.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gvfbmwsbh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbbjclbs.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.fanxiaobao.xyz/Article/details/ghplviocb.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdhaoqfu.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.fanxiaobao.xyz/Article/details/gzibtzwyz.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjcfuetn.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwgzxeyi.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.fanxiaobao.xyz/Article/details/getnsmffg.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.fanxiaobao.xyz/Article/details/grmftnmlb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbwwayas.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.fanxiaobao.xyz/Article/details/giyzxmftv.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.fanxiaobao.xyz/Article/details/gakbvllac.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.fanxiaobao.xyz/Article/details/gsawhkkwy.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gbcxpguaz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtimkregp.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgfbqikr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjlwvjust.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkejnfcd.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnygkejem.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fanxiaobao.xyz/Article/details/ghvvxwfcp.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gdmerkrob.sHtML

[E16] 数字千分位
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxbqtxpj.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gllfxfftm.sHtML

PHP:  number_format(1234567);
来源：http://blog.fanxiaobao.xyz/Article/details/gimpundiv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwgiaqajf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.fanxiaobao.xyz/Article/details/ghbqolknu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.fanxiaobao.xyz/Article/details/geddspymp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.fanxiaobao.xyz/Article/details/gjucfsndc.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqcdngfam.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.fanxiaobao.xyz/Article/details/guyfxzxax.sHtML

[E17] 首字母大写
来源：http://www.share.fanxiaobao.xyz/Article/details/glmwihuwz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjccifnmt.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fanxiaobao.xyz/Article/details/gtwlucwwg.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/guxzwgscn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gexpuytam.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzctnqoay.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.fanxiaobao.xyz/Article/details/graqlhuiw.sHtML

Ruby: s.capitalize
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqqzogcm.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.fanxiaobao.xyz/Article/details/gikobqoth.sHtML

[E18] 模板占位符替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gaekiuxwd.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gundpzgmo.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.fanxiaobao.xyz/Article/details/gdfczvkla.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmtezumx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.fanxiaobao.xyz/Article/details/ghmmmrwsi.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmgfhckl.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.fanxiaobao.xyz/Article/details/ggwjimtkl.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.fanxiaobao.xyz/Article/details/gpqyocvlj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkshpxas.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwxlgkdjj.sHtML

Py:   s.splitlines()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymqzwiod.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/gjvqvdipt.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdwtnurb.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsdeybrui.sHtML

Java: s.lines().toList()
来源：http://3g.fanxiaobao.xyz/Article/details/gtgrmyqyx.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.fanxiaobao.xyz/Article/details/guhkbeeez.sHtML

Ruby: s.lines
来源：http://blog.fanxiaobao.xyz/Article/details/gieskgmaj.sHtML

C#:   s.Split('\n')
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjtevzsk.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.fanxiaobao.xyz/Article/details/gjcuupbfi.sHtML

Py:   if not s:
来源：http://3g.fanxiaobao.xyz/Article/details/gguitsdny.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwifeucke.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gbilctkar.sHtML

TS:   if (s === "") {}
来源：http://m.share.fanxiaobao.xyz/Article/details/geqjbxvfy.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gephyijkr.sHtML

Go:   if s == "" {}
来源：http://blog.fanxiaobao.xyz/Article/details/gednoakfr.sHtML

Ruby: if s.empty?
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvpoxjqoi.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fanxiaobao.xyz/Article/details/ginlmxlxl.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxmeonrb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvhzvyee.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.fanxiaobao.xyz/Article/details/gbryxvseu.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxfsladf.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fanxiaobao.xyz/Article/details/goamqxkok.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqtfwjir.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fanxiaobao.xyz/Article/details/glehvmimk.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpseeioym.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.fanxiaobao.xyz/Article/details/grhxrlklc.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fanxiaobao.xyz/Article/details/grfkvecho.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfyjckczk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fanxiaobao.xyz/Article/details/gaoznxvgt.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpljaxdl.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gepmyovcl.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.fanxiaobao.xyz/Article/details/gulubqoqr.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fanxiaobao.xyz/Article/details/ggssebjnh.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gducfhljn.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.fanxiaobao.xyz/Article/details/gejzjhgpf.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gppilrfsc.sHtML

F. 文件与目录
来源：http://blog.fanxiaobao.xyz/Article/details/gjgjnffge.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gppevnusj.sHtML

[F01] 读取整个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfmsqhur.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.fanxiaobao.xyz/Article/details/gyogidsrs.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gelbjelum.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.fanxiaobao.xyz/Article/details/gmdqhxbmf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwhqtcuz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fanxiaobao.xyz/Article/details/gwoqmwuxc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.fanxiaobao.xyz/Article/details/gdtvmtuvn.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmklvdwe.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/gkiwmnekq.sHtML

[F02] 逐行读取文件
来源：http://baike.fanxiaobao.xyz/Article/details/gylhldhqa.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.fanxiaobao.xyz/Article/details/gtwjsnxni.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.fanxiaobao.xyz/Article/details/galgvvndh.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gxplidduf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gmvuosrop.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.fanxiaobao.xyz/Article/details/gnnmqwkgz.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmhdmoag.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjfetmml.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwngcvbyd.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glabmvidi.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.fanxiaobao.xyz/Article/details/grtnezraj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/genqidrlr.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fanxiaobao.xyz/Article/details/gstoaivny.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fanxiaobao.xyz/Article/details/gikcfvbas.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfpbfqan.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubgayxya.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.fanxiaobao.xyz/Article/details/gtailixvm.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxqbdxdk.sHtML

[F04] 追加写入文件
来源：http://wap.fanxiaobao.xyz/Article/details/gccafpncl.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohludkvp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.fanxiaobao.xyz/Article/details/ggihphymo.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fanxiaobao.xyz/Article/details/gepnpglrp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fanxiaobao.xyz/Article/details/gsypznpyw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdscdbslp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fanxiaobao.xyz/Article/details/gmdnzfndm.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.fanxiaobao.xyz/Article/details/ggmsaiyrj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.fanxiaobao.xyz/Article/details/gsfhnfgyz.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gcaxmygaf.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.fanxiaobao.xyz/Article/details/gdjrbdtkm.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/gerxsyjdg.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/ggtpjseje.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gukgyiwdl.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.fanxiaobao.xyz/Article/details/gxtoaetfw.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fanxiaobao.xyz/Article/details/ggaihiurz.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gxwiicbxq.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggqpepyvv.sHtML

[F06] 删除文件
来源：http://blog.fanxiaobao.xyz/Article/details/gpwhhcfcf.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwbryfzt.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/grwhffbbv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgrkpctr.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gidxnrzaw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fanxiaobao.xyz/Article/details/gethellap.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/guggoahqe.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynoitnaa.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.fanxiaobao.xyz/Article/details/gtsgvxbgd.sHtML

[F07] 创建目录（含多级）
来源：http://3g.fanxiaobao.xyz/Article/details/glfogmnao.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/gotmwdkfu.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goqymqwcc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fanxiaobao.xyz/Article/details/gvtxwjlmk.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fanxiaobao.xyz/Article/details/gjaoubdpl.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcfatfmk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfldhfpnd.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxywjllf.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.fanxiaobao.xyz/Article/details/gjogknsuc.sHtML

[F08] 遍历目录
来源：http://3g.fanxiaobao.xyz/Article/details/gmkypbcei.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fanxiaobao.xyz/Article/details/gflaxbvhm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlfxpruh.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gydfnrmab.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmljvsgr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.fanxiaobao.xyz/Article/details/gfnvgdvgh.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.fanxiaobao.xyz/Article/details/gebgrpuna.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fanxiaobao.xyz/Article/details/gdtavxlvq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.fanxiaobao.xyz/Article/details/gahelgpul.sHtML

[F09] 获取文件大小
来源：http://3g.fanxiaobao.xyz/Article/details/grfropklc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/grfijyrjc.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghikdyqmo.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.fanxiaobao.xyz/Article/details/gofsagnyu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fanxiaobao.xyz/Article/details/grmnlbnvr.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fanxiaobao.xyz/Article/details/gckwmksxx.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fanxiaobao.xyz/Article/details/gecmwuoba.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwuxloyc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fanxiaobao.xyz/Article/details/gipmzjkeg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.fanxiaobao.xyz/Article/details/guyxlqoqe.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gpldefmts.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gslarxdmu.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcpihkqfn.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/girpgxydp.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fanxiaobao.xyz/Article/details/gnxswcqph.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/ggjjuwsiw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gqchdupav.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzkrcvni.sHtML

[F11] 复制与移动文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmbxzwjc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gizkxdkbi.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/gsehacahp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdxvnhkfw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gbzsbfvvn.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.fanxiaobao.xyz/Article/details/gdnyoatjz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvduvlor.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gyuizpltd.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbpaoncqf.sHtML

[F12] CSV 读写
来源：http://read.share.fanxiaobao.xyz/Article/details/gmtthuyqx.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbafkrlsx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.fanxiaobao.xyz/Article/details/gclxslqxd.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.fanxiaobao.xyz/Article/details/gklqyjrwx.sHtML

TS:   // 同上
来源：http://blog.fanxiaobao.xyz/Article/details/ghkxivmcw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giukqspra.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.fanxiaobao.xyz/Article/details/gccmsuixg.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.fanxiaobao.xyz/Article/details/gysqjukjg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmxcmsljb.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gvshqgwkp.sHtML

G. 面向对象
来源：http://blog.fanxiaobao.xyz/Article/details/gjcgxxwem.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxuplmlb.sHtML

[G01] 定义类
来源：http://read.share.fanxiaobao.xyz/Article/details/glltlwnue.sHtML

Py:   class User: pass
来源：http://blog.fanxiaobao.xyz/Article/details/gwhgmwhgc.sHtML

PHP:  class User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjfihmmo.sHtML

JS:   class User {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrmsawds.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdthnpsog.sHtML

Java: class User {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvrexovlt.sHtML

Go:   type User struct { Name string }
来源：http://www.share.fanxiaobao.xyz/Article/details/gavinvaco.sHtML

Ruby: class User; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gibikqyps.sHtML

C#:   class User {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gysdjehce.sHtML

[G02] 构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqmtfvgs.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.fanxiaobao.xyz/Article/details/gnyijnzeo.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytrsjilu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhrmguod.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbobxlgq.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fanxiaobao.xyz/Article/details/glsfpvybz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbdvmykx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnxudfwz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwhqczgoy.sHtML

[G03] 实例属性
来源：http://wap.fanxiaobao.xyz/Article/details/gwyuwupby.sHtML

Py:   self.name = "x"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavrpodqe.sHtML

PHP:  public string $name = "x";
来源：http://3g.fanxiaobao.xyz/Article/details/gxaesyxvg.sHtML

JS:   this.name = "x";
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzgslwte.sHtML

TS:   name: string = "x";
来源：http://blog.fanxiaobao.xyz/Article/details/gjxalruhp.sHtML

Java: private String name;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gruernghh.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fanxiaobao.xyz/Article/details/gudfwqrzo.sHtML

Ruby: @name = "x"
来源：http://www.share.fanxiaobao.xyz/Article/details/glxpuvfbw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozrvtgra.sHtML

[G04] 定义方法
来源：http://3g.fanxiaobao.xyz/Article/details/gskewnwnu.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.fanxiaobao.xyz/Article/details/gguizootx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwqwbivo.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gvqkswlec.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gwubbzjxg.sHtML

Java: String greet() { return name; }
来源：http://3g.fanxiaobao.xyz/Article/details/glkxrviql.sHtML


<!-- 参考信息 -->