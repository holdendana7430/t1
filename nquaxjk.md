代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.zdbjq.cn/Article/details/gxjgjbgxi.sHtML

TS:   s.split(",")
来源：http://read.share.hesvh.cn/Article/details/gglyouyrc.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.fehbvm.com/Article/details/gtfoqkmrw.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.fehbvm.com/Article/details/gqzdcxxkd.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.zdbjq.cn/Article/details/guwnwmmzm.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.fehbvm.com/Article/details/gntlltrsc.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.fehbvm.com/Article/details/gqniodekk.sHtML

Py:   ",".join(items)
来源：http://read.share.zdbjq.cn/Article/details/gyinkujkl.sHtML

PHP:  implode(",", $items);
来源：http://www.share.hesvh.cn/Article/details/gsulfbmku.sHtML

JS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gwakncqzf.sHtML

TS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gnzdolrhp.sHtML

Java: String.join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gibpsxvmj.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.zdbjq.cn/Article/details/geqxwsqbw.sHtML

Ruby: items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gfqbzokqb.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/gagjvkrfq.sHtML

[E09] 去除所有空白字符
来源：http://read.share.zdbjq.cn/Article/details/gmvhteiuz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.hesvh.cn/Article/details/gjgzuzusk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.hesvh.cn/Article/details/gtmywcidx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gthsulfdf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/gclgweidk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.hesvh.cn/Article/details/gskksssqw.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.hesvh.cn/Article/details/gkvtbrnnr.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.fehbvm.com/Article/details/gahsiyinr.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.fehbvm.com/Article/details/gxxligvyu.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.zdbjq.cn/Article/details/guikofkax.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gyivtznli.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.hesvh.cn/Article/details/gcbtwiada.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gwunjmxci.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gebxdbmfr.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gnpyvshzx.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gjgupsebh.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gfmnrzkyx.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.fehbvm.com/Article/details/gwlbkjlks.sHtML

[E11] 反转字符串
来源：http://read.share.hesvh.cn/Article/details/gjmhebgem.sHtML

Py:   s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/gluyvavxq.sHtML

PHP:  strrev($s);
来源：http://www.share.fehbvm.com/Article/details/glbiioxqe.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gqvolxlkd.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gcvjbnlkg.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.hesvh.cn/Article/details/gchqbwuyj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.fehbvm.com/Article/details/gongaveya.sHtML

Ruby: s.reverse
来源：http://baike.fehbvm.com/Article/details/gdugoyzci.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/gnktsvufm.sHtML

[E12] 统计某字符出现次数
来源：http://baike.hesvh.cn/Article/details/goieaudcg.sHtML

Py:   s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/gpgeluhqc.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.zdbjq.cn/Article/details/gsyltgpok.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/gksraalli.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/gtmthtmuz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.zdbjq.cn/Article/details/gpiijatxr.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.hesvh.cn/Article/details/gluxsebyj.sHtML

Ruby: s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/gbdmhxhnb.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.hesvh.cn/Article/details/gmnqtcluc.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.hesvh.cn/Article/details/gonkefdkf.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.fehbvm.com/Article/details/gwdgpwjuh.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.fehbvm.com/Article/details/gqeqdkbjk.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gfvefceyo.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/gtqlvtsiy.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.fehbvm.com/Article/details/guzdxdnmo.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.zdbjq.cn/Article/details/gtubksssh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.zdbjq.cn/Article/details/guonionct.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.zdbjq.cn/Article/details/guvmolqvu.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.hesvh.cn/Article/details/guccxfyrb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.hesvh.cn/Article/details/gndqtfbpx.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.zdbjq.cn/Article/details/gcunbxfbt.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.zdbjq.cn/Article/details/gqfaxajoo.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.fehbvm.com/Article/details/gtmoqahou.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gjgbiewus.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.fehbvm.com/Article/details/gbqrgpoqk.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.hesvh.cn/Article/details/gmwgqyhet.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gyplbjnpr.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.fehbvm.com/Article/details/glscaeowh.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.zdbjq.cn/Article/details/gncdhqvic.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fehbvm.com/Article/details/gdkjdcqjc.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.hesvh.cn/Article/details/gbysyczpv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.fehbvm.com/Article/details/gqvfwjdog.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.fehbvm.com/Article/details/gwruqfkwi.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.zdbjq.cn/Article/details/guftijiya.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.hesvh.cn/Article/details/gdhgdgbqt.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.zdbjq.cn/Article/details/gfggbawlt.sHtML

[E16] 数字千分位
来源：http://www.blog.fehbvm.com/Article/details/gmsjxeftx.sHtML

Py:   f"{1234567:,}"
来源：http://3g.zdbjq.cn/Article/details/gmyqtuhnq.sHtML

PHP:  number_format(1234567);
来源：http://blog.hesvh.cn/Article/details/gidxvlfyb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gaqmuybvl.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gicklfujz.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.zdbjq.cn/Article/details/gyuazzdso.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.zdbjq.cn/Article/details/gnrxdxxkv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.fehbvm.com/Article/details/gkgjofenl.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.hesvh.cn/Article/details/gjrqasosz.sHtML

[E17] 首字母大写
来源：http://3g.hesvh.cn/Article/details/gryxjnint.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.hesvh.cn/Article/details/geemrirzy.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fehbvm.com/Article/details/gisqcpomt.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/gxeruthnk.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/gsmjiauol.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.hesvh.cn/Article/details/giordhxhr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.zdbjq.cn/Article/details/gpcgziadx.sHtML

Ruby: s.capitalize
来源：http://baike.hesvh.cn/Article/details/gyxhlxtew.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.fehbvm.com/Article/details/gpjurbfkh.sHtML

[E18] 模板占位符替换
来源：http://m.share.fehbvm.com/Article/details/gzfprloka.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.zdbjq.cn/Article/details/gwndhjhph.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.fehbvm.com/Article/details/gsxqezsnr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/ghiyxrina.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/ghgrzwfbd.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gmrfgsslb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gzluwhpvv.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.fehbvm.com/Article/details/ggubknyxw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.hesvh.cn/Article/details/gpqlrojso.sHtML

[E19] 多行文本按行拆分
来源：http://wap.fehbvm.com/Article/details/gqmdtlgsw.sHtML

Py:   s.splitlines()
来源：http://m.share.hesvh.cn/Article/details/gedzknhas.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.zdbjq.cn/Article/details/gadwrvxyy.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gfkhhsujc.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/gzrmuhbzw.sHtML

Java: s.lines().toList()
来源：http://3g.zdbjq.cn/Article/details/gkrghqvjd.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.zdbjq.cn/Article/details/gncqeiret.sHtML

Ruby: s.lines
来源：http://baike.hesvh.cn/Article/details/gvaozlauf.sHtML

C#:   s.Split('\n')
来源：http://blog.hesvh.cn/Article/details/gnadbznsx.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.zdbjq.cn/Article/details/gaooshbll.sHtML

Py:   if not s:
来源：http://m.share.zdbjq.cn/Article/details/glurrvolu.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.zdbjq.cn/Article/details/gwtgeeehu.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fehbvm.com/Article/details/ghnnofdye.sHtML

TS:   if (s === "") {}
来源：http://read.share.hesvh.cn/Article/details/gwfyrknvq.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gdidygnbn.sHtML

Go:   if s == "" {}
来源：http://3g.hesvh.cn/Article/details/gyojtiecd.sHtML

Ruby: if s.empty?
来源：http://blog.hesvh.cn/Article/details/gbkrxsjrt.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.hesvh.cn/Article/details/gjbwaazdj.sHtML

[E21] 超长截断加省略号
来源：http://blog.fehbvm.com/Article/details/gebtfchlw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fehbvm.com/Article/details/gyvkwypnb.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gmwojttct.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gdwzzpelr.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gsgyxusbh.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gdmwxdjvi.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.fehbvm.com/Article/details/gppwywjyf.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gxaokckfn.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gguppsdpy.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.fehbvm.com/Article/details/gmbdxtnaw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.fehbvm.com/Article/details/gexrocqpg.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/golllmtge.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/ggggboeei.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/gwqletwnp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.hesvh.cn/Article/details/gwupacibw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.fehbvm.com/Article/details/guavqlsea.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gkrtlhuhn.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.zdbjq.cn/Article/details/gzewstqex.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gtnaozfli.sHtML

F. 文件与目录
来源：http://www.share.hesvh.cn/Article/details/gilhqomoo.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxcykrxkh.sHtML

[F01] 读取整个文件
来源：http://read.share.zdbjq.cn/Article/details/glnrcqwdb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.zdbjq.cn/Article/details/gdrogwuzv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gegeswvmk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.zdbjq.cn/Article/details/grxhysrod.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gqnylfcko.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gbtiqagat.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.zdbjq.cn/Article/details/gnjqsscqf.sHtML

Ruby: File.read("a.txt")
来源：http://3g.fehbvm.com/Article/details/gwksfcbst.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gajnktfes.sHtML

[F02] 逐行读取文件
来源：http://blog.zdbjq.cn/Article/details/gtlzfousg.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.hesvh.cn/Article/details/ghbaerrnt.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.fehbvm.com/Article/details/gjbauclzq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gultqptya.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gmclvzori.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/genyqxlhz.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.zdbjq.cn/Article/details/ggsedvgge.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.hesvh.cn/Article/details/gzzshwfcp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.hesvh.cn/Article/details/gugcgxfcy.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.zdbjq.cn/Article/details/gtbotrtyt.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.zdbjq.cn/Article/details/gcdvgzujs.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/gbbasorgu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gabuyvoxu.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/ggirvsffa.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.zdbjq.cn/Article/details/gdxylcbfb.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.hesvh.cn/Article/details/gryjjtcvh.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.hesvh.cn/Article/details/gihefrzoj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gmonmpbtu.sHtML

[F04] 追加写入文件
来源：http://read.share.zdbjq.cn/Article/details/gfyhobcrq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fehbvm.com/Article/details/grxhuebwm.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.fehbvm.com/Article/details/gugduirov.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/getjrgknn.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/gwiufipgl.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.hesvh.cn/Article/details/gmgimqffh.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.fehbvm.com/Article/details/gbsafumoe.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.fehbvm.com/Article/details/gkwdqkyoc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.zdbjq.cn/Article/details/gckpaktld.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.hesvh.cn/Article/details/gyhsdacpu.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.hesvh.cn/Article/details/grogtqioa.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fehbvm.com/Article/details/gawodxbju.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gdcmzsqrs.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gcbfqidyd.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/ggltdsrae.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.fehbvm.com/Article/details/gugursaeo.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gzptrhmgy.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gvbbsyvos.sHtML

[F06] 删除文件
来源：http://www.m.share.hesvh.cn/Article/details/gdagqytrp.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gblnqdvko.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gxnzcnwhv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/ggjrhwrsm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gwkmxrirt.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gikapxswd.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gkqmnfdut.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gzsfguxag.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gapzbbdvt.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.hesvh.cn/Article/details/gptpwafsv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gihssbmes.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.fehbvm.com/Article/details/ggfoxhlgj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gwsmjvuuv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/gagbuobtk.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.zdbjq.cn/Article/details/gcplsadpe.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.hesvh.cn/Article/details/glzajqrww.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.hesvh.cn/Article/details/gaczjveju.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.zdbjq.cn/Article/details/gqkynhdxz.sHtML

[F08] 遍历目录
来源：http://www.share.fehbvm.com/Article/details/gwfyoepfz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.fehbvm.com/Article/details/ghxedgghq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fehbvm.com/Article/details/gaavbzjle.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/ganwzvrdr.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gautbqdem.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gimkeuxxx.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.fehbvm.com/Article/details/gxbttjgca.sHtML

Ruby: Dir.children("dir")
来源：http://blog.hesvh.cn/Article/details/gojyhmkcd.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.zdbjq.cn/Article/details/gyntwtcmx.sHtML

[F09] 获取文件大小
来源：http://mobile.hesvh.cn/Article/details/gqijrwrnh.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.hesvh.cn/Article/details/grlkcqkrt.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gfvkfydkh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gpqhotqxj.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gyjfntfrx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gicuyugkv.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.fehbvm.com/Article/details/gxaaiqzwx.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gzjuxbxer.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.hesvh.cn/Article/details/gkgwwuxoj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.fehbvm.com/Article/details/glpyzrnrw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gfkzjahgb.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gwydqcssd.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gxdawybxy.sHtML

TS:   path.extname("a.txt")
来源：http://baike.hesvh.cn/Article/details/gmqdxvall.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.fehbvm.com/Article/details/gbufisdha.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/ggosmjodo.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gpzamxopd.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gdtqsmerw.sHtML

[F11] 复制与移动文件
来源：http://wap.fehbvm.com/Article/details/gslsvrqvg.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gyckomyux.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.hesvh.cn/Article/details/gdvofyluo.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gauyrsapu.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/glckiqwlm.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.fehbvm.com/Article/details/gxrdadato.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.zdbjq.cn/Article/details/gvzhiwtho.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/ggkytploy.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.fehbvm.com/Article/details/gjgtdlcai.sHtML

[F12] CSV 读写
来源：http://mobile.fehbvm.com/Article/details/girmtfsat.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.fehbvm.com/Article/details/gfhvtnjeb.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.hesvh.cn/Article/details/gjuvqipiw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.hesvh.cn/Article/details/ggdqbrlcq.sHtML

TS:   // 同上
来源：http://blog.hesvh.cn/Article/details/gxrlcyvok.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.hesvh.cn/Article/details/gbsixheqd.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.hesvh.cn/Article/details/gnxnipead.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.hesvh.cn/Article/details/gkgdlxawh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fehbvm.com/Article/details/gnjlpyaif.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gabxexvul.sHtML

G. 面向对象
来源：http://www.blog.fehbvm.com/Article/details/gccdrtacz.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/guwfguvxm.sHtML

[G01] 定义类
来源：http://blog.zdbjq.cn/Article/details/ghyfeyrtd.sHtML

Py:   class User: pass
来源：http://mobile.zdbjq.cn/Article/details/gighlxztb.sHtML

PHP:  class User {}
来源：http://www.blog.fehbvm.com/Article/details/goaeriuzi.sHtML

JS:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gbtzjhvtj.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.hesvh.cn/Article/details/ggmrrvxjm.sHtML

Java: class User {}
来源：http://3g.fehbvm.com/Article/details/geddmedrs.sHtML

Go:   type User struct { Name string }
来源：http://blog.hesvh.cn/Article/details/gpvetafge.sHtML

Ruby: class User; end
来源：http://blog.hesvh.cn/Article/details/gpdbcdqlu.sHtML

C#:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gowvyised.sHtML

[G02] 构造函数
来源：http://www.blog.fehbvm.com/Article/details/gsknlbtdh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.hesvh.cn/Article/details/gihgdxfar.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.fehbvm.com/Article/details/ggfrnyooc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/ggmktwxwh.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.hesvh.cn/Article/details/glyzkwnah.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gqhekecew.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.zdbjq.cn/Article/details/gvobznnmu.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.hesvh.cn/Article/details/gfwmeeaqs.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.fehbvm.com/Article/details/goxbtxiyh.sHtML

[G03] 实例属性
来源：http://blog.hesvh.cn/Article/details/gjixrclkl.sHtML

Py:   self.name = "x"
来源：http://baike.hesvh.cn/Article/details/gcdsdaphr.sHtML

PHP:  public string $name = "x";
来源：http://blog.fehbvm.com/Article/details/gsvlqlwsl.sHtML

JS:   this.name = "x";
来源：http://baike.hesvh.cn/Article/details/gfwzvsxti.sHtML

TS:   name: string = "x";
来源：http://baike.hesvh.cn/Article/details/grcicfudn.sHtML

Java: private String name;
来源：http://m.share.hesvh.cn/Article/details/gpmzyotwp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.zdbjq.cn/Article/details/gibmsznjb.sHtML

Ruby: @name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gfhocujzj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.zdbjq.cn/Article/details/ghprnrwrc.sHtML

[G04] 定义方法
来源：http://www.blog.hesvh.cn/Article/details/gixhyiiou.sHtML

Py:   def greet(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/grgetpkby.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gyyxvyywm.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gsmhxgzeu.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/grtoojcii.sHtML

Java: String greet() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gtrnvbgzx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gzmceewye.sHtML

Ruby: def greet; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gppwrjxoa.sHtML

C#:   public string Greet() => Name;
来源：http://baike.hesvh.cn/Article/details/gqbaguyrr.sHtML

[G05] 继承
来源：http://baike.hesvh.cn/Article/details/gxjdqyhbu.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.zdbjq.cn/Article/details/gdzeowcnx.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gvlyomqgp.sHtML

JS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gmphpgwwr.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/glkavjqgn.sHtML

Java: class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gkzdcnygv.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.hesvh.cn/Article/details/gmczedlbe.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.fehbvm.com/Article/details/glqlxgxcl.sHtML

C#:   class Admin : User {}
来源：http://mobile.fehbvm.com/Article/details/gyiggxpzs.sHtML


<!-- 参考信息 -->