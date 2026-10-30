代发 wailian999

C#:   s.Replace("a", "b")
来源：http://baike.fanxiaobao.xyz/Article/details/gxcqjctij.sHtML

[E07] 按分隔符拆分
来源：http://wap.fanxiaobao.xyz/Article/details/gpjleibzy.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.fanxiaobao.xyz/Article/details/gchquihrq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.fanxiaobao.xyz/Article/details/grzaxigrn.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.fanxiaobao.xyz/Article/details/gkrlitgzl.sHtML

TS:   s.split(",")
来源：http://wap.fanxiaobao.xyz/Article/details/gitfulkno.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzkrzqfn.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guuvvaaie.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.fanxiaobao.xyz/Article/details/giloiumsg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmahurrlq.sHtML

[E08] 数组按分隔符合并
来源：http://baike.fanxiaobao.xyz/Article/details/glqxqfyer.sHtML

Py:   ",".join(items)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyztkvbmr.sHtML

PHP:  implode(",", $items);
来源：http://baike.fanxiaobao.xyz/Article/details/gucdcsmuy.sHtML

JS:   items.join(",")
来源：http://www.share.fanxiaobao.xyz/Article/details/gaunjwfxh.sHtML

TS:   items.join(",")
来源：http://3g.fanxiaobao.xyz/Article/details/gdxymgnjv.sHtML

Java: String.join(",", items)
来源：http://read.share.fanxiaobao.xyz/Article/details/giqgsvkgz.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.fanxiaobao.xyz/Article/details/ggiegmnuz.sHtML

Ruby: items.join(",")
来源：http://wap.fanxiaobao.xyz/Article/details/glzpfcieg.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtcnwntoz.sHtML

[E09] 去除所有空白字符
来源：http://www.share.fanxiaobao.xyz/Article/details/gjyrmxrrk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxahxhunf.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmlngyji.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.fanxiaobao.xyz/Article/details/gflmfolkv.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.fanxiaobao.xyz/Article/details/gbcaxbvtv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.fanxiaobao.xyz/Article/details/gbrwtxzed.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnkwhactj.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.fanxiaobao.xyz/Article/details/gzqpabcei.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkcrayayl.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.fanxiaobao.xyz/Article/details/gxccoqtjd.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.fanxiaobao.xyz/Article/details/gblidcgjo.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.fanxiaobao.xyz/Article/details/gvmplhayy.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.fanxiaobao.xyz/Article/details/gsmtmwwms.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchjffoux.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqaiozhh.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzukxfkd.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fanxiaobao.xyz/Article/details/gwbkqcqcd.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.fanxiaobao.xyz/Article/details/gbyzaanvv.sHtML

[E11] 反转字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goeosfqxh.sHtML

Py:   s[::-1]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gteokowwz.sHtML

PHP:  strrev($s);
来源：http://3g.fanxiaobao.xyz/Article/details/gqfjnvdlh.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzkokpgr.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.fanxiaobao.xyz/Article/details/glcrsnsiu.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.fanxiaobao.xyz/Article/details/gdhasaxid.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmmqrdjc.sHtML

Ruby: s.reverse
来源：http://3g.fanxiaobao.xyz/Article/details/grztfczgp.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.fanxiaobao.xyz/Article/details/gehhewusr.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.fanxiaobao.xyz/Article/details/grymhhdzr.sHtML

Py:   s.count("a")
来源：http://blog.fanxiaobao.xyz/Article/details/gvdbsvvtk.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.fanxiaobao.xyz/Article/details/gbijthcgs.sHtML

JS:   s.split("a").length - 1
来源：http://wap.fanxiaobao.xyz/Article/details/gbgvlmyib.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjndzfhi.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.fanxiaobao.xyz/Article/details/ghymzkriu.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnqfyeyq.sHtML

Ruby: s.count("a")
来源：http://blog.fanxiaobao.xyz/Article/details/gknulxcwk.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqjhtizo.sHtML

[E13] 逐字符遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gcckzxltw.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glubgnblj.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegygcrac.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fanxiaobao.xyz/Article/details/gdtucmgqi.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjxvkbhb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.fanxiaobao.xyz/Article/details/ghnxzxbll.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/geiireqgh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.fanxiaobao.xyz/Article/details/grwxnhmha.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwuacdndb.sHtML

[E14] URL 编码与 Base64
来源：http://baike.fanxiaobao.xyz/Article/details/gcjbotsqh.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdxzvwgj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.fanxiaobao.xyz/Article/details/gahmsmziy.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcljhjhtl.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvxjqkis.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.fanxiaobao.xyz/Article/details/gkzqtcyhp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyaawonqb.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.fanxiaobao.xyz/Article/details/grxagzzmq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawcmclxl.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.fanxiaobao.xyz/Article/details/gpribpitk.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fanxiaobao.xyz/Article/details/ggntxsnta.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdrpwmadj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnftkgemq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/girkffitg.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbeilzbu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gnezgaugy.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gngpxzkle.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.fanxiaobao.xyz/Article/details/geucthcik.sHtML

[E16] 数字千分位
来源：http://baike.fanxiaobao.xyz/Article/details/gecechrxo.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/glkrnzduf.sHtML

PHP:  number_format(1234567);
来源：http://baike.fanxiaobao.xyz/Article/details/gyfpfgzjw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fanxiaobao.xyz/Article/details/gzshgwibz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvqqobcx.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmuqbubgj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjwhuqvf.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.fanxiaobao.xyz/Article/details/gewqechxn.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnmegmfh.sHtML

[E17] 首字母大写
来源：http://3g.fanxiaobao.xyz/Article/details/giafmatcg.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubjklxnx.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmztarwmx.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbogsyjo.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fanxiaobao.xyz/Article/details/gpytyheng.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gokjkgtjr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqalfdjbi.sHtML

Ruby: s.capitalize
来源：http://blog.fanxiaobao.xyz/Article/details/gxwqvzgyt.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.fanxiaobao.xyz/Article/details/glfjilcfz.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmclcuns.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzlhgpurv.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.fanxiaobao.xyz/Article/details/gbraxozsp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmplhtbjt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.fanxiaobao.xyz/Article/details/guaefmdfz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.fanxiaobao.xyz/Article/details/gdfqkicrv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.fanxiaobao.xyz/Article/details/gbnugjpir.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.fanxiaobao.xyz/Article/details/gjuvwjgoh.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.fanxiaobao.xyz/Article/details/gbmkcgwkk.sHtML

[E19] 多行文本按行拆分
来源：http://baike.fanxiaobao.xyz/Article/details/gdaebwkfi.sHtML

Py:   s.splitlines()
来源：http://mobile.fanxiaobao.xyz/Article/details/gysdprpry.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtheosyjq.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.fanxiaobao.xyz/Article/details/gobxswijb.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.fanxiaobao.xyz/Article/details/gxsctgach.sHtML

Java: s.lines().toList()
来源：http://blog.fanxiaobao.xyz/Article/details/gfnfhbqcq.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.fanxiaobao.xyz/Article/details/gsquwbzoe.sHtML

Ruby: s.lines
来源：http://baike.fanxiaobao.xyz/Article/details/gydscesmm.sHtML

C#:   s.Split('\n')
来源：http://3g.fanxiaobao.xyz/Article/details/ggxvckwgd.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.fanxiaobao.xyz/Article/details/ggoiwjmtj.sHtML

Py:   if not s:
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvvbidjg.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxyuapsr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gtnhvksvc.sHtML

TS:   if (s === "") {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfwevoms.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gcrfeqfhy.sHtML

Go:   if s == "" {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gkoctczzx.sHtML

Ruby: if s.empty?
来源：http://read.share.fanxiaobao.xyz/Article/details/gkripzsee.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxrjafwk.sHtML

[E21] 超长截断加省略号
来源：http://wap.fanxiaobao.xyz/Article/details/gwikzhrgc.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fanxiaobao.xyz/Article/details/gmqwzpirg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.fanxiaobao.xyz/Article/details/gbijvwyyk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkdmoznd.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fanxiaobao.xyz/Article/details/gbdbafrgk.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.fanxiaobao.xyz/Article/details/gwegyvqns.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfkwpxmj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbxiqhpd.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.fanxiaobao.xyz/Article/details/gqqfziplp.sHtML

[E22] 字节长度与字符长度
来源：http://baike.fanxiaobao.xyz/Article/details/gmrvqjqqt.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gqmpawdlf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fanxiaobao.xyz/Article/details/gfdlrlzcn.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fanxiaobao.xyz/Article/details/gssofnzxy.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndplifpp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrwphqyf.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.fanxiaobao.xyz/Article/details/gvzprknuq.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fanxiaobao.xyz/Article/details/gezfmtzks.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.fanxiaobao.xyz/Article/details/godqbodzg.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gpkqzbylv.sHtML

F. 文件与目录
来源：http://m.share.fanxiaobao.xyz/Article/details/gxkbheyeu.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gfimfyvcg.sHtML

[F01] 读取整个文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glkgdproz.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fanxiaobao.xyz/Article/details/gkddgvxuh.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbnrkgni.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdlhikda.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.fanxiaobao.xyz/Article/details/ggwmrbmep.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.fanxiaobao.xyz/Article/details/gybywpbry.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.fanxiaobao.xyz/Article/details/gviexqrtk.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geoejslbw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/grzjdmpbz.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gteyessaj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdcplfhi.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.fanxiaobao.xyz/Article/details/gpcdvpvug.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gtykagegn.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fanxiaobao.xyz/Article/details/grvlaoeyv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrewugzw.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geuqvncpj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.fanxiaobao.xyz/Article/details/gdthpcmlx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvaqhjhrk.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaafkswdf.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fanxiaobao.xyz/Article/details/gqrkkngzw.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gcxnbsdwe.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbyuguqq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fanxiaobao.xyz/Article/details/gjbbqysex.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.fanxiaobao.xyz/Article/details/gtjlkfdrm.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fanxiaobao.xyz/Article/details/gnshtpujz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gropflxhn.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/gttnvhpcn.sHtML

[F04] 追加写入文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gdplwcayn.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkjfhdob.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.fanxiaobao.xyz/Article/details/gqzlqrbkv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fanxiaobao.xyz/Article/details/ghoxhwcss.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fanxiaobao.xyz/Article/details/gwunfqnpa.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjieygty.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.fanxiaobao.xyz/Article/details/gzplbadpm.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxixblmdl.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.fanxiaobao.xyz/Article/details/gexxbwvgq.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/ggeinvfgl.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfvxibfg.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.fanxiaobao.xyz/Article/details/gjmfkgthx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwjreumm.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gjzckeazd.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fanxiaobao.xyz/Article/details/gohyanlwc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.fanxiaobao.xyz/Article/details/gfejncznn.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gymjxhkgf.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxsltoab.sHtML

[F06] 删除文件
来源：http://blog.fanxiaobao.xyz/Article/details/gtajpaohq.sHtML

Py:   os.remove("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gydkeakzn.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gaftuqwad.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/glsvmzana.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gyrhaxumf.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.fanxiaobao.xyz/Article/details/gdoxmrmyw.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gubvpcqjq.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gyupcdskw.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/govghgubo.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.fanxiaobao.xyz/Article/details/gtujkyhby.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/glmowmzfl.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.fanxiaobao.xyz/Article/details/gdgicfoyy.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fanxiaobao.xyz/Article/details/gnmkdrsqw.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqypwkwe.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fanxiaobao.xyz/Article/details/gaopgevob.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fanxiaobao.xyz/Article/details/getcauwqh.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.fanxiaobao.xyz/Article/details/grwifrjeu.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fanxiaobao.xyz/Article/details/gqilkzcil.sHtML

[F08] 遍历目录
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrxhrusr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.fanxiaobao.xyz/Article/details/gukxczbvi.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gaoglpaqh.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmxynwas.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.fanxiaobao.xyz/Article/details/gdaqfsupz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.fanxiaobao.xyz/Article/details/gsjlzdull.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqqhcsjs.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbrlogwc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.fanxiaobao.xyz/Article/details/gyaezbaum.sHtML

[F09] 获取文件大小
来源：http://baike.fanxiaobao.xyz/Article/details/gqcvbbwvn.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gkiatbour.sHtML

PHP:  filesize("a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/guyowhfrk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fanxiaobao.xyz/Article/details/gzodhjsmw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnzjidiq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.fanxiaobao.xyz/Article/details/ggsiaomzc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkpwlqsc.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gqwpmjsgh.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gogeakwba.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.fanxiaobao.xyz/Article/details/geaylnaow.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqrniuiu.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrrzhvif.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbppaeio.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtziftsm.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwyoxbqeo.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gpmqcgicy.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gvslwcjyc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfasrjgb.sHtML

[F11] 复制与移动文件
来源：http://blog.fanxiaobao.xyz/Article/details/glnyaosle.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbwpplat.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gubalixyl.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gkrziwszp.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gnucvhyyw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fanxiaobao.xyz/Article/details/gmynawuib.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.fanxiaobao.xyz/Article/details/gdulsmvtb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gbruvauey.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.fanxiaobao.xyz/Article/details/gonxcsvno.sHtML

[F12] CSV 读写
来源：http://wap.fanxiaobao.xyz/Article/details/gbbibpcnz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmhdoncl.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fanxiaobao.xyz/Article/details/guazfisua.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.fanxiaobao.xyz/Article/details/gqopsjegz.sHtML

TS:   // 同上
来源：http://baike.fanxiaobao.xyz/Article/details/gvbroidwh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzwjpery.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.fanxiaobao.xyz/Article/details/getodurpq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fanxiaobao.xyz/Article/details/gdxpglhti.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fanxiaobao.xyz/Article/details/gknwelfos.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/glzjldijg.sHtML

G. 面向对象
来源：http://3g.fanxiaobao.xyz/Article/details/gxzjyietb.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gxnadyorx.sHtML

[G01] 定义类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndeiamsd.sHtML

Py:   class User: pass
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmnedxsu.sHtML

PHP:  class User {}
来源：http://www.share.fanxiaobao.xyz/Article/details/geuykkfqt.sHtML

JS:   class User {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnquzyzm.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkinjgtg.sHtML

Java: class User {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkuvuaic.sHtML

Go:   type User struct { Name string }
来源：http://baike.fanxiaobao.xyz/Article/details/ghkfgyshf.sHtML

Ruby: class User; end
来源：http://baike.fanxiaobao.xyz/Article/details/glmhbqcgy.sHtML

C#:   class User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcyxfbsy.sHtML

[G02] 构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhxefkie.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfmzvboi.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnjmvdvf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnqchjmk.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbrgmbjx.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gskwaogip.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbdpvhpm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gaarduwsf.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjrwvpnxy.sHtML

[G03] 实例属性
来源：http://read.share.fanxiaobao.xyz/Article/details/guckqtffc.sHtML

Py:   self.name = "x"
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdmjocxp.sHtML

PHP:  public string $name = "x";
来源：http://blog.fanxiaobao.xyz/Article/details/gzmwrgbza.sHtML

JS:   this.name = "x";
来源：http://www.share.fanxiaobao.xyz/Article/details/glxxorhaj.sHtML

TS:   name: string = "x";
来源：http://read.share.fanxiaobao.xyz/Article/details/gopokjzmj.sHtML

Java: private String name;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmyvyllgt.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fanxiaobao.xyz/Article/details/gxapbgxmu.sHtML

Ruby: @name = "x"
来源：http://blog.fanxiaobao.xyz/Article/details/geddoqrce.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.fanxiaobao.xyz/Article/details/gtgqbtbiw.sHtML

[G04] 定义方法
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvqudhxi.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.fanxiaobao.xyz/Article/details/gdsvffjzk.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gejrgyzmf.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/godlmervb.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfykpjkj.sHtML

Java: String greet() { return name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gahjvmsvb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fanxiaobao.xyz/Article/details/gxbusewmb.sHtML

Ruby: def greet; @name; end
来源：http://blog.fanxiaobao.xyz/Article/details/gfwxhzclz.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmtsrzdx.sHtML

[G05] 继承
来源：http://3g.fanxiaobao.xyz/Article/details/gtaputbde.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwadheso.sHtML

PHP:  class Admin extends User {}
来源：http://3g.fanxiaobao.xyz/Article/details/gkcpohoid.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gygmwljyp.sHtML

TS:   class Admin extends User {}
来源：http://wap.fanxiaobao.xyz/Article/details/goulhzenv.sHtML


<!-- 参考信息 -->