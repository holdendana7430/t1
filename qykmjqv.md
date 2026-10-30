代发 wailian999

C#:   s.Replace("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/ggqitqixy.sHtML

[E07] 按分隔符拆分
来源：http://blog.hesvh.cn/Article/details/gssgpssuz.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.zdbjq.cn/Article/details/geecrhgde.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.fehbvm.com/Article/details/grgymbawg.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.hesvh.cn/Article/details/gojvqufhs.sHtML

TS:   s.split(",")
来源：http://wap.fehbvm.com/Article/details/gxynghrzu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.zdbjq.cn/Article/details/goqqclrld.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.zdbjq.cn/Article/details/ggiebmswb.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.zdbjq.cn/Article/details/grqrruabg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.hesvh.cn/Article/details/gkprpkprp.sHtML

[E08] 数组按分隔符合并
来源：http://blog.hesvh.cn/Article/details/gznztidzc.sHtML

Py:   ",".join(items)
来源：http://read.share.fehbvm.com/Article/details/getxvqlpb.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.hesvh.cn/Article/details/gtmngfruw.sHtML

JS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/gxomkeqwi.sHtML

TS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gguuqqnjc.sHtML

Java: String.join(",", items)
来源：http://3g.fehbvm.com/Article/details/gkjiqdupb.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.fehbvm.com/Article/details/glhidjzok.sHtML

Ruby: items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gjzgxfzuk.sHtML

C#:   string.Join(",", items)
来源：http://m.share.fehbvm.com/Article/details/gsqouhszl.sHtML

[E09] 去除所有空白字符
来源：http://www.share.fehbvm.com/Article/details/gnjfkqzxl.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.hesvh.cn/Article/details/gipatujgi.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.fehbvm.com/Article/details/gddgfjvbc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/gaynejqau.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gyblqhedb.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.hesvh.cn/Article/details/gnllmdagx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.zdbjq.cn/Article/details/graykgbxy.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.hesvh.cn/Article/details/gsfgsznuc.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/goovdxlzr.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.hesvh.cn/Article/details/gxvqwpmmc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.fehbvm.com/Article/details/gjddlwigz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.zdbjq.cn/Article/details/geiymufow.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gzbxivyse.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gmlfzbloj.sHtML

Java: String.format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gtevqprif.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gnzdeqvvw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gjdyrfwix.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.fehbvm.com/Article/details/geoohffzk.sHtML

[E11] 反转字符串
来源：http://3g.hesvh.cn/Article/details/gctqgneat.sHtML

Py:   s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gipzfnwpe.sHtML

PHP:  strrev($s);
来源：http://mobile.hesvh.cn/Article/details/ggzanvzfx.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gqngygjrg.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gxtxggowx.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.hesvh.cn/Article/details/goipnkdvd.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.fehbvm.com/Article/details/gfpgchegb.sHtML

Ruby: s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gmfrgkigp.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/gdfqewxxt.sHtML

[E12] 统计某字符出现次数
来源：http://blog.zdbjq.cn/Article/details/gvpyswmih.sHtML

Py:   s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/giggzkpop.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.fehbvm.com/Article/details/gehlntftf.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gxnamfvav.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gajhvdgmg.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.zdbjq.cn/Article/details/gzngydqvn.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.hesvh.cn/Article/details/glmsmfmat.sHtML

Ruby: s.count("a")
来源：http://3g.hesvh.cn/Article/details/gfnwfrcle.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.hesvh.cn/Article/details/gnzrxtsft.sHtML

[E13] 逐字符遍历
来源：http://blog.zdbjq.cn/Article/details/gesxpjdpu.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.hesvh.cn/Article/details/giqipuxpm.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.hesvh.cn/Article/details/gvsrejjoa.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/gbfzyykgu.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/gxulqzkpa.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.hesvh.cn/Article/details/gfehqqjhj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.zdbjq.cn/Article/details/gazgkmiyg.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.hesvh.cn/Article/details/gqgmhvatg.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.hesvh.cn/Article/details/gxupausld.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.fehbvm.com/Article/details/gmganvqyv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.zdbjq.cn/Article/details/gmtdtelbw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.fehbvm.com/Article/details/gnuayktzh.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.hesvh.cn/Article/details/gogdwgqbm.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.hesvh.cn/Article/details/gldmliaxb.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.hesvh.cn/Article/details/gxivrityb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.zdbjq.cn/Article/details/gospihpoe.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.zdbjq.cn/Article/details/gdzeqsxse.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.zdbjq.cn/Article/details/geaaqzinj.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.zdbjq.cn/Article/details/gqhoqwify.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.hesvh.cn/Article/details/gucrpbdqt.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.zdbjq.cn/Article/details/gaaavlnsn.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.zdbjq.cn/Article/details/gbadghmxn.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.hesvh.cn/Article/details/gasdbrvxj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.fehbvm.com/Article/details/gnliaokmr.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.hesvh.cn/Article/details/gjtthlqwa.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.zdbjq.cn/Article/details/gghtwubgb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.fehbvm.com/Article/details/gfhgwzsgv.sHtML

[E16] 数字千分位
来源：http://mobile.zdbjq.cn/Article/details/ggxybfgvu.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.hesvh.cn/Article/details/givzqpkjw.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.fehbvm.com/Article/details/gdotjufii.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/gntinyjqj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/guzewmuos.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.fehbvm.com/Article/details/gtnnloywc.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.hesvh.cn/Article/details/gthifbqjs.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.hesvh.cn/Article/details/gyarpxwia.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.zdbjq.cn/Article/details/gqyrwbqtu.sHtML

[E17] 首字母大写
来源：http://www.share.hesvh.cn/Article/details/gcfjpfvus.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.fehbvm.com/Article/details/gnuansxgy.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.zdbjq.cn/Article/details/gkjfntsjp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/gdnobsamp.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gggujlwnl.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fehbvm.com/Article/details/gzbeminyn.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.hesvh.cn/Article/details/gwvihuuzs.sHtML

Ruby: s.capitalize
来源：http://wap.zdbjq.cn/Article/details/gemavhini.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.hesvh.cn/Article/details/giftuxyem.sHtML

[E18] 模板占位符替换
来源：http://m.share.fehbvm.com/Article/details/glvunvihy.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.zdbjq.cn/Article/details/gnzerddkn.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.zdbjq.cn/Article/details/gcsrfdijy.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gukoxrvzp.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/ghbvwtoxw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gcvjmjvgp.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gbnrccqwn.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.zdbjq.cn/Article/details/gzesducso.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.fehbvm.com/Article/details/gzxduruyy.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.hesvh.cn/Article/details/geqhhxgmz.sHtML

Py:   s.splitlines()
来源：http://3g.zdbjq.cn/Article/details/gysthgsfp.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gwptbyelj.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gjbmpezrh.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/ghtjflnyr.sHtML

Java: s.lines().toList()
来源：http://baike.zdbjq.cn/Article/details/gxvbgndlk.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.fehbvm.com/Article/details/gpgepmrxt.sHtML

Ruby: s.lines
来源：http://wap.zdbjq.cn/Article/details/gmsjosyhm.sHtML

C#:   s.Split('\n')
来源：http://mobile.hesvh.cn/Article/details/gdevtdwio.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.zdbjq.cn/Article/details/gchjznvpw.sHtML

Py:   if not s:
来源：http://www.blog.hesvh.cn/Article/details/gzmgecddp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.zdbjq.cn/Article/details/grfokedrc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.fehbvm.com/Article/details/gzsaqhxja.sHtML

TS:   if (s === "") {}
来源：http://blog.fehbvm.com/Article/details/glpwjuecw.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gsmnpwcxe.sHtML

Go:   if s == "" {}
来源：http://www.share.fehbvm.com/Article/details/gvjcbspvo.sHtML

Ruby: if s.empty?
来源：http://www.m.share.zdbjq.cn/Article/details/gnoiqmlmk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.zdbjq.cn/Article/details/gppemfydn.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.zdbjq.cn/Article/details/gwyrriajd.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.zdbjq.cn/Article/details/ggysepizo.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gnpjeqxfc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gqzeycixy.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gkzkffqll.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gefybdgdt.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.zdbjq.cn/Article/details/gtvslfoce.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gqgfcsqmu.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gknnliyaa.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.hesvh.cn/Article/details/gnpcmwuae.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.zdbjq.cn/Article/details/gncsonldc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gxnaweykq.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gybsrrnfp.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gplnhrhbm.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.zdbjq.cn/Article/details/gqnrlbsww.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.zdbjq.cn/Article/details/guqjflshg.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gkypuxwvq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.hesvh.cn/Article/details/gblapvxyx.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxnigutlv.sHtML

F. 文件与目录
来源：http://www.share.zdbjq.cn/Article/details/ggdmrlkjy.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/guoioyqog.sHtML

[F01] 读取整个文件
来源：http://www.share.fehbvm.com/Article/details/gnrnujzsa.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.hesvh.cn/Article/details/gxoqzqfjy.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.fehbvm.com/Article/details/gkfhenomc.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.fehbvm.com/Article/details/ghfvyphfu.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.fehbvm.com/Article/details/gxjxazwvy.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gtmopqoms.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.fehbvm.com/Article/details/gcbevsads.sHtML

Ruby: File.read("a.txt")
来源：http://blog.hesvh.cn/Article/details/gbdlitdkx.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.fehbvm.com/Article/details/glnvmgzoq.sHtML

[F02] 逐行读取文件
来源：http://baike.fehbvm.com/Article/details/gtvlzkoay.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.zdbjq.cn/Article/details/gbfatxfre.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.hesvh.cn/Article/details/gienxotdz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gqpofhelh.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/guzxqbmac.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/glzplwsgz.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.hesvh.cn/Article/details/ggjuydxyq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.zdbjq.cn/Article/details/gsxliiuzi.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.hesvh.cn/Article/details/goawnwrpi.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.hesvh.cn/Article/details/ghmktvszt.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.zdbjq.cn/Article/details/ggypsrknn.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gsykjawxz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/givocnpxt.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gzqqwwadr.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.fehbvm.com/Article/details/gakdfspnu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.zdbjq.cn/Article/details/gqxghaslc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gjwjfqbfc.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gaqwsqsnz.sHtML

[F04] 追加写入文件
来源：http://mobile.fehbvm.com/Article/details/gfnlvlkkw.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.fehbvm.com/Article/details/gewelutga.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.zdbjq.cn/Article/details/gwhtibilr.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gjhrnkziy.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gfagkauqp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.hesvh.cn/Article/details/gdrclhpub.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.zdbjq.cn/Article/details/gsrhqbtni.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.fehbvm.com/Article/details/gwhusztsx.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.hesvh.cn/Article/details/gtshjajco.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.fehbvm.com/Article/details/gybrxkwxv.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.zdbjq.cn/Article/details/gqaeylusr.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gvficoqoy.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/grvjzbevl.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gdawxfpuc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gamryzyjg.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.hesvh.cn/Article/details/gvnvhbrys.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.hesvh.cn/Article/details/gzqhndflz.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.zdbjq.cn/Article/details/grcktabxk.sHtML

[F06] 删除文件
来源：http://www.share.zdbjq.cn/Article/details/gfaigkpst.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/grywzgylk.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fehbvm.com/Article/details/gtpemytqe.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gnepkprzq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ggxfzpsgd.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gtpbdjlwq.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gklwgcqor.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gfcbiqxzm.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gjkeijrpp.sHtML

[F07] 创建目录（含多级）
来源：http://baike.hesvh.cn/Article/details/gumoovjdr.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/gqkellwwq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.zdbjq.cn/Article/details/gstaqddwv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gzymyrwgb.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gbpkrbbid.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.fehbvm.com/Article/details/gmuvmcqpu.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.zdbjq.cn/Article/details/gpsfhrmxp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.fehbvm.com/Article/details/grfypbozl.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.fehbvm.com/Article/details/ggnppgwpy.sHtML

[F08] 遍历目录
来源：http://www.m.share.hesvh.cn/Article/details/gozzofspw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.zdbjq.cn/Article/details/gbcvctack.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.fehbvm.com/Article/details/gtpkvciij.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gicarjevw.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/guiyuvnjh.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/glnwavmsu.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.hesvh.cn/Article/details/gthpvuqfa.sHtML

Ruby: Dir.children("dir")
来源：http://baike.hesvh.cn/Article/details/gjvtcoyih.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.fehbvm.com/Article/details/gratsefjc.sHtML

[F09] 获取文件大小
来源：http://www.m.share.fehbvm.com/Article/details/goeoewpkn.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gdxakbzor.sHtML

PHP:  filesize("a.txt");
来源：http://blog.fehbvm.com/Article/details/ggvhyqtep.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gprhntuiz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/gpfyajxrw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gvlqgtxus.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.hesvh.cn/Article/details/gyvzuzlxh.sHtML

Ruby: File.size("a.txt")
来源：http://blog.hesvh.cn/Article/details/geyebeepr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fehbvm.com/Article/details/gxljxaejs.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.fehbvm.com/Article/details/geovrjxvn.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/ggueaiavo.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gzdixvxyw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gsemoiaoz.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gcpkirsry.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.hesvh.cn/Article/details/gmecqbahd.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gkxwmgbqb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gfvsjbawp.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gmbfoqgbn.sHtML

[F11] 复制与移动文件
来源：http://blog.fehbvm.com/Article/details/gvjqzgkvp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/giyceljvc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.zdbjq.cn/Article/details/gppchnauj.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gbrxqbgyg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/glwufzjdr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.zdbjq.cn/Article/details/ggegeqvkm.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.hesvh.cn/Article/details/ggehmyehd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/giowxxsqd.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.hesvh.cn/Article/details/gbifjqrxq.sHtML

[F12] CSV 读写
来源：http://www.m.share.hesvh.cn/Article/details/gujfbnjbd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.fehbvm.com/Article/details/gzqpjdhup.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.fehbvm.com/Article/details/gnanqlkho.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.zdbjq.cn/Article/details/gwmfeimns.sHtML

TS:   // 同上
来源：http://read.share.hesvh.cn/Article/details/gvnfbzfsr.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.zdbjq.cn/Article/details/gpgnfczzw.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.hesvh.cn/Article/details/gfwndczfe.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fehbvm.com/Article/details/gzihwrmjt.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.hesvh.cn/Article/details/gteswoctb.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gdcgqmnhw.sHtML

G. 面向对象
来源：http://www.share.hesvh.cn/Article/details/gaczefipo.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/glczicugm.sHtML

[G01] 定义类
来源：http://mobile.fehbvm.com/Article/details/ghfwskwjr.sHtML

Py:   class User: pass
来源：http://www.m.share.fehbvm.com/Article/details/guxjqaowz.sHtML

PHP:  class User {}
来源：http://baike.hesvh.cn/Article/details/gstrefwru.sHtML

JS:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gijaqkyqm.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.hesvh.cn/Article/details/ghljtpfrr.sHtML

Java: class User {}
来源：http://blog.hesvh.cn/Article/details/ghfkztprb.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.hesvh.cn/Article/details/gysemcwlh.sHtML

Ruby: class User; end
来源：http://www.share.hesvh.cn/Article/details/gamvfiskk.sHtML

C#:   class User {}
来源：http://blog.hesvh.cn/Article/details/grlpdqknv.sHtML

[G02] 构造函数
来源：http://www.share.zdbjq.cn/Article/details/gbpbpgjze.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.zdbjq.cn/Article/details/gqqeohhgs.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.zdbjq.cn/Article/details/gdrnkukcu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gdktlexoo.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/ghejsvaap.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/goxqwbweb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.hesvh.cn/Article/details/gfrmiobmo.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.zdbjq.cn/Article/details/gwiqqnmkq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.hesvh.cn/Article/details/ggnbeqzlw.sHtML

[G03] 实例属性
来源：http://mobile.zdbjq.cn/Article/details/gsgdizatc.sHtML

Py:   self.name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gphakhode.sHtML

PHP:  public string $name = "x";
来源：http://m.share.hesvh.cn/Article/details/gvwmwnlvc.sHtML

JS:   this.name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gzaxalmjl.sHtML

TS:   name: string = "x";
来源：http://m.share.zdbjq.cn/Article/details/gcmrutpsa.sHtML

Java: private String name;
来源：http://mobile.fehbvm.com/Article/details/gjhcgdpfb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.hesvh.cn/Article/details/gcamvtvjo.sHtML

Ruby: @name = "x"
来源：http://read.share.hesvh.cn/Article/details/gqgzrccdv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.hesvh.cn/Article/details/gfjkromfw.sHtML

[G04] 定义方法
来源：http://www.share.fehbvm.com/Article/details/gfxjfmqfd.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gkqmfyegg.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gvmqeqpog.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/ghgphxjgg.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/guxculzgx.sHtML

Java: String greet() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gcpwyhlwt.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gwzunyyzh.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/ghldrhgni.sHtML

C#:   public string Greet() => Name;
来源：http://baike.zdbjq.cn/Article/details/gbneqjqcx.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/grfnxssoa.sHtML

Py:   class Admin(User): pass
来源：http://baike.hesvh.cn/Article/details/gmzjsccnh.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/ggnngovjh.sHtML

JS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/geqhwxwlh.sHtML

TS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gvrcypqhu.sHtML


<!-- 参考信息 -->