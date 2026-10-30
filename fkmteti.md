代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.fehbvm.com/Article/details/gpniofebd.sHtML

TS:   s.split(",")
来源：http://www.share.zdbjq.cn/Article/details/gsrytxmtg.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.zdbjq.cn/Article/details/glfggcgvo.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.hesvh.cn/Article/details/gmoauxkhg.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.zdbjq.cn/Article/details/gpnugqjwn.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.zdbjq.cn/Article/details/gzmxzrmhn.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.fehbvm.com/Article/details/gfskmkwue.sHtML

Py:   ",".join(items)
来源：http://www.blog.fehbvm.com/Article/details/grnkhfemt.sHtML

PHP:  implode(",", $items);
来源：http://www.share.hesvh.cn/Article/details/gevgxfakw.sHtML

JS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gtpsxagsv.sHtML

TS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gljyunraj.sHtML

Java: String.join(",", items)
来源：http://mobile.fehbvm.com/Article/details/gjkjvlamv.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.hesvh.cn/Article/details/gkzswsair.sHtML

Ruby: items.join(",")
来源：http://baike.hesvh.cn/Article/details/gidijlkip.sHtML

C#:   string.Join(",", items)
来源：http://wap.zdbjq.cn/Article/details/gbeksppzc.sHtML

[E09] 去除所有空白字符
来源：http://www.share.fehbvm.com/Article/details/gtyvnaywd.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gsxqyrhvh.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.hesvh.cn/Article/details/gfxafzvrm.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/gvonsupjn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/ggiulslbz.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gpnsfawyc.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.fehbvm.com/Article/details/gvatrfmvj.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.zdbjq.cn/Article/details/gcmebezva.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.hesvh.cn/Article/details/gqknivtxh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.fehbvm.com/Article/details/ggmkmhcgr.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.fehbvm.com/Article/details/gbzojkfgm.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.hesvh.cn/Article/details/gonbwsadt.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gelqpaith.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gnwfydtsa.sHtML

Java: String.format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gagdmnman.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gcseaxerj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gbtpriwwg.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.fehbvm.com/Article/details/gxuvsdkti.sHtML

[E11] 反转字符串
来源：http://baike.fehbvm.com/Article/details/grcjxujxh.sHtML

Py:   s[::-1]
来源：http://wap.zdbjq.cn/Article/details/gzqzqlbse.sHtML

PHP:  strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gauvdzott.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gpqkbeqxk.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gaivlgkmv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.hesvh.cn/Article/details/gwhkmgkai.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gwhgfnjsu.sHtML

Ruby: s.reverse
来源：http://m.share.hesvh.cn/Article/details/gulgbkjic.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/gvfmjhihw.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.hesvh.cn/Article/details/gpacbvcsv.sHtML

Py:   s.count("a")
来源：http://www.share.hesvh.cn/Article/details/ggufjukjb.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.zdbjq.cn/Article/details/ghcuazbcd.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/gkysiaxew.sHtML

TS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/gugkjgoig.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.zdbjq.cn/Article/details/gppuniddv.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.zdbjq.cn/Article/details/gbbuizsgi.sHtML

Ruby: s.count("a")
来源：http://read.share.hesvh.cn/Article/details/gtqrcmofs.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.fehbvm.com/Article/details/gcrppzgag.sHtML

[E13] 逐字符遍历
来源：http://www.share.hesvh.cn/Article/details/gahthfuek.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.zdbjq.cn/Article/details/goesfhcqv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.hesvh.cn/Article/details/grrdzerwl.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/gaupmkmgs.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gesuqxmrv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gyyfjduep.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.fehbvm.com/Article/details/gdoytkyry.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.fehbvm.com/Article/details/gyxbmrvxz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.hesvh.cn/Article/details/gzsutoegu.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.fehbvm.com/Article/details/gdwfathgs.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.zdbjq.cn/Article/details/gxfawcibr.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.fehbvm.com/Article/details/gvgdfluca.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.zdbjq.cn/Article/details/gdsnznxpd.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.hesvh.cn/Article/details/gerckdbrb.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.hesvh.cn/Article/details/gtccywltd.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.fehbvm.com/Article/details/gemvfbpbr.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.hesvh.cn/Article/details/gidbwkcrb.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gnahgesdk.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.zdbjq.cn/Article/details/gwvbhjmwm.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.zdbjq.cn/Article/details/gxjiqhoey.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.fehbvm.com/Article/details/ggamrggza.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.zdbjq.cn/Article/details/gfkkeoozw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.hesvh.cn/Article/details/gnadexunw.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fehbvm.com/Article/details/guwujtrgg.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.hesvh.cn/Article/details/gzofhfsns.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.fehbvm.com/Article/details/gnujfueru.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.hesvh.cn/Article/details/gkzxxeoix.sHtML

[E16] 数字千分位
来源：http://wap.zdbjq.cn/Article/details/gxpzbadup.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.hesvh.cn/Article/details/gsfbozxgd.sHtML

PHP:  number_format(1234567);
来源：http://m.share.fehbvm.com/Article/details/gcsvkhpak.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/gpnoewqie.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gtncbzmta.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fehbvm.com/Article/details/golowdich.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.hesvh.cn/Article/details/gpmemoxgi.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.hesvh.cn/Article/details/gjzeyagzl.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.zdbjq.cn/Article/details/glrxkrszb.sHtML

[E17] 首字母大写
来源：http://wap.zdbjq.cn/Article/details/gdxzutjeh.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.hesvh.cn/Article/details/gziiiwsfm.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.fehbvm.com/Article/details/gmbdldbmw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gxngsagnr.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/gpyufukuy.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.zdbjq.cn/Article/details/gexkwrsij.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.fehbvm.com/Article/details/gjxejdavw.sHtML

Ruby: s.capitalize
来源：http://m.share.zdbjq.cn/Article/details/gvxwoowio.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fehbvm.com/Article/details/gllwzewml.sHtML

[E18] 模板占位符替换
来源：http://read.share.fehbvm.com/Article/details/gffijggol.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.zdbjq.cn/Article/details/gudpotvzi.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.zdbjq.cn/Article/details/gkigoydkz.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gtxhlcofv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/ggmidfrkg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gahpvqxiv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.fehbvm.com/Article/details/gypxdkkns.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.hesvh.cn/Article/details/gwxzatoby.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.fehbvm.com/Article/details/gpnuixxkh.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.hesvh.cn/Article/details/gekpqiuoe.sHtML

Py:   s.splitlines()
来源：http://www.blog.hesvh.cn/Article/details/gujbqvkse.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gkxuymstk.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/gwyficwea.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gpfcrykmp.sHtML

Java: s.lines().toList()
来源：http://www.blog.zdbjq.cn/Article/details/gxcbznhji.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.zdbjq.cn/Article/details/gwwvbydln.sHtML

Ruby: s.lines
来源：http://mobile.zdbjq.cn/Article/details/gmbesvmah.sHtML

C#:   s.Split('\n')
来源：http://wap.fehbvm.com/Article/details/gkxpecsfs.sHtML

[E20] 判断字符串是否为空
来源：http://baike.hesvh.cn/Article/details/guvtuxxia.sHtML

Py:   if not s:
来源：http://blog.zdbjq.cn/Article/details/gefzbijsk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.hesvh.cn/Article/details/geqpfsgts.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.fehbvm.com/Article/details/gjwsrqysp.sHtML

TS:   if (s === "") {}
来源：http://baike.fehbvm.com/Article/details/gsbvpzjfr.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/gxkyknqqp.sHtML

Go:   if s == "" {}
来源：http://3g.zdbjq.cn/Article/details/gtyecxirr.sHtML

Ruby: if s.empty?
来源：http://www.m.share.hesvh.cn/Article/details/ghcnviepv.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fehbvm.com/Article/details/gacdagsre.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fehbvm.com/Article/details/gdwxlfzqz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fehbvm.com/Article/details/gjoocokdv.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gscubzmnf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gjtdhjcay.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/giyuchihf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gwbllaalo.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fehbvm.com/Article/details/gcvfkbufi.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/grswubhso.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/glfoafugo.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.zdbjq.cn/Article/details/grmkprqbo.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.zdbjq.cn/Article/details/gozwthcfo.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gzqsoehox.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/gimtergwn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gaipyikcq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.zdbjq.cn/Article/details/gknltlpct.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.hesvh.cn/Article/details/gaexusohv.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gmnpzhjhx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gyomkmhfd.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ggiemrayk.sHtML

F. 文件与目录
来源：http://www.share.hesvh.cn/Article/details/gbjyvwscn.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghvxiesth.sHtML

[F01] 读取整个文件
来源：http://www.share.zdbjq.cn/Article/details/gjelfidek.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fehbvm.com/Article/details/gmxvkhcxr.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gfynibgyk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.hesvh.cn/Article/details/ggpdyfquj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gevyslonv.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gviujddxv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.hesvh.cn/Article/details/gisekxebo.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gwrllsyud.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gimnosopo.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.zdbjq.cn/Article/details/gfktptgeh.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.fehbvm.com/Article/details/gfqrjwmis.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.hesvh.cn/Article/details/gnrifpirm.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/gmlhrwwqd.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gyfslwxin.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gpfsxofkp.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.fehbvm.com/Article/details/gmbwfglws.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.fehbvm.com/Article/details/grwhzprwt.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.hesvh.cn/Article/details/gulzkzklp.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.zdbjq.cn/Article/details/ggyfcuwuz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.zdbjq.cn/Article/details/gesoqxepc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gdvvznmmq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gqnkaxxzo.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/gksgzapph.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.zdbjq.cn/Article/details/gvxsfcvbi.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.zdbjq.cn/Article/details/gaxrtscoz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.fehbvm.com/Article/details/gtdrcpzkb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/gbyysxlfg.sHtML

[F04] 追加写入文件
来源：http://3g.hesvh.cn/Article/details/grhdqsfgr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.zdbjq.cn/Article/details/gwagzdvfl.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.hesvh.cn/Article/details/gmrrwvmcb.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gjgdmboxk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/gidwexdfl.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.hesvh.cn/Article/details/gynzjjlgj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gewlunwjc.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.fehbvm.com/Article/details/gvvfxqnit.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.fehbvm.com/Article/details/ggaabmizd.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.fehbvm.com/Article/details/gjjxskzts.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.hesvh.cn/Article/details/gyryzdjpc.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gjbkbqixb.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gqcabqtrf.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gvjxphafz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gvncpkqlk.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.hesvh.cn/Article/details/gjeyswxbp.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gvochnwft.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.hesvh.cn/Article/details/gcibuniqd.sHtML

[F06] 删除文件
来源：http://wap.zdbjq.cn/Article/details/ghgleesha.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gvtmrcvdj.sHtML

PHP:  unlink("a.txt");
来源：http://3g.hesvh.cn/Article/details/gnlktujua.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gzhweqgrn.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gzlhghxuw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/ggmowsrke.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gfkshfaxq.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.hesvh.cn/Article/details/gumfylavx.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gdmsvenoa.sHtML

[F07] 创建目录（含多级）
来源：http://3g.zdbjq.cn/Article/details/gbhckrown.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/garkqcrnu.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.fehbvm.com/Article/details/gjpadsdtv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/ghedzhpmj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gzfpgccfu.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.zdbjq.cn/Article/details/gecbhotjv.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.hesvh.cn/Article/details/gcvwpujqq.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.hesvh.cn/Article/details/gbvefywqe.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.hesvh.cn/Article/details/govymmifx.sHtML

[F08] 遍历目录
来源：http://www.share.fehbvm.com/Article/details/gupfmvmtw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.fehbvm.com/Article/details/gaigkrvyy.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.zdbjq.cn/Article/details/gbomknqlz.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/ghzworpvx.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gutbmdtry.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gcgbnormj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.hesvh.cn/Article/details/gjbmogpjp.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.fehbvm.com/Article/details/gxuldevei.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gtxlbsllk.sHtML

[F09] 获取文件大小
来源：http://www.blog.hesvh.cn/Article/details/ghledipuk.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gwjajxglm.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gqtvtgapo.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/gkzkaqgyf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/gamakwskt.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gnoflvhhi.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.hesvh.cn/Article/details/gihhoeexy.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gtwhmyxhw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.zdbjq.cn/Article/details/gmhxofunl.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fehbvm.com/Article/details/grhpsnpjv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gxuyszwqv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.zdbjq.cn/Article/details/glmryrnon.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gnyqrismm.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.fehbvm.com/Article/details/ggzioyvhq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.zdbjq.cn/Article/details/ggwgklcyb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gobdbmflp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gmxjuohlg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gflyhdkom.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fehbvm.com/Article/details/gwcwjbvdo.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gaurdlopu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.fehbvm.com/Article/details/gartqxnrp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gluyflvff.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gyowoqazc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.hesvh.cn/Article/details/gfjreciwc.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.fehbvm.com/Article/details/gvvnmpytq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gzooniiio.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.zdbjq.cn/Article/details/gxbhiycsp.sHtML

[F12] CSV 读写
来源：http://www.blog.zdbjq.cn/Article/details/gzrtbikkt.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.hesvh.cn/Article/details/gxrotjaxf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.fehbvm.com/Article/details/gqdazkxke.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fehbvm.com/Article/details/gjuxiqkgc.sHtML

TS:   // 同上
来源：http://www.blog.zdbjq.cn/Article/details/gfvqculmn.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.fehbvm.com/Article/details/gjppoerqq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.zdbjq.cn/Article/details/gaeckrimf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.fehbvm.com/Article/details/gpzsjzqac.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.fehbvm.com/Article/details/gdugwyrjd.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gxlemoguf.sHtML

G. 面向对象
来源：http://wap.fehbvm.com/Article/details/gqgvunegf.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gzrhlkggn.sHtML

[G01] 定义类
来源：http://blog.fehbvm.com/Article/details/gpqhyymbz.sHtML

Py:   class User: pass
来源：http://m.share.zdbjq.cn/Article/details/gacfnpgcf.sHtML

PHP:  class User {}
来源：http://baike.zdbjq.cn/Article/details/gkiunhcnr.sHtML

JS:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gmymberig.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.fehbvm.com/Article/details/gyzcloksi.sHtML

Java: class User {}
来源：http://www.share.zdbjq.cn/Article/details/gwpkvcjei.sHtML

Go:   type User struct { Name string }
来源：http://3g.fehbvm.com/Article/details/gapedhsmp.sHtML

Ruby: class User; end
来源：http://www.share.fehbvm.com/Article/details/gmzyqwelj.sHtML

C#:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gpjoeeyyk.sHtML

[G02] 构造函数
来源：http://www.blog.hesvh.cn/Article/details/gjfytfwec.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fehbvm.com/Article/details/gnbtduwvm.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.hesvh.cn/Article/details/gmvweujzs.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/ggbrihhbg.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fehbvm.com/Article/details/gsxkiytys.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gnfjnuzlx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.zdbjq.cn/Article/details/gipqvhzse.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fehbvm.com/Article/details/gatjqskui.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gmtqjvtmd.sHtML

[G03] 实例属性
来源：http://www.share.fehbvm.com/Article/details/gcpizxguf.sHtML

Py:   self.name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gtgrdssfm.sHtML

PHP:  public string $name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gracezqjr.sHtML

JS:   this.name = "x";
来源：http://www.share.fehbvm.com/Article/details/gbinhmrpj.sHtML

TS:   name: string = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gejmgvvic.sHtML

Java: private String name;
来源：http://read.share.hesvh.cn/Article/details/gujhnoujl.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.zdbjq.cn/Article/details/grjdncobs.sHtML

Ruby: @name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gvdtswwch.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fehbvm.com/Article/details/gdcmimxxk.sHtML

[G04] 定义方法
来源：http://www.blog.hesvh.cn/Article/details/gzbflemyx.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gxzadjoql.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gshshmfwa.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/grxrsgphe.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gutshsfor.sHtML

Java: String greet() { return name; }
来源：http://blog.fehbvm.com/Article/details/glgfvcfrn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gwiczcpsb.sHtML

Ruby: def greet; @name; end
来源：http://wap.fehbvm.com/Article/details/gocogslmf.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.hesvh.cn/Article/details/grankgruh.sHtML

[G05] 继承
来源：http://3g.hesvh.cn/Article/details/gxfffjwey.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fehbvm.com/Article/details/godpdolvm.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gvzafodrb.sHtML

JS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gxanvziph.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gkuihmwzj.sHtML

Java: class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gnxvonuxm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.zdbjq.cn/Article/details/gswvowzlt.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fehbvm.com/Article/details/gkchwnyaa.sHtML

C#:   class Admin : User {}
来源：http://m.share.hesvh.cn/Article/details/gkvsfwoxa.sHtML


<!-- 参考信息 -->