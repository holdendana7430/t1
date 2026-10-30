代发 wailian999

C#:   s.Replace("a", "b")
来源：http://blog.fehbvm.com/Article/details/gutgsftmj.sHtML

[E07] 按分隔符拆分
来源：http://www.share.zdbjq.cn/Article/details/gvpyyftdm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.fehbvm.com/Article/details/gftrcfujk.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gvppoavac.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.fehbvm.com/Article/details/gxfaoxlmb.sHtML

TS:   s.split(",")
来源：http://wap.hesvh.cn/Article/details/gtpshkrtw.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.fehbvm.com/Article/details/gdtsgimqy.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.hesvh.cn/Article/details/giskpwqcw.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.zdbjq.cn/Article/details/gmmzkxfan.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.zdbjq.cn/Article/details/gdczszhrb.sHtML

[E08] 数组按分隔符合并
来源：http://baike.fehbvm.com/Article/details/gvkxuzgrh.sHtML

Py:   ",".join(items)
来源：http://mobile.hesvh.cn/Article/details/gdalsqewo.sHtML

PHP:  implode(",", $items);
来源：http://baike.hesvh.cn/Article/details/gnxhivlwv.sHtML

JS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/ggnlpscrp.sHtML

TS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gmorwkykl.sHtML

Java: String.join(",", items)
来源：http://3g.fehbvm.com/Article/details/gxxkvadcm.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.fehbvm.com/Article/details/gfmddlwfy.sHtML

Ruby: items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gzcgiszku.sHtML

C#:   string.Join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gmhlmvprd.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.hesvh.cn/Article/details/grkwateow.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.zdbjq.cn/Article/details/gsjxiurvg.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fehbvm.com/Article/details/gukhypvpi.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/glrkxnuwr.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gvjozoylb.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/gqxawlgwz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.fehbvm.com/Article/details/glhuswybq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.fehbvm.com/Article/details/gnscxicsf.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gkkxxmdvu.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.fehbvm.com/Article/details/gbzfweroi.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gpqfgorpf.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.zdbjq.cn/Article/details/gmwlvwotf.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gfylyasjs.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gdkjvjcyz.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gtvpldpyu.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gfixmmrrq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/grbqsuyin.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.hesvh.cn/Article/details/gsbiofkyd.sHtML

[E11] 反转字符串
来源：http://wap.fehbvm.com/Article/details/gzwhabrbu.sHtML

Py:   s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gumswooqh.sHtML

PHP:  strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/gwnequdql.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/giobzlvnr.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gqamxujjw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.zdbjq.cn/Article/details/gsbmuhbwu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.zdbjq.cn/Article/details/gazrykcoe.sHtML

Ruby: s.reverse
来源：http://mobile.fehbvm.com/Article/details/gbxxjaopk.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gytfohaxr.sHtML

[E12] 统计某字符出现次数
来源：http://wap.fehbvm.com/Article/details/gpuasfarn.sHtML

Py:   s.count("a")
来源：http://wap.fehbvm.com/Article/details/gnhjlzblj.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.fehbvm.com/Article/details/gwoljeodq.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/grwltlfun.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/gctajuwry.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.hesvh.cn/Article/details/gribfqece.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.fehbvm.com/Article/details/gmitpfbcb.sHtML

Ruby: s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gkveawtku.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.hesvh.cn/Article/details/gocryrjnv.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.fehbvm.com/Article/details/gfpquaxaw.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.hesvh.cn/Article/details/gnlfpoxef.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.zdbjq.cn/Article/details/gmtyjwush.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/glxpspluf.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gassujodo.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.fehbvm.com/Article/details/gcdelduxs.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.fehbvm.com/Article/details/ghgitlyfq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.hesvh.cn/Article/details/gwyscpubn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.hesvh.cn/Article/details/gcgswffkd.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.zdbjq.cn/Article/details/gesvqwnsc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.hesvh.cn/Article/details/gfaxptneh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.fehbvm.com/Article/details/gfdrstkix.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.fehbvm.com/Article/details/gbvkjkyyd.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.hesvh.cn/Article/details/gilpglyhh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/guhlbrbee.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fehbvm.com/Article/details/gwipiokdy.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.zdbjq.cn/Article/details/gblvpfavy.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.fehbvm.com/Article/details/gnccomqho.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.hesvh.cn/Article/details/gheatwhwk.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.hesvh.cn/Article/details/gdqaulnut.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.hesvh.cn/Article/details/godrkxmhr.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.zdbjq.cn/Article/details/gwrnfivkj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.fehbvm.com/Article/details/giljnaqof.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.hesvh.cn/Article/details/gelwpjylu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.hesvh.cn/Article/details/guaqvwbvz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.zdbjq.cn/Article/details/gfzbqpfeu.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.hesvh.cn/Article/details/gsksxtvoi.sHtML

[E16] 数字千分位
来源：http://3g.hesvh.cn/Article/details/gjgdbabnt.sHtML

Py:   f"{1234567:,}"
来源：http://blog.zdbjq.cn/Article/details/ghkumnics.sHtML

PHP:  number_format(1234567);
来源：http://baike.zdbjq.cn/Article/details/golyikkvp.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/gpxndbmov.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gebzygtqt.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/gygbwvdva.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.fehbvm.com/Article/details/gwufmusso.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.hesvh.cn/Article/details/gttqlbliw.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fehbvm.com/Article/details/gpmaeqoio.sHtML

[E17] 首字母大写
来源：http://read.share.zdbjq.cn/Article/details/gfckmhqsf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.zdbjq.cn/Article/details/gkkdopwvw.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.fehbvm.com/Article/details/gushamcse.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gbylbtgvs.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/ghjdmghac.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.zdbjq.cn/Article/details/gsyxlplau.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.fehbvm.com/Article/details/gqjkqganx.sHtML

Ruby: s.capitalize
来源：http://www.m.share.hesvh.cn/Article/details/gmmzatlek.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.fehbvm.com/Article/details/gbdjgvapp.sHtML

[E18] 模板占位符替换
来源：http://3g.zdbjq.cn/Article/details/ggeonkuqs.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.zdbjq.cn/Article/details/gfrfgmouk.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.fehbvm.com/Article/details/giuysvkfe.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/glmvmorcv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/ghjhuqojz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gdiaoptbu.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gvlgzobgu.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.hesvh.cn/Article/details/gtabhcpsg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.hesvh.cn/Article/details/gyedyxlyq.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.hesvh.cn/Article/details/gprppeodb.sHtML

Py:   s.splitlines()
来源：http://www.blog.hesvh.cn/Article/details/gaowrqydk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gtngwahjj.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gnyebjwkl.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gduhrrujn.sHtML

Java: s.lines().toList()
来源：http://blog.hesvh.cn/Article/details/gkjcppuux.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.zdbjq.cn/Article/details/gnfrzstdm.sHtML

Ruby: s.lines
来源：http://www.share.zdbjq.cn/Article/details/gerrivdup.sHtML

C#:   s.Split('\n')
来源：http://www.share.hesvh.cn/Article/details/ghfpalpif.sHtML

[E20] 判断字符串是否为空
来源：http://blog.zdbjq.cn/Article/details/gbmueptzh.sHtML

Py:   if not s:
来源：http://wap.hesvh.cn/Article/details/gjeybcpdl.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.hesvh.cn/Article/details/ggmbtyqhn.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.zdbjq.cn/Article/details/gjteakvgo.sHtML

TS:   if (s === "") {}
来源：http://www.share.zdbjq.cn/Article/details/ggfahvhhh.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/gxcwasguo.sHtML

Go:   if s == "" {}
来源：http://3g.fehbvm.com/Article/details/ggzhiwtvf.sHtML

Ruby: if s.empty?
来源：http://read.share.hesvh.cn/Article/details/gxswxomli.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.zdbjq.cn/Article/details/gwmtueuia.sHtML

[E21] 超长截断加省略号
来源：http://blog.hesvh.cn/Article/details/gadndawvt.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.fehbvm.com/Article/details/gxmbvhwee.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gorpooihg.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gxjfflpli.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gjtmweelm.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gyquaflzv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.zdbjq.cn/Article/details/gvhmhbufy.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gevyiylth.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gokismwyu.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.hesvh.cn/Article/details/gkaauzhey.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.zdbjq.cn/Article/details/gnmlfbrum.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gmjaeskfo.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/gcbnvtlmn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/ggsfaxewh.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.fehbvm.com/Article/details/ghaljksvq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.hesvh.cn/Article/details/girefuker.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.zdbjq.cn/Article/details/goysklfrb.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.hesvh.cn/Article/details/gqplkqcaz.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/guqayuwta.sHtML

F. 文件与目录
来源：http://read.share.zdbjq.cn/Article/details/glshtfuwu.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gawzfdarj.sHtML

[F01] 读取整个文件
来源：http://read.share.fehbvm.com/Article/details/grvejanii.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.hesvh.cn/Article/details/glhiqekqh.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.hesvh.cn/Article/details/glyllbatm.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.hesvh.cn/Article/details/gqkyxxlqe.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gipxqtiqn.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gphubtups.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.hesvh.cn/Article/details/gkmdzdluf.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fehbvm.com/Article/details/glgslqtac.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gpxpugpuv.sHtML

[F02] 逐行读取文件
来源：http://www.share.hesvh.cn/Article/details/gvmqpnekp.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.zdbjq.cn/Article/details/gplzqpojb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.fehbvm.com/Article/details/gzbvwlbhr.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/gaejycjds.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gexhjaupw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gwuyqgdtr.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.fehbvm.com/Article/details/gxcvvwpjh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.hesvh.cn/Article/details/gvpbgtiku.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.fehbvm.com/Article/details/gbzisydmf.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fehbvm.com/Article/details/guwdetvcs.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.hesvh.cn/Article/details/gtomuyadk.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gjuvoqxtx.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gslwdvgqf.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gnhiyctqq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.fehbvm.com/Article/details/gotamqwmk.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fehbvm.com/Article/details/gtyeqpjfm.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.fehbvm.com/Article/details/gzfyngrwx.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/grdtgbaox.sHtML

[F04] 追加写入文件
来源：http://read.share.hesvh.cn/Article/details/gltkyitlm.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.zdbjq.cn/Article/details/gjwgemzyb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.hesvh.cn/Article/details/gyykjaxea.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/golkxncnc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gvygxhycg.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.hesvh.cn/Article/details/gmaohzjdv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gsosgwoyr.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.hesvh.cn/Article/details/gnojxcinj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.zdbjq.cn/Article/details/gkpfifqux.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.hesvh.cn/Article/details/gzqucmcyc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.fehbvm.com/Article/details/gnquakfur.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.hesvh.cn/Article/details/gpggumtgm.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gixrgkmpr.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gqkykioby.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gnbuvpegv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.zdbjq.cn/Article/details/gjmsphcvy.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gmxtxojuy.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gdaftngit.sHtML

[F06] 删除文件
来源：http://mobile.fehbvm.com/Article/details/gqzfwkddz.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gflexohzl.sHtML

PHP:  unlink("a.txt");
来源：http://baike.hesvh.cn/Article/details/gvbgdwfgi.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gdrajjgdr.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gkubijjpd.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gwzypdhuk.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/golhjgyob.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gniaecahq.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gymwdpbnf.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.fehbvm.com/Article/details/gnuxsulrd.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/gulhfnkog.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.hesvh.cn/Article/details/gxcfkcyfx.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/gmvmxezhs.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gckcpxhkz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.zdbjq.cn/Article/details/gjvbbnlun.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.zdbjq.cn/Article/details/gpflqnwse.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.zdbjq.cn/Article/details/gcfzesmgh.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.hesvh.cn/Article/details/giwnimngo.sHtML

[F08] 遍历目录
来源：http://www.blog.fehbvm.com/Article/details/gdvxxivpq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.zdbjq.cn/Article/details/gbwtlczks.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.zdbjq.cn/Article/details/ghjexaypk.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gbenjexjm.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gvtlbacdg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gcwhhbukc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.hesvh.cn/Article/details/gambzojmp.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.hesvh.cn/Article/details/geqeoazig.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gxbjjiqqt.sHtML

[F09] 获取文件大小
来源：http://m.share.hesvh.cn/Article/details/gorivgwbs.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/ggkgdgoti.sHtML

PHP:  filesize("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gohbfjrtq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gnbcywrsm.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gyqcogrxe.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/guthkvbck.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.hesvh.cn/Article/details/gingbvtzk.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/geqnewjpe.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.hesvh.cn/Article/details/gbjnhdfso.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.hesvh.cn/Article/details/gwofhtwds.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gvhalatkv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gbpkalhjr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gexrpqurw.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gtixwjglq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.fehbvm.com/Article/details/guidcebgm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gxxvhlhjd.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gutxriscj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gjdayflkv.sHtML

[F11] 复制与移动文件
来源：http://read.share.zdbjq.cn/Article/details/gbeawyciw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gtjnmvbdo.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.hesvh.cn/Article/details/ggtmmkelz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gqbrlrwzc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gldeblxpz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.hesvh.cn/Article/details/gmpysiqdu.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.hesvh.cn/Article/details/gcanygtvh.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gsxyemiem.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.hesvh.cn/Article/details/gnoxmcfly.sHtML

[F12] CSV 读写
来源：http://www.m.share.hesvh.cn/Article/details/gjncvaaoe.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fehbvm.com/Article/details/gpbcmpebu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.zdbjq.cn/Article/details/gfthaoemm.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.hesvh.cn/Article/details/gqpxmxwxw.sHtML

TS:   // 同上
来源：http://mobile.fehbvm.com/Article/details/gmxlxezqu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.zdbjq.cn/Article/details/gflbechbp.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.hesvh.cn/Article/details/gowjetwrf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fehbvm.com/Article/details/gzmnxpzsu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fehbvm.com/Article/details/grfpsyqtq.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwrduhhio.sHtML

G. 面向对象
来源：http://mobile.zdbjq.cn/Article/details/gkqqwuitu.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmtqgugcb.sHtML

[G01] 定义类
来源：http://www.share.zdbjq.cn/Article/details/gggpaxyuo.sHtML

Py:   class User: pass
来源：http://3g.fehbvm.com/Article/details/gdqddtypb.sHtML

PHP:  class User {}
来源：http://www.share.hesvh.cn/Article/details/gwppeovlo.sHtML

JS:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gdaqgvpcw.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.hesvh.cn/Article/details/gwqkfdqnb.sHtML

Java: class User {}
来源：http://www.share.zdbjq.cn/Article/details/glptyeubd.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/gysqjdfdt.sHtML

Ruby: class User; end
来源：http://blog.hesvh.cn/Article/details/gyacnviza.sHtML

C#:   class User {}
来源：http://3g.hesvh.cn/Article/details/grltziilg.sHtML

[G02] 构造函数
来源：http://blog.zdbjq.cn/Article/details/gzawwspdk.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.hesvh.cn/Article/details/gscvbfopn.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.hesvh.cn/Article/details/geejdhaod.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gzkkzefdz.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fehbvm.com/Article/details/glxtokhdi.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gxjdllhjz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fehbvm.com/Article/details/gyszeuedt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.fehbvm.com/Article/details/gilqdydig.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.hesvh.cn/Article/details/gprzbxnjt.sHtML

[G03] 实例属性
来源：http://m.share.zdbjq.cn/Article/details/grnftnknm.sHtML

Py:   self.name = "x"
来源：http://read.share.fehbvm.com/Article/details/gfcieenfz.sHtML

PHP:  public string $name = "x";
来源：http://baike.zdbjq.cn/Article/details/gmzojxlpl.sHtML

JS:   this.name = "x";
来源：http://3g.fehbvm.com/Article/details/gyvohggsi.sHtML

TS:   name: string = "x";
来源：http://baike.fehbvm.com/Article/details/gbvpviyeq.sHtML

Java: private String name;
来源：http://wap.fehbvm.com/Article/details/gwofnslpa.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.hesvh.cn/Article/details/gghqvmmuq.sHtML

Ruby: @name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gyexgazbz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.zdbjq.cn/Article/details/gtstjssim.sHtML

[G04] 定义方法
来源：http://mobile.zdbjq.cn/Article/details/ghusljjjk.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gzcdyvxoh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxxclsaoa.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gglvnxolw.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gqkltymxi.sHtML

Java: String greet() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/ggyurwszf.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gobuqfdgo.sHtML

Ruby: def greet; @name; end
来源：http://baike.zdbjq.cn/Article/details/gxkmnvtco.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gtbopqkuj.sHtML

[G05] 继承
来源：http://www.blog.zdbjq.cn/Article/details/gcyeyizup.sHtML

Py:   class Admin(User): pass
来源：http://m.share.zdbjq.cn/Article/details/gkhjlyvqk.sHtML

PHP:  class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gitaivbfq.sHtML

JS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/ghzdoecgp.sHtML

TS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gebftqssh.sHtML


<!-- 参考信息 -->