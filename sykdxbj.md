代发 wailian999

Go:   strings.Join(items, ",")
来源：http://mobile.hesvh.cn/Article/details/gznysvyff.sHtML

Ruby: items.join(",")
来源：http://baike.zdbjq.cn/Article/details/ggbmunwct.sHtML

C#:   string.Join(",", items)
来源：http://wap.zdbjq.cn/Article/details/gzvfjhiip.sHtML

[E09] 去除所有空白字符
来源：http://wap.hesvh.cn/Article/details/gdmhjlxzg.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.fehbvm.com/Article/details/galathhkm.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.zdbjq.cn/Article/details/gkiqwbwyw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gcmqqemnb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gfwubilwt.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.fehbvm.com/Article/details/gsjntjjvu.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.zdbjq.cn/Article/details/geivfpgcx.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.zdbjq.cn/Article/details/ggeikkdol.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gxvkvyeps.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.zdbjq.cn/Article/details/gffszcfyu.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.fehbvm.com/Article/details/gmmbanznm.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.fehbvm.com/Article/details/geucttfvt.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gqlrnammq.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/grehxbabo.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gusrsgpia.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gewmhisas.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gfzablfab.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.fehbvm.com/Article/details/gtamqwndi.sHtML

[E11] 反转字符串
来源：http://baike.zdbjq.cn/Article/details/gxqdipaht.sHtML

Py:   s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/glhptiydl.sHtML

PHP:  strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gcdbqzeip.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gfuvyjkpj.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/glxtnupky.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.zdbjq.cn/Article/details/grgkmfnma.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.fehbvm.com/Article/details/gclnqelks.sHtML

Ruby: s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gxfuhffxr.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/gygopejwp.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.fehbvm.com/Article/details/gthhktyuh.sHtML

Py:   s.count("a")
来源：http://blog.zdbjq.cn/Article/details/guglpeqxg.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.hesvh.cn/Article/details/gwwwiyrjh.sHtML

JS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/grfduqodl.sHtML

TS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gjcjfnpzz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.zdbjq.cn/Article/details/ghvhlhuuj.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.hesvh.cn/Article/details/gzwwokath.sHtML

Ruby: s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/gaxsoaeyb.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.hesvh.cn/Article/details/gpvqzvprn.sHtML

[E13] 逐字符遍历
来源：http://blog.hesvh.cn/Article/details/gnoaaackb.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.fehbvm.com/Article/details/glbthuzla.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.fehbvm.com/Article/details/gajmzvcuc.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/ghtangcmg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/guyydbuaj.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.fehbvm.com/Article/details/gygxlycqw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.hesvh.cn/Article/details/gllkzansf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.fehbvm.com/Article/details/gztebqxpi.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gwkiyrmgo.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.hesvh.cn/Article/details/grhqtqkzx.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.hesvh.cn/Article/details/guhjavpsc.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.fehbvm.com/Article/details/gpjgofetn.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.fehbvm.com/Article/details/gigjuxxnc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.fehbvm.com/Article/details/gbzajqhup.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.fehbvm.com/Article/details/gtaqruaza.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.zdbjq.cn/Article/details/gweiqdhse.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.zdbjq.cn/Article/details/gbjrculxl.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.fehbvm.com/Article/details/gkvycvutf.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.hesvh.cn/Article/details/gsjqasydi.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.zdbjq.cn/Article/details/gnyatbqyc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.zdbjq.cn/Article/details/gtfmhdukd.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.zdbjq.cn/Article/details/gqbtgudfo.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.hesvh.cn/Article/details/gecdliksa.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.fehbvm.com/Article/details/grrvxbyzy.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.zdbjq.cn/Article/details/gkwprqnaj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gcehoxenv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.zdbjq.cn/Article/details/gyjoszhif.sHtML

[E16] 数字千分位
来源：http://www.blog.hesvh.cn/Article/details/ghncbarop.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.fehbvm.com/Article/details/gbvncktzz.sHtML

PHP:  number_format(1234567);
来源：http://baike.fehbvm.com/Article/details/gfifcrqxi.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gqwbvmdac.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gbicuuyzf.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.fehbvm.com/Article/details/gkwcfnuyx.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.hesvh.cn/Article/details/gozujynli.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.zdbjq.cn/Article/details/gthpiojer.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.fehbvm.com/Article/details/geuharizm.sHtML

[E17] 首字母大写
来源：http://baike.hesvh.cn/Article/details/gxcrcmmgt.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.zdbjq.cn/Article/details/gnieyldoc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.hesvh.cn/Article/details/gpihfsgoh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gwbeluldi.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gcrqnrdzf.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.zdbjq.cn/Article/details/ghsjwqdko.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.zdbjq.cn/Article/details/goxqgeuth.sHtML

Ruby: s.capitalize
来源：http://3g.zdbjq.cn/Article/details/gkdfrluwu.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.hesvh.cn/Article/details/gngionoig.sHtML

[E18] 模板占位符替换
来源：http://3g.hesvh.cn/Article/details/glsmkwzfh.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.fehbvm.com/Article/details/ghosedpmv.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.zdbjq.cn/Article/details/gmtypszeb.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/guyljefor.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/ginzffuai.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gpsvpyiii.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gjxvaxidd.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.hesvh.cn/Article/details/gvcpxxmgv.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.fehbvm.com/Article/details/gfbflmrmn.sHtML

[E19] 多行文本按行拆分
来源：http://wap.zdbjq.cn/Article/details/ghnlzswaj.sHtML

Py:   s.splitlines()
来源：http://mobile.zdbjq.cn/Article/details/gdkhzvrzp.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.hesvh.cn/Article/details/guuilebgg.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/ghxdkcpiy.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gidjoxwod.sHtML

Java: s.lines().toList()
来源：http://www.share.zdbjq.cn/Article/details/giedxpmba.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.fehbvm.com/Article/details/gqknnbfwi.sHtML

Ruby: s.lines
来源：http://www.blog.fehbvm.com/Article/details/gieqybdtt.sHtML

C#:   s.Split('\n')
来源：http://blog.hesvh.cn/Article/details/gpamzkhek.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.zdbjq.cn/Article/details/gekldjypx.sHtML

Py:   if not s:
来源：http://www.m.share.fehbvm.com/Article/details/gwztjeees.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.hesvh.cn/Article/details/gieasxfwh.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.fehbvm.com/Article/details/glhxxoezo.sHtML

TS:   if (s === "") {}
来源：http://www.share.hesvh.cn/Article/details/gwemewszb.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/gxqabggwm.sHtML

Go:   if s == "" {}
来源：http://wap.zdbjq.cn/Article/details/gcxsmzedm.sHtML

Ruby: if s.empty?
来源：http://m.share.fehbvm.com/Article/details/gxqecduoo.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.zdbjq.cn/Article/details/ghhldcejv.sHtML

[E21] 超长截断加省略号
来源：http://m.share.hesvh.cn/Article/details/growmplbx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.zdbjq.cn/Article/details/gozoitomm.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gepcnjvoy.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gorducrbj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gnxelozoa.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/guggpxccx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fehbvm.com/Article/details/gfkvedvpm.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gjskrdfye.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gavpafmrb.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.hesvh.cn/Article/details/gmveeabwh.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.zdbjq.cn/Article/details/goysuawkl.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gqourzbdi.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gkcdnbfnl.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/gfhrbmspj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.hesvh.cn/Article/details/ghnwqzqjw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.hesvh.cn/Article/details/gklriqxjo.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.fehbvm.com/Article/details/gjmhecrwd.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.hesvh.cn/Article/details/ggqwtjptu.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxgpkcorr.sHtML

F. 文件与目录
来源：http://3g.hesvh.cn/Article/details/gckrqueth.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gtdmimgku.sHtML

[F01] 读取整个文件
来源：http://www.blog.zdbjq.cn/Article/details/gemkrmjwd.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fehbvm.com/Article/details/gehefmyeb.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gfusbmtne.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.zdbjq.cn/Article/details/gacogvesa.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.hesvh.cn/Article/details/gpabfvvwt.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/geaxnmdru.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.zdbjq.cn/Article/details/gzaxrcjgv.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gkvwvuqku.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gjsydtbnx.sHtML

[F02] 逐行读取文件
来源：http://read.share.zdbjq.cn/Article/details/gsqwaqpnl.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.fehbvm.com/Article/details/gebfilewx.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.hesvh.cn/Article/details/gkljxynyr.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gurxhqhag.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gvadaljvt.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/gasbmjqiv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.zdbjq.cn/Article/details/ggxgvqota.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.hesvh.cn/Article/details/gpmgpxuqy.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.zdbjq.cn/Article/details/goyjxenlo.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.hesvh.cn/Article/details/gvmrhnmuv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.hesvh.cn/Article/details/gzsrgdnko.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gypopmbkq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gxncbtdts.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gjwptqjtj.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.hesvh.cn/Article/details/gkpsviecj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.zdbjq.cn/Article/details/graoivyeu.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gvfbjznhh.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gwdjxyrkd.sHtML

[F04] 追加写入文件
来源：http://baike.fehbvm.com/Article/details/gxgbalrjo.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.hesvh.cn/Article/details/gwaqbghiy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.zdbjq.cn/Article/details/gtadptcff.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gawaowbaj.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/gejmzkyck.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.fehbvm.com/Article/details/gaptfohed.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gtdwrnkas.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.hesvh.cn/Article/details/gledygske.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.hesvh.cn/Article/details/grdcnzhrk.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.zdbjq.cn/Article/details/gqwhwioqp.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.hesvh.cn/Article/details/gtxstbeob.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.fehbvm.com/Article/details/grulanoav.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gaaehrowb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gtkwychmj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gvqdafnzy.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.zdbjq.cn/Article/details/gsejriled.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.hesvh.cn/Article/details/ggqfspsgd.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.fehbvm.com/Article/details/gxjsnjygg.sHtML

[F06] 删除文件
来源：http://3g.zdbjq.cn/Article/details/gmczvchfz.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/ggssbpuie.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gfftugzoy.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gbygiehra.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gxgjvvstn.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gcibxszvt.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gptzrpyqh.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gxihxovtm.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gazbkpnsg.sHtML

[F07] 创建目录（含多级）
来源：http://baike.fehbvm.com/Article/details/gnibmkdoa.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gcmgcjodz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.fehbvm.com/Article/details/gmswltmbx.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/grmnxuvpv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gtdjrzuuq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.hesvh.cn/Article/details/gfnylggnr.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.hesvh.cn/Article/details/geothswxr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.hesvh.cn/Article/details/gwopzyeza.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.hesvh.cn/Article/details/gmqclxkqv.sHtML

[F08] 遍历目录
来源：http://blog.hesvh.cn/Article/details/gjupzicas.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.hesvh.cn/Article/details/gdlbwdhwf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fehbvm.com/Article/details/gfwonndpt.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/gimdxrmpr.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/grjizbxxl.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gjdigmash.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.hesvh.cn/Article/details/grqqziqzo.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fehbvm.com/Article/details/gmeolnvug.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.hesvh.cn/Article/details/gnbsutwde.sHtML

[F09] 获取文件大小
来源：http://blog.zdbjq.cn/Article/details/grdzhodzj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.hesvh.cn/Article/details/gimbohkxv.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gfhiougfx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/geeylcdmb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/gpmxgyjxp.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gyplloezk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.zdbjq.cn/Article/details/gielaoerr.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gqfhcjgtr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.zdbjq.cn/Article/details/gazvvvnzi.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.zdbjq.cn/Article/details/giithjggg.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gwyfpjzxs.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.hesvh.cn/Article/details/gulfacmnn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gerntkksp.sHtML

TS:   path.extname("a.txt")
来源：http://blog.hesvh.cn/Article/details/gmzofknpt.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.hesvh.cn/Article/details/gxdmwyutd.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/ghnikjlmd.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/ghnqsuysq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gcmtszcdy.sHtML

[F11] 复制与移动文件
来源：http://wap.hesvh.cn/Article/details/gtbgjllwg.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gdolvjbpb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.hesvh.cn/Article/details/gthvdjwvk.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gtrrkjjou.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gpmoxupfi.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gzdyuyqwi.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.fehbvm.com/Article/details/gbyrhemxv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gkxlegkaw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.zdbjq.cn/Article/details/gqzbfilam.sHtML

[F12] CSV 读写
来源：http://m.share.hesvh.cn/Article/details/gyhwrxbxw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.hesvh.cn/Article/details/gxneerxzf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.hesvh.cn/Article/details/gkdkonywe.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.zdbjq.cn/Article/details/gdlmsysiz.sHtML

TS:   // 同上
来源：http://www.blog.zdbjq.cn/Article/details/geayzfnum.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fehbvm.com/Article/details/gwxdtjsej.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.hesvh.cn/Article/details/githryqqs.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.hesvh.cn/Article/details/goixyrljb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fehbvm.com/Article/details/gwwckyykf.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gxdkmzldg.sHtML

G. 面向对象
来源：http://read.share.hesvh.cn/Article/details/gfhiitbfw.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gwqeqtdgn.sHtML

[G01] 定义类
来源：http://blog.fehbvm.com/Article/details/glwsxeegl.sHtML

Py:   class User: pass
来源：http://wap.zdbjq.cn/Article/details/gnevdwwmx.sHtML

PHP:  class User {}
来源：http://www.share.fehbvm.com/Article/details/ghtpulyes.sHtML

JS:   class User {}
来源：http://baike.hesvh.cn/Article/details/ghlpzuyzw.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.zdbjq.cn/Article/details/gjxhnwqaw.sHtML

Java: class User {}
来源：http://baike.hesvh.cn/Article/details/gydvjsgzt.sHtML

Go:   type User struct { Name string }
来源：http://read.share.fehbvm.com/Article/details/goeiduzzb.sHtML

Ruby: class User; end
来源：http://3g.fehbvm.com/Article/details/gujlksrej.sHtML

C#:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmurrbkry.sHtML

[G02] 构造函数
来源：http://www.share.fehbvm.com/Article/details/gntrwzbvr.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/gwzhrlgih.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.hesvh.cn/Article/details/gujznzoua.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/ggboixjzw.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fehbvm.com/Article/details/gypxiuipz.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gumklmbuj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.hesvh.cn/Article/details/gcjjmxhxj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.zdbjq.cn/Article/details/gofbxzvyk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gqwmeqluo.sHtML

[G03] 实例属性
来源：http://baike.fehbvm.com/Article/details/gryaqstbn.sHtML

Py:   self.name = "x"
来源：http://m.share.fehbvm.com/Article/details/gfqgmmjye.sHtML

PHP:  public string $name = "x";
来源：http://wap.hesvh.cn/Article/details/gqrclqwax.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gqhwafyms.sHtML

TS:   name: string = "x";
来源：http://read.share.hesvh.cn/Article/details/gpoevblqj.sHtML

Java: private String name;
来源：http://3g.fehbvm.com/Article/details/gentbseok.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fehbvm.com/Article/details/gcqdfjlio.sHtML

Ruby: @name = "x"
来源：http://baike.hesvh.cn/Article/details/giierbbly.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.zdbjq.cn/Article/details/gexqfbvxv.sHtML

[G04] 定义方法
来源：http://mobile.zdbjq.cn/Article/details/ghzsiadww.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gllizlkos.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gqmovlfph.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gkrurlutm.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gieztbqmn.sHtML

Java: String greet() { return name; }
来源：http://3g.hesvh.cn/Article/details/gnxwknltg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gzjqmcrsx.sHtML

Ruby: def greet; @name; end
来源：http://baike.fehbvm.com/Article/details/gloosuzxa.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.zdbjq.cn/Article/details/ggyfavycy.sHtML

[G05] 继承
来源：http://3g.hesvh.cn/Article/details/gpsfhvyll.sHtML

Py:   class Admin(User): pass
来源：http://www.share.fehbvm.com/Article/details/gvtpzrebf.sHtML

PHP:  class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gckiipmjq.sHtML

JS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gyttrlbfa.sHtML

TS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gjnlxjuvf.sHtML

Java: class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gltcroqjd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.hesvh.cn/Article/details/grisosqan.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.fehbvm.com/Article/details/guixinihs.sHtML

C#:   class Admin : User {}
来源：http://m.share.hesvh.cn/Article/details/gvimkyzuv.sHtML

[G06] 重写方法
来源：http://wap.zdbjq.cn/Article/details/gcdkuyatg.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.zdbjq.cn/Article/details/galuiknhj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gpuojpeqt.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gffuzdxcg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gkjfstwuf.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gidyopfzl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.zdbjq.cn/Article/details/geqcfovqu.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.hesvh.cn/Article/details/gfwvwmhqv.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fehbvm.com/Article/details/gidfpcyjz.sHtML

[G07] 调用父类方法
来源：http://wap.zdbjq.cn/Article/details/gqosndlda.sHtML

Py:   super().greet()
来源：http://wap.fehbvm.com/Article/details/gvvahnihf.sHtML

PHP:  parent::greet();
来源：http://m.share.zdbjq.cn/Article/details/ggpbykrdf.sHtML


<!-- 参考信息 -->