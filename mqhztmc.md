代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/ggphktamf.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gwehtbnix.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/gfiymnucc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gqpeclzkd.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fehbvm.com/Article/details/gqmkqerpp.sHtML

[E07] 按分隔符拆分
来源：http://read.share.hesvh.cn/Article/details/gdczediyw.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.hesvh.cn/Article/details/gdjnmjeyy.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gbxhpbqju.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.zdbjq.cn/Article/details/griagsdoc.sHtML

TS:   s.split(",")
来源：http://read.share.fehbvm.com/Article/details/guhqwzcdd.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.zdbjq.cn/Article/details/gtvdkdvip.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.hesvh.cn/Article/details/gxzzlszcj.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.fehbvm.com/Article/details/gvvzmyyjv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.zdbjq.cn/Article/details/glzisfxlp.sHtML

[E08] 数组按分隔符合并
来源：http://3g.hesvh.cn/Article/details/gfyturetk.sHtML

Py:   ",".join(items)
来源：http://www.m.share.fehbvm.com/Article/details/gkrxhfjft.sHtML

PHP:  implode(",", $items);
来源：http://www.share.hesvh.cn/Article/details/giqhzhlzl.sHtML

JS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gvtjednur.sHtML

TS:   items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gzthpdhsa.sHtML

Java: String.join(",", items)
来源：http://wap.zdbjq.cn/Article/details/gvanzzusc.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.fehbvm.com/Article/details/giwbvqgkf.sHtML

Ruby: items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gnluuzewb.sHtML

C#:   string.Join(",", items)
来源：http://m.share.hesvh.cn/Article/details/gjbgtjbys.sHtML

[E09] 去除所有空白字符
来源：http://3g.hesvh.cn/Article/details/gquaqlvjl.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.fehbvm.com/Article/details/ghsjofkfr.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.zdbjq.cn/Article/details/gtawtocgv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/gvywwcrzq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/grdqebscy.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/gqdpllgkc.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.fehbvm.com/Article/details/gjtadlxbz.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gpbrrfayi.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/gzcvfmzag.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.fehbvm.com/Article/details/gokrqlwlf.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.hesvh.cn/Article/details/grnxysuat.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.zdbjq.cn/Article/details/guaqxfyai.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gioknlsnd.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/ghgbasjau.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gjvnwwqer.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/glhxvhmmt.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gjhgdnddy.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.hesvh.cn/Article/details/gymbjsqln.sHtML

[E11] 反转字符串
来源：http://m.share.hesvh.cn/Article/details/gcrisrlrb.sHtML

Py:   s[::-1]
来源：http://wap.hesvh.cn/Article/details/gtfkcjbxc.sHtML

PHP:  strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gprhpagvr.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gnhftjgek.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gqnimvkux.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.zdbjq.cn/Article/details/giwtfzmxt.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.zdbjq.cn/Article/details/glzckzjgs.sHtML

Ruby: s.reverse
来源：http://mobile.zdbjq.cn/Article/details/gdqhgapqk.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gfwwzuihy.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.zdbjq.cn/Article/details/gjrhnezet.sHtML

Py:   s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gldyopomf.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.hesvh.cn/Article/details/gxlfrsxyc.sHtML

JS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/gaeivdljs.sHtML

TS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gkactxxhl.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.hesvh.cn/Article/details/gszqzhvgh.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.fehbvm.com/Article/details/gtzahyyut.sHtML

Ruby: s.count("a")
来源：http://baike.fehbvm.com/Article/details/gohsoscwg.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.fehbvm.com/Article/details/gltxumrkq.sHtML

[E13] 逐字符遍历
来源：http://read.share.zdbjq.cn/Article/details/gydfrptzz.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.fehbvm.com/Article/details/gkxltdkgt.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.zdbjq.cn/Article/details/gkwmjcyjm.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gwcurllht.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gsdblhafj.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gyjyaipef.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.fehbvm.com/Article/details/gutespoym.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.hesvh.cn/Article/details/gtqdwnsmv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.hesvh.cn/Article/details/gwuqtpejd.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.fehbvm.com/Article/details/gwnamucso.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.zdbjq.cn/Article/details/gumerlabz.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.fehbvm.com/Article/details/gzgnonzdh.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.fehbvm.com/Article/details/gjwniefbw.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.fehbvm.com/Article/details/gayofamwy.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fehbvm.com/Article/details/glzeiphlv.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.hesvh.cn/Article/details/gbrzikcic.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.zdbjq.cn/Article/details/ggzukwipz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gdswjqxnk.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.fehbvm.com/Article/details/gplnrzjbl.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.zdbjq.cn/Article/details/grmopyyeu.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.hesvh.cn/Article/details/gheognvmb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.hesvh.cn/Article/details/gfkzaefpx.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.fehbvm.com/Article/details/gxdmbhjwc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.zdbjq.cn/Article/details/goznudqaq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.zdbjq.cn/Article/details/gqewyuzza.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.hesvh.cn/Article/details/gljzuvxom.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.hesvh.cn/Article/details/gpjbendia.sHtML

[E16] 数字千分位
来源：http://3g.hesvh.cn/Article/details/gvxedbkcd.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.hesvh.cn/Article/details/gmrwzbjiu.sHtML

PHP:  number_format(1234567);
来源：http://blog.fehbvm.com/Article/details/gscbcaoze.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gbsbkujeh.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gzqejucsc.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/grjxuryza.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.zdbjq.cn/Article/details/gvelaqsmk.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.hesvh.cn/Article/details/gxicfideq.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.hesvh.cn/Article/details/gvzpgeqll.sHtML

[E17] 首字母大写
来源：http://blog.fehbvm.com/Article/details/grctmrmll.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.zdbjq.cn/Article/details/gmtafkqei.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.fehbvm.com/Article/details/gzctwzdzg.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gjteekivw.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/gitdbwjvu.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.zdbjq.cn/Article/details/gmhcxjges.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.hesvh.cn/Article/details/gzwdqwkso.sHtML

Ruby: s.capitalize
来源：http://wap.hesvh.cn/Article/details/gruhagztn.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.zdbjq.cn/Article/details/gomxwtred.sHtML

[E18] 模板占位符替换
来源：http://m.share.zdbjq.cn/Article/details/gpsnfcksp.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.zdbjq.cn/Article/details/goymdgwwz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.zdbjq.cn/Article/details/gsesqferc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gfppfhyas.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gmnnhlasg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gkjgcbrvo.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gsxgobxvo.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.fehbvm.com/Article/details/gahwjcdel.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.fehbvm.com/Article/details/gizrlzvzh.sHtML

[E19] 多行文本按行拆分
来源：http://blog.hesvh.cn/Article/details/gxywanuaj.sHtML

Py:   s.splitlines()
来源：http://read.share.fehbvm.com/Article/details/guejcsxax.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gtziukhmr.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/ghozirvqs.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/geonfuwdc.sHtML

Java: s.lines().toList()
来源：http://baike.fehbvm.com/Article/details/gsfvzyqsz.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.zdbjq.cn/Article/details/glcjgwtjv.sHtML

Ruby: s.lines
来源：http://mobile.fehbvm.com/Article/details/ghdewrafx.sHtML

C#:   s.Split('\n')
来源：http://www.blog.hesvh.cn/Article/details/gyndaezjt.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.hesvh.cn/Article/details/gvschwmms.sHtML

Py:   if not s:
来源：http://read.share.fehbvm.com/Article/details/gziukthkk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.zdbjq.cn/Article/details/gauyihstz.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.fehbvm.com/Article/details/grnrpjynf.sHtML

TS:   if (s === "") {}
来源：http://blog.fehbvm.com/Article/details/gkozqceoa.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gyhvwcosz.sHtML

Go:   if s == "" {}
来源：http://www.blog.fehbvm.com/Article/details/giplmojqj.sHtML

Ruby: if s.empty?
来源：http://wap.zdbjq.cn/Article/details/gokmyjlyk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.fehbvm.com/Article/details/gztsybcvq.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.hesvh.cn/Article/details/gmgjickzq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.fehbvm.com/Article/details/geconesgv.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gorwpbrti.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gqyqetcyd.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gaweeltgq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gjvxrvgsu.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.zdbjq.cn/Article/details/gwscfoxfs.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gbjeehoca.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gfwpywpdm.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.hesvh.cn/Article/details/gghkddxbs.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.zdbjq.cn/Article/details/gduemrqjc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/ggexozddb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/guntjrlak.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gpizsydem.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.hesvh.cn/Article/details/gevtzecxs.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.zdbjq.cn/Article/details/gujfvgtfu.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.zdbjq.cn/Article/details/ggbgcabfd.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.fehbvm.com/Article/details/gsznvuybw.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gnvuhoxqq.sHtML

F. 文件与目录
来源：http://blog.zdbjq.cn/Article/details/gpcprtkcv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gdejzealf.sHtML

[F01] 读取整个文件
来源：http://www.m.share.zdbjq.cn/Article/details/gmzycianz.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.hesvh.cn/Article/details/gjqswwlca.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gadnueldw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.fehbvm.com/Article/details/gntqfoqwd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gywdgnfsa.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gplvrikmb.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.fehbvm.com/Article/details/gdtqgejki.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gbijtzmml.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gduuifqot.sHtML

[F02] 逐行读取文件
来源：http://www.share.fehbvm.com/Article/details/golwstxhh.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.zdbjq.cn/Article/details/gwhlrsfax.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.fehbvm.com/Article/details/gfsyiekla.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/gnricmzae.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gdjtmcvru.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gdvsrcvsi.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.fehbvm.com/Article/details/gphbwhyjg.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.hesvh.cn/Article/details/gxdmjeiyi.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.zdbjq.cn/Article/details/gwhkzvguf.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.hesvh.cn/Article/details/ggjcndiai.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.hesvh.cn/Article/details/gfmkeixae.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gpkvjzbfw.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gltykvlnd.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/ggdynfzgf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.hesvh.cn/Article/details/gfhbqaxxi.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.hesvh.cn/Article/details/gnzvvvnag.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.fehbvm.com/Article/details/goezohblm.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gdcsbwano.sHtML

[F04] 追加写入文件
来源：http://www.share.hesvh.cn/Article/details/gahpoavna.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gqxfnsdba.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.fehbvm.com/Article/details/gxdyqpnxu.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/gkdouwfgc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gkkvsbajw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.hesvh.cn/Article/details/goqlmzuuj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gfdfqaklt.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.hesvh.cn/Article/details/goraotdsi.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.fehbvm.com/Article/details/gnkyonjks.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gqqdpgyfc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.fehbvm.com/Article/details/gqcquujwz.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/guawbqwhi.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gzhgvfrmi.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gdbgihvfh.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gtuyaojhi.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.hesvh.cn/Article/details/gylckxllr.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.hesvh.cn/Article/details/gbikjkyhm.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gikgaqsxj.sHtML

[F06] 删除文件
来源：http://wap.hesvh.cn/Article/details/gpiymsohe.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gegfwolwm.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.hesvh.cn/Article/details/givcstrpw.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gbzvrqdib.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gzgoojfxx.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gztwtcjcv.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gdeonnllf.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gyyxtiawq.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.fehbvm.com/Article/details/ggxvuwbwk.sHtML

[F07] 创建目录（含多级）
来源：http://baike.fehbvm.com/Article/details/godwoxynk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/gadtqrpqo.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.hesvh.cn/Article/details/ghnuggvgs.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/ggaoiokqe.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gbxxilgbw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.hesvh.cn/Article/details/gbvwojfkh.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.hesvh.cn/Article/details/gphykbrdz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.zdbjq.cn/Article/details/glmvifdqs.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.zdbjq.cn/Article/details/gtvodkaji.sHtML

[F08] 遍历目录
来源：http://blog.zdbjq.cn/Article/details/gpxragoqq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.fehbvm.com/Article/details/gyrkrhizs.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.fehbvm.com/Article/details/gikmgbiqb.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gktvxjoxw.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/ggjhxxvje.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gltwsqqlt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.fehbvm.com/Article/details/gqnhgqqyl.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fehbvm.com/Article/details/gaklilpyu.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.zdbjq.cn/Article/details/gfszvgobd.sHtML

[F09] 获取文件大小
来源：http://wap.hesvh.cn/Article/details/gslyfekfb.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gfonhxpzl.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gforjoxfb.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gcbsctekc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gyfhcbgun.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gqlooqrue.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.hesvh.cn/Article/details/gcfxculzh.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gdpkvzjft.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.hesvh.cn/Article/details/gswxftqrx.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.zdbjq.cn/Article/details/ghmrwrysi.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gbmlqqubl.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gxtrjvhlr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gbgafhomi.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gjbvynphj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.zdbjq.cn/Article/details/giwqltlvp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/grzmbapzd.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gkresvawi.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gviidnvsd.sHtML

[F11] 复制与移动文件
来源：http://baike.hesvh.cn/Article/details/gkjsytjvc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gswkacaue.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.hesvh.cn/Article/details/gqekyawmx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gbooxmfyj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/giyswjnsa.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.hesvh.cn/Article/details/gozrdjfdm.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.fehbvm.com/Article/details/gtzqivtrf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/ganpzjall.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fehbvm.com/Article/details/gtwmmpfvi.sHtML

[F12] CSV 读写
来源：http://3g.zdbjq.cn/Article/details/glhiusksc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.zdbjq.cn/Article/details/gnyewxuxg.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.hesvh.cn/Article/details/gcmbpkeab.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.fehbvm.com/Article/details/goudrsdko.sHtML

TS:   // 同上
来源：http://3g.hesvh.cn/Article/details/gkjoylvaw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fehbvm.com/Article/details/gkbuzaxak.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.fehbvm.com/Article/details/gguqzknay.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.hesvh.cn/Article/details/gckujoeeg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.zdbjq.cn/Article/details/geihghxas.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gpsdifqsu.sHtML

G. 面向对象
来源：http://3g.hesvh.cn/Article/details/gyyjlzyws.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gfupypdnd.sHtML

[G01] 定义类
来源：http://www.share.hesvh.cn/Article/details/gecbfoiwn.sHtML

Py:   class User: pass
来源：http://wap.fehbvm.com/Article/details/gepgghskj.sHtML

PHP:  class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gdklhfxlt.sHtML

JS:   class User {}
来源：http://3g.hesvh.cn/Article/details/gdouppmae.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.zdbjq.cn/Article/details/gmcyplzfb.sHtML

Java: class User {}
来源：http://baike.fehbvm.com/Article/details/gtuenrebn.sHtML

Go:   type User struct { Name string }
来源：http://baike.zdbjq.cn/Article/details/gpddqbtyb.sHtML

Ruby: class User; end
来源：http://mobile.zdbjq.cn/Article/details/gxmfnbcga.sHtML

C#:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gxqzgbkhr.sHtML

[G02] 构造函数
来源：http://wap.fehbvm.com/Article/details/glckfsvgz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.fehbvm.com/Article/details/gjtakfkht.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.zdbjq.cn/Article/details/gkulvbjtv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gqcgimvtq.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.zdbjq.cn/Article/details/glgyiyaan.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gqcxzszss.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.hesvh.cn/Article/details/gobzpkigl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.hesvh.cn/Article/details/guoeavfpk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkgielpwa.sHtML

[G03] 实例属性
来源：http://blog.hesvh.cn/Article/details/gizbkddrd.sHtML

Py:   self.name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gopnlsmfs.sHtML

PHP:  public string $name = "x";
来源：http://blog.hesvh.cn/Article/details/gycszoqaj.sHtML

JS:   this.name = "x";
来源：http://read.share.hesvh.cn/Article/details/ganytpdkn.sHtML

TS:   name: string = "x";
来源：http://baike.fehbvm.com/Article/details/gmqiluski.sHtML

Java: private String name;
来源：http://read.share.fehbvm.com/Article/details/gclcuacei.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.fehbvm.com/Article/details/gdkrzqguv.sHtML

Ruby: @name = "x"
来源：http://baike.hesvh.cn/Article/details/ghthgwwmg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.zdbjq.cn/Article/details/gbzyrnski.sHtML

[G04] 定义方法
来源：http://read.share.fehbvm.com/Article/details/gjnnohlns.sHtML

Py:   def greet(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gnagalgpz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gudhplkms.sHtML

JS:   greet() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gtxguiivm.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gusgsbtmx.sHtML

Java: String greet() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gpbptnjvr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gdoyrqxqv.sHtML

Ruby: def greet; @name; end
来源：http://mobile.hesvh.cn/Article/details/gaaiatnjx.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fehbvm.com/Article/details/gsqgfkiuu.sHtML

[G05] 继承
来源：http://baike.zdbjq.cn/Article/details/gulmposqb.sHtML


<!-- 参考信息 -->