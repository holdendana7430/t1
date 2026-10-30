代发 wailian999

Ruby: s.split(",");  s.split
来源：http://www.m.share.fehbvm.com/Article/details/gzoyuflys.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.hesvh.cn/Article/details/gvuebrmha.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.hesvh.cn/Article/details/glqauawnt.sHtML

Py:   ",".join(items)
来源：http://mobile.zdbjq.cn/Article/details/geedcxrot.sHtML

PHP:  implode(",", $items);
来源：http://www.share.hesvh.cn/Article/details/gyvlfjhzf.sHtML

JS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gcnjistyk.sHtML

TS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/glfcnylje.sHtML

Java: String.join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/gptdfxvyu.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.hesvh.cn/Article/details/glsrwpfje.sHtML

Ruby: items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gdpgitmnj.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/garyaepoo.sHtML

[E09] 去除所有空白字符
来源：http://m.share.hesvh.cn/Article/details/gabsrzljp.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.hesvh.cn/Article/details/gaezoyxuo.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.fehbvm.com/Article/details/gcjhiwmkd.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gioxhovmh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/gqjxfvthf.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.fehbvm.com/Article/details/geipdofti.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.hesvh.cn/Article/details/gudexeckv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.zdbjq.cn/Article/details/gpnhnapkg.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gcdbtwalw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.zdbjq.cn/Article/details/gtkeohzdn.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.fehbvm.com/Article/details/gwbvjfisy.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.hesvh.cn/Article/details/gzhvlxqic.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gjnpvrrcf.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/glamjvkld.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/glitstjhq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gydpyhkxa.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gxvclmppx.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.zdbjq.cn/Article/details/gwxayewfd.sHtML

[E11] 反转字符串
来源：http://baike.hesvh.cn/Article/details/gdvcuykqk.sHtML

Py:   s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gsmydpcib.sHtML

PHP:  strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gmqcuwnuo.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/grnyivzaa.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/guhaarxau.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.zdbjq.cn/Article/details/gfgjuwiik.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fehbvm.com/Article/details/gjbvpjqkx.sHtML

Ruby: s.reverse
来源：http://mobile.zdbjq.cn/Article/details/ghzdvovph.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/gfefwykmx.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.fehbvm.com/Article/details/gteyxogkd.sHtML

Py:   s.count("a")
来源：http://3g.hesvh.cn/Article/details/gxsaexwlf.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.fehbvm.com/Article/details/gcxayijfn.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gatnxbcdx.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gzlkffpkr.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.fehbvm.com/Article/details/gkrjsykmy.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.hesvh.cn/Article/details/gktrusphg.sHtML

Ruby: s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/gribfskwi.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.zdbjq.cn/Article/details/gnbhlwgvj.sHtML

[E13] 逐字符遍历
来源：http://wap.zdbjq.cn/Article/details/gftkehcpg.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.hesvh.cn/Article/details/ggvsmbtsq.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.fehbvm.com/Article/details/gycxkmxam.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gophsamid.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gsofyzqex.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.zdbjq.cn/Article/details/ggtedwlte.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.hesvh.cn/Article/details/gupmrzgjb.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.hesvh.cn/Article/details/gpfuaxzbb.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.fehbvm.com/Article/details/gghjbfnwt.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.hesvh.cn/Article/details/gryjqzicb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.zdbjq.cn/Article/details/glsuyzvqd.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gurwafots.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.zdbjq.cn/Article/details/gbbugxayw.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.hesvh.cn/Article/details/guxfqyxkr.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gjspfqnqo.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fehbvm.com/Article/details/gdsjzwzyb.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.fehbvm.com/Article/details/genfvphpd.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.hesvh.cn/Article/details/gblkajxxb.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.zdbjq.cn/Article/details/gvjzelrog.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.fehbvm.com/Article/details/ghnkxkgku.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.zdbjq.cn/Article/details/gzltpdcxj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gmijgdmhw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.fehbvm.com/Article/details/ghnoqwjav.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.hesvh.cn/Article/details/glxmvjgxc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fehbvm.com/Article/details/gdmrquiyi.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.hesvh.cn/Article/details/glhepzeoh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.zdbjq.cn/Article/details/gxleaoihj.sHtML

[E16] 数字千分位
来源：http://3g.fehbvm.com/Article/details/gtsmeddfs.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.zdbjq.cn/Article/details/ggrbfzldy.sHtML

PHP:  number_format(1234567);
来源：http://www.share.zdbjq.cn/Article/details/gllhcxans.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/gvydsfsjc.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/gwwqfnqhd.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.fehbvm.com/Article/details/gclunlfxj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.zdbjq.cn/Article/details/gndnkfuvo.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.hesvh.cn/Article/details/gimnikxzu.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.hesvh.cn/Article/details/gmkzvzaxg.sHtML

[E17] 首字母大写
来源：http://m.share.zdbjq.cn/Article/details/ghzugxfeu.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.fehbvm.com/Article/details/gclxhawcc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.hesvh.cn/Article/details/godduwxvy.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gjyrmnohl.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/gmojwnepq.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.fehbvm.com/Article/details/gahseeowz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.hesvh.cn/Article/details/glvhxwepf.sHtML

Ruby: s.capitalize
来源：http://wap.fehbvm.com/Article/details/ggsnopgnv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.fehbvm.com/Article/details/gsgobvpsu.sHtML

[E18] 模板占位符替换
来源：http://blog.hesvh.cn/Article/details/gkfqblppi.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.zdbjq.cn/Article/details/gcpoprvsl.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.fehbvm.com/Article/details/ghzhklboh.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gecacapla.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gakfrtzhj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/ghsyljnrv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.fehbvm.com/Article/details/giwzkhhnb.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.hesvh.cn/Article/details/gwenitzbu.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.hesvh.cn/Article/details/grqnyasdo.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fehbvm.com/Article/details/gwqmboeeq.sHtML

Py:   s.splitlines()
来源：http://blog.zdbjq.cn/Article/details/glumszjzb.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.hesvh.cn/Article/details/gxtvjpira.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/guopvqrra.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gpkegqrdc.sHtML

Java: s.lines().toList()
来源：http://www.blog.hesvh.cn/Article/details/gfzawlbpu.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.fehbvm.com/Article/details/geeaijarn.sHtML

Ruby: s.lines
来源：http://m.share.hesvh.cn/Article/details/gbqntwkdo.sHtML

C#:   s.Split('\n')
来源：http://read.share.zdbjq.cn/Article/details/gywbeuvpu.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.zdbjq.cn/Article/details/gybhjirdp.sHtML

Py:   if not s:
来源：http://wap.fehbvm.com/Article/details/gexgasuvu.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.zdbjq.cn/Article/details/gkcssxzhy.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.hesvh.cn/Article/details/gqlxtjuoj.sHtML

TS:   if (s === "") {}
来源：http://read.share.zdbjq.cn/Article/details/gjcflezmv.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/geazzqnhi.sHtML

Go:   if s == "" {}
来源：http://wap.zdbjq.cn/Article/details/gijrcoqbx.sHtML

Ruby: if s.empty?
来源：http://read.share.fehbvm.com/Article/details/gpidyfvsl.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.hesvh.cn/Article/details/gjfkmslxk.sHtML

[E21] 超长截断加省略号
来源：http://wap.zdbjq.cn/Article/details/goefypgob.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.zdbjq.cn/Article/details/gtwkkqriu.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gkiigthcv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/grzolsehj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gnsytiylm.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gujgjbjws.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.zdbjq.cn/Article/details/gblhggomt.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gabsgdqkg.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/goimwjjjp.sHtML

[E22] 字节长度与字符长度
来源：http://blog.hesvh.cn/Article/details/gicapccqv.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.fehbvm.com/Article/details/gwjsvpaga.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/guhivepwk.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gjmrymyey.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/galouhyhw.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.zdbjq.cn/Article/details/ggncrrwhv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.fehbvm.com/Article/details/glsvazvcs.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.fehbvm.com/Article/details/gdipwibds.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.zdbjq.cn/Article/details/gofslpuhq.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/govfdecdn.sHtML

F. 文件与目录
来源：http://m.share.hesvh.cn/Article/details/giwvlkoda.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gqulnjrcp.sHtML

[F01] 读取整个文件
来源：http://read.share.zdbjq.cn/Article/details/gahjfmopq.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.hesvh.cn/Article/details/ggatkpnco.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gztmndqyr.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.hesvh.cn/Article/details/gsxtnzazc.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gioveyjfc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/giurzqfjd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.fehbvm.com/Article/details/gmqohgxrh.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/glrpkiwei.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.zdbjq.cn/Article/details/goujbnajy.sHtML

[F02] 逐行读取文件
来源：http://3g.zdbjq.cn/Article/details/gztirtopn.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.zdbjq.cn/Article/details/gjrbbbjgu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.fehbvm.com/Article/details/gtyfgmowr.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gyddaisdn.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gjipbssee.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gwmuefovm.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.hesvh.cn/Article/details/gxftvsccj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.hesvh.cn/Article/details/grndlnius.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.fehbvm.com/Article/details/guyxmmglt.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.zdbjq.cn/Article/details/gfrllzavp.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.fehbvm.com/Article/details/gpvqtfxlv.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gforsdbve.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gvvjoaxwz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/gzrrtwvzk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.fehbvm.com/Article/details/gpocsfwjz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.zdbjq.cn/Article/details/gjneezrbn.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.zdbjq.cn/Article/details/gutgygshl.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.fehbvm.com/Article/details/gnooajnrk.sHtML

[F04] 追加写入文件
来源：http://3g.zdbjq.cn/Article/details/gptowmwud.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.zdbjq.cn/Article/details/gtauzwbts.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fehbvm.com/Article/details/ggpahozcs.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/gntuanydt.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/gvaqadgwd.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fehbvm.com/Article/details/gidwckmfj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gscraewzm.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.hesvh.cn/Article/details/guxdifkou.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fehbvm.com/Article/details/gjkcwqlit.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.zdbjq.cn/Article/details/gvojskjzk.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.fehbvm.com/Article/details/gyvvxniey.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gpcqlnuye.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gbplsuhmn.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gszkzjjqj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/glirmvytz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fehbvm.com/Article/details/gnzsgtikx.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gifnpcikw.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.hesvh.cn/Article/details/glvabdvcs.sHtML

[F06] 删除文件
来源：http://m.share.hesvh.cn/Article/details/gghdxeblu.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/goqjlxvfn.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gnydwedre.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/giwxaproa.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gtoujegcs.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gwurvohsk.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gzcignpvz.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.zdbjq.cn/Article/details/grgsszmed.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.fehbvm.com/Article/details/glvetgipg.sHtML

[F07] 创建目录（含多级）
来源：http://3g.fehbvm.com/Article/details/gpnpxooxt.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/gasrlumak.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.fehbvm.com/Article/details/gmnogytvv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gbnabjhzv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/gqodtzuxq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.zdbjq.cn/Article/details/gmqfcktvp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.hesvh.cn/Article/details/gmnhwkyik.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.hesvh.cn/Article/details/gasgrxpni.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.fehbvm.com/Article/details/gjkaynahd.sHtML

[F08] 遍历目录
来源：http://baike.hesvh.cn/Article/details/gqdqowiyx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.hesvh.cn/Article/details/gvnnfsshv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.fehbvm.com/Article/details/gfcbleghm.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/gqdrommzy.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/ghhkmsqsx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gfpjvdigv.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.fehbvm.com/Article/details/gkcbqbiyu.sHtML

Ruby: Dir.children("dir")
来源：http://baike.zdbjq.cn/Article/details/gsphofrcg.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.hesvh.cn/Article/details/groubsfpt.sHtML

[F09] 获取文件大小
来源：http://read.share.hesvh.cn/Article/details/giywmhraj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gfyksooly.sHtML

PHP:  filesize("a.txt");
来源：http://baike.hesvh.cn/Article/details/gqjcfffcz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gbdpkukgo.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/gvdnzkntt.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gsvffeiij.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.zdbjq.cn/Article/details/gsowrglar.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gvscolvsd.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.hesvh.cn/Article/details/gxydyiqki.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.zdbjq.cn/Article/details/gpuiwkqnx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gulgvgddn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gsexfensk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/grskvgvcr.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gdsyhbdjy.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.fehbvm.com/Article/details/glllgfxui.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gvwnrrcgo.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gdjljpvxp.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/grrdbsozd.sHtML

[F11] 复制与移动文件
来源：http://blog.hesvh.cn/Article/details/gegtqcusj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gvuqlylpf.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.fehbvm.com/Article/details/gnzdzsnwi.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ggwqnubmo.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gzsmvldvu.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fehbvm.com/Article/details/gxsijeoqa.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.hesvh.cn/Article/details/grwaokexv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gsjbapiad.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.hesvh.cn/Article/details/gyudvnqgu.sHtML

[F12] CSV 读写
来源：http://www.blog.fehbvm.com/Article/details/geiaqlksr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.zdbjq.cn/Article/details/gpywaknjk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.zdbjq.cn/Article/details/gkhxbxcpa.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.hesvh.cn/Article/details/gdqvmoehw.sHtML

TS:   // 同上
来源：http://blog.fehbvm.com/Article/details/gxwomzbyq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.zdbjq.cn/Article/details/gdsobkmbd.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.zdbjq.cn/Article/details/guvkmclff.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fehbvm.com/Article/details/ggiwqftrp.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fehbvm.com/Article/details/gpyjsazrx.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gsrhxoswr.sHtML

G. 面向对象
来源：http://baike.fehbvm.com/Article/details/goxejdclb.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gtnizufst.sHtML

[G01] 定义类
来源：http://wap.fehbvm.com/Article/details/gntuocoev.sHtML

Py:   class User: pass
来源：http://wap.hesvh.cn/Article/details/gxaffwgrh.sHtML

PHP:  class User {}
来源：http://www.m.share.hesvh.cn/Article/details/grpkldaeu.sHtML

JS:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gdzxgkssz.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.hesvh.cn/Article/details/giwkzvzgh.sHtML

Java: class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/giwevuuhi.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.zdbjq.cn/Article/details/gublvrzht.sHtML

Ruby: class User; end
来源：http://wap.zdbjq.cn/Article/details/grlkepgfh.sHtML

C#:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gcohnvwnv.sHtML

[G02] 构造函数
来源：http://m.share.fehbvm.com/Article/details/ghrlqvexd.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.hesvh.cn/Article/details/gtfwwvbfi.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fehbvm.com/Article/details/gyqlwrkal.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/ggdldbqhs.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.zdbjq.cn/Article/details/glscrmfwz.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gaaxysapj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.fehbvm.com/Article/details/gnwzjbnob.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.hesvh.cn/Article/details/gctjoisvm.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.zdbjq.cn/Article/details/ghbluxsmv.sHtML

[G03] 实例属性
来源：http://baike.hesvh.cn/Article/details/gpbqlmlsq.sHtML

Py:   self.name = "x"
来源：http://blog.hesvh.cn/Article/details/gtlsqagmq.sHtML

PHP:  public string $name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gaynzyonq.sHtML

JS:   this.name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gkiwxssdv.sHtML

TS:   name: string = "x";
来源：http://www.blog.hesvh.cn/Article/details/ginmghmao.sHtML

Java: private String name;
来源：http://wap.fehbvm.com/Article/details/gcyuupxlh.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.zdbjq.cn/Article/details/gxfankacu.sHtML

Ruby: @name = "x"
来源：http://wap.fehbvm.com/Article/details/gbmhjlmta.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.zdbjq.cn/Article/details/gkqsapekr.sHtML

[G04] 定义方法
来源：http://baike.fehbvm.com/Article/details/gtzkqyziz.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gtkzdnviz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/glxypenvd.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gsxkhjsdm.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gmrasazmt.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/groltuvvm.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gbzmqrqse.sHtML

Ruby: def greet; @name; end
来源：http://read.share.hesvh.cn/Article/details/gwxcqychk.sHtML

C#:   public string Greet() => Name;
来源：http://3g.hesvh.cn/Article/details/gsjfazyoy.sHtML

[G05] 继承
来源：http://mobile.fehbvm.com/Article/details/gkrcnszic.sHtML

Py:   class Admin(User): pass
来源：http://baike.zdbjq.cn/Article/details/gyxxlxjzu.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gnlvxhwwk.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghctuwife.sHtML

TS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gplfggzmk.sHtML

Java: class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gkyiixurr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.hesvh.cn/Article/details/gzptzlaov.sHtML

Ruby: class Admin < User; end
来源：http://mobile.zdbjq.cn/Article/details/gsyfulssd.sHtML

C#:   class Admin : User {}
来源：http://baike.zdbjq.cn/Article/details/gbklbeppc.sHtML

[G06] 重写方法
来源：http://3g.hesvh.cn/Article/details/gjhzfuyuv.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.zdbjq.cn/Article/details/ggdyuzrgg.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gldajdlli.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gphkbhamb.sHtML


<!-- 参考信息 -->