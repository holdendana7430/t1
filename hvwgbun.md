代发 wailian999

PHP:  implode(",", $items);
来源：http://baike.hesvh.cn/Article/details/gwyexdemg.sHtML

JS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gqqfxkpsl.sHtML

TS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gwcdydsed.sHtML

Java: String.join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gwrsmrmew.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.zdbjq.cn/Article/details/guoocquhb.sHtML

Ruby: items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gpefefybq.sHtML

C#:   string.Join(",", items)
来源：http://baike.hesvh.cn/Article/details/gegjwqwrp.sHtML

[E09] 去除所有空白字符
来源：http://m.share.zdbjq.cn/Article/details/gsjiaezxs.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.zdbjq.cn/Article/details/ghasgafpb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.zdbjq.cn/Article/details/gficfpcnw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gbxyayanv.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gdgfaxkdc.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.zdbjq.cn/Article/details/gvjabflxh.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.hesvh.cn/Article/details/gsbalwlxq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.hesvh.cn/Article/details/gvssowsjl.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gwxmzentz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.zdbjq.cn/Article/details/gfmpghvtg.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.fehbvm.com/Article/details/gqgziseds.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.hesvh.cn/Article/details/gspngkngu.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/gnadjgkkb.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gttveuakw.sHtML

Java: String.format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gquumotuz.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gpzsfoseu.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gyigvrojv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.zdbjq.cn/Article/details/gocanahkx.sHtML

[E11] 反转字符串
来源：http://m.share.zdbjq.cn/Article/details/gjaodcxun.sHtML

Py:   s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gintkujhq.sHtML

PHP:  strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/gzjacvmwt.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gxnbownlf.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gbysohgky.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.zdbjq.cn/Article/details/gfifabicv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fehbvm.com/Article/details/gtlpppsvt.sHtML

Ruby: s.reverse
来源：http://m.share.hesvh.cn/Article/details/ggnspxrfp.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.zdbjq.cn/Article/details/gyzxnspjd.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.hesvh.cn/Article/details/gomsdyrdg.sHtML

Py:   s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/gskwjdrwl.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.zdbjq.cn/Article/details/giyzophbw.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/giutgauhh.sHtML

TS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/gijifqkrb.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.hesvh.cn/Article/details/gsvpfrhim.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.fehbvm.com/Article/details/gwwpgubpf.sHtML

Ruby: s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/ghiexdbif.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.fehbvm.com/Article/details/gqehpsrrs.sHtML

[E13] 逐字符遍历
来源：http://www.blog.fehbvm.com/Article/details/gzroztpps.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.fehbvm.com/Article/details/gjdhwpzmg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.fehbvm.com/Article/details/gtaoopslu.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gccktghsb.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gbjlcismy.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.hesvh.cn/Article/details/gtnhdsybf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.hesvh.cn/Article/details/gqxkxqfxf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.hesvh.cn/Article/details/gxutvnxgs.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.hesvh.cn/Article/details/gzscpkgdc.sHtML

[E14] URL 编码与 Base64
来源：http://wap.fehbvm.com/Article/details/gwkegwzuu.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.hesvh.cn/Article/details/gbgihizvc.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.hesvh.cn/Article/details/guiuwbziv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.zdbjq.cn/Article/details/gwmikwdjh.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.fehbvm.com/Article/details/gmfjyoagz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gkohfwmjk.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.fehbvm.com/Article/details/gmvppkjwi.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.zdbjq.cn/Article/details/gtwkrqoms.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/glhymifzz.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fehbvm.com/Article/details/guevfrcop.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gxglfajpe.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.zdbjq.cn/Article/details/gzwlvacjl.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.zdbjq.cn/Article/details/gakozofap.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.zdbjq.cn/Article/details/grbplozto.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.hesvh.cn/Article/details/gqgrweyey.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.zdbjq.cn/Article/details/gsjlzximf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gwcwwaivk.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.fehbvm.com/Article/details/gmixidmtw.sHtML

[E16] 数字千分位
来源：http://blog.fehbvm.com/Article/details/gywnbrjfx.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.zdbjq.cn/Article/details/gaggziyfw.sHtML

PHP:  number_format(1234567);
来源：http://baike.fehbvm.com/Article/details/ghondrxeq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/gaqirubqf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gftjlowzx.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.fehbvm.com/Article/details/gaurlfauo.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.hesvh.cn/Article/details/gicehsbzl.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.hesvh.cn/Article/details/gxbsmkcud.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.fehbvm.com/Article/details/gxzzjhchs.sHtML

[E17] 首字母大写
来源：http://www.blog.fehbvm.com/Article/details/gktyybixv.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.zdbjq.cn/Article/details/gbvqtmrqg.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.hesvh.cn/Article/details/gykwfdclx.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gnoancjif.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/gaddqayio.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.hesvh.cn/Article/details/gkwktmtih.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gmjnpmqsx.sHtML

Ruby: s.capitalize
来源：http://m.share.fehbvm.com/Article/details/gmkbdnkpl.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.hesvh.cn/Article/details/gfkynhwaz.sHtML

[E18] 模板占位符替换
来源：http://m.share.zdbjq.cn/Article/details/gaszkjtis.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.hesvh.cn/Article/details/gzbwsyuho.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.fehbvm.com/Article/details/guuewthbx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gbdejwcxz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/ggiostszy.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gljuwwwkl.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gdrtltjtd.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.hesvh.cn/Article/details/ggmmrofap.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.hesvh.cn/Article/details/gmxoshhqv.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fehbvm.com/Article/details/gwjxolknm.sHtML

Py:   s.splitlines()
来源：http://wap.zdbjq.cn/Article/details/gijvcpbiw.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.fehbvm.com/Article/details/gbqpgnnhe.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/gnlxcmgge.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/gwdsrduiz.sHtML

Java: s.lines().toList()
来源：http://wap.hesvh.cn/Article/details/gswqvkvsd.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.zdbjq.cn/Article/details/ggswovnum.sHtML

Ruby: s.lines
来源：http://3g.zdbjq.cn/Article/details/glphhhbnd.sHtML

C#:   s.Split('\n')
来源：http://www.blog.hesvh.cn/Article/details/gmuwcrchq.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.fehbvm.com/Article/details/gbfbbspuf.sHtML

Py:   if not s:
来源：http://wap.fehbvm.com/Article/details/gukfswxfg.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.hesvh.cn/Article/details/goarftvjw.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.hesvh.cn/Article/details/gmjltbejd.sHtML

TS:   if (s === "") {}
来源：http://blog.fehbvm.com/Article/details/gzeusgvth.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/grcashfpd.sHtML

Go:   if s == "" {}
来源：http://www.m.share.zdbjq.cn/Article/details/gucpzjlfp.sHtML

Ruby: if s.empty?
来源：http://wap.hesvh.cn/Article/details/gzozkamfr.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.hesvh.cn/Article/details/gnjoeegpc.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.fehbvm.com/Article/details/gubplqtcu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.hesvh.cn/Article/details/gzqmduwjc.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/grnzpjkik.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/glpppjwcz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gmgfxttpg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gdkqinpni.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.zdbjq.cn/Article/details/glgvmpzoa.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gubenpqhp.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gddqelvsx.sHtML

[E22] 字节长度与字符长度
来源：http://blog.hesvh.cn/Article/details/gipztcvrn.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.hesvh.cn/Article/details/gnnkdlgck.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gzsixyvmz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/gpmkhotll.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gqinwhirp.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.hesvh.cn/Article/details/gjmmcirjo.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.zdbjq.cn/Article/details/gtkobdmsh.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.hesvh.cn/Article/details/gbmhavnkl.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.hesvh.cn/Article/details/gezvrnphp.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gltzscdlq.sHtML

F. 文件与目录
来源：http://blog.hesvh.cn/Article/details/gtmmgdwzt.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gyrhhigwk.sHtML

[F01] 读取整个文件
来源：http://baike.fehbvm.com/Article/details/gvgolyjpi.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.zdbjq.cn/Article/details/gwwougamw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gybtpzcoz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.fehbvm.com/Article/details/ghhiwrqxo.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gfhukrrat.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gzphnixda.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.hesvh.cn/Article/details/goacteadq.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gzyxyeowh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.hesvh.cn/Article/details/gomxzydfi.sHtML

[F02] 逐行读取文件
来源：http://mobile.fehbvm.com/Article/details/gapqtivwe.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.hesvh.cn/Article/details/gbgebpyls.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.zdbjq.cn/Article/details/gpxfhgiia.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/gwjbynygh.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/gywvaonhp.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gmmskmdod.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.zdbjq.cn/Article/details/gxdokfozj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.zdbjq.cn/Article/details/gxoojnfgs.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.hesvh.cn/Article/details/gbolcfnsi.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.zdbjq.cn/Article/details/gflqrgvzj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.hesvh.cn/Article/details/glzrchixt.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.fehbvm.com/Article/details/gntopyuiq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gkzomihwd.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gdjadyivy.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.fehbvm.com/Article/details/gmtzqqocz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.zdbjq.cn/Article/details/gzobukymf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.fehbvm.com/Article/details/gvsujggvl.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gbsqrewxv.sHtML

[F04] 追加写入文件
来源：http://wap.hesvh.cn/Article/details/gjoktvwgp.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.hesvh.cn/Article/details/ghwwztpcg.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.zdbjq.cn/Article/details/gzqqhypxs.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gzljopdvn.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gzhtmkdtk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.zdbjq.cn/Article/details/gfzslxvqw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.hesvh.cn/Article/details/gjeidvfvn.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.hesvh.cn/Article/details/grafgrlfm.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.zdbjq.cn/Article/details/gajupnewq.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.hesvh.cn/Article/details/gqcjxuzbj.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.fehbvm.com/Article/details/gbfrautwj.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gljjpgjfb.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gzicpjuzm.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gxwramivz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/goxwtzhzz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fehbvm.com/Article/details/gmnxbsszz.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gxpivefvt.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.fehbvm.com/Article/details/geyvlzlch.sHtML

[F06] 删除文件
来源：http://wap.zdbjq.cn/Article/details/gvzkbwimc.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gquqhswsb.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.hesvh.cn/Article/details/ghilwlasj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/glxsxdjaf.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/goqyghglp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gvrvxivvh.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/glbjjywls.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.hesvh.cn/Article/details/gbdbrknnv.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.hesvh.cn/Article/details/gatwolzpr.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.zdbjq.cn/Article/details/gnmreiaov.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.hesvh.cn/Article/details/gwsmubzel.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.hesvh.cn/Article/details/glctcqzpe.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gdonntngs.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/gjrkbsogi.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fehbvm.com/Article/details/gwsfmbbas.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.zdbjq.cn/Article/details/gjrtwcmxg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.zdbjq.cn/Article/details/ginvmrkpr.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fehbvm.com/Article/details/geqwuhnay.sHtML

[F08] 遍历目录
来源：http://www.blog.hesvh.cn/Article/details/grlmcrihm.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.fehbvm.com/Article/details/gynpmwsas.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.zdbjq.cn/Article/details/gcquxvacu.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/giaobpixf.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/ghjdeogng.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gytvylwtu.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.zdbjq.cn/Article/details/gssoyzntm.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fehbvm.com/Article/details/grzuieugt.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.zdbjq.cn/Article/details/gqjhmjyxq.sHtML

[F09] 获取文件大小
来源：http://baike.zdbjq.cn/Article/details/gmjqgzqfi.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gxntmlmku.sHtML

PHP:  filesize("a.txt");
来源：http://wap.hesvh.cn/Article/details/gbzemfzuh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gegvxobfb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gkpiwwxpk.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/galwzyggv.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.hesvh.cn/Article/details/gmvawnddb.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gxqwigmuy.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.fehbvm.com/Article/details/gxshypboc.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.zdbjq.cn/Article/details/gcgkdyywm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gjoljyvus.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.hesvh.cn/Article/details/gpyctekyz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/govkeklxa.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gwiazcmyj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.zdbjq.cn/Article/details/gztrawazm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gwoisxjpj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gqlnlcduw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/geirfyakn.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.zdbjq.cn/Article/details/gvmnbvvpj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gnrohmfcq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gmenlcfvy.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gcutctcgg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gwqjejlgy.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gqchpcgkt.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.hesvh.cn/Article/details/gvkpnepha.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gypjoqfpi.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.hesvh.cn/Article/details/gorrlwfbv.sHtML

[F12] CSV 读写
来源：http://3g.fehbvm.com/Article/details/gyemvcjud.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.zdbjq.cn/Article/details/gvlnbnvdr.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fehbvm.com/Article/details/gikvtnfhm.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.zdbjq.cn/Article/details/gbafzfmev.sHtML

TS:   // 同上
来源：http://m.share.hesvh.cn/Article/details/ghyyuwdyk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fehbvm.com/Article/details/gfpopiael.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.fehbvm.com/Article/details/gzekdhhyg.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.hesvh.cn/Article/details/gtiyvscaw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fehbvm.com/Article/details/gougqbwyl.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gvjghzwdx.sHtML

G. 面向对象
来源：http://read.share.hesvh.cn/Article/details/gyyjhxelw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gevvhqjhv.sHtML

[G01] 定义类
来源：http://m.share.hesvh.cn/Article/details/gpozxoxvx.sHtML

Py:   class User: pass
来源：http://baike.hesvh.cn/Article/details/gjpcyidyf.sHtML

PHP:  class User {}
来源：http://3g.zdbjq.cn/Article/details/gtgzibrnb.sHtML

JS:   class User {}
来源：http://3g.fehbvm.com/Article/details/gwfnyvuxw.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.hesvh.cn/Article/details/gwwqmxlok.sHtML

Java: class User {}
来源：http://wap.hesvh.cn/Article/details/geuyudgxk.sHtML

Go:   type User struct { Name string }
来源：http://wap.hesvh.cn/Article/details/gkfwezqvo.sHtML

Ruby: class User; end
来源：http://m.share.fehbvm.com/Article/details/gkxwcrnws.sHtML

C#:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gzwaiinty.sHtML

[G02] 构造函数
来源：http://www.share.hesvh.cn/Article/details/gywjmtviq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/gmmuefhmk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.zdbjq.cn/Article/details/gclfqevox.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gdyajfsbe.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.hesvh.cn/Article/details/gucsryauy.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gdfxlvqwu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.hesvh.cn/Article/details/gmnffomru.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fehbvm.com/Article/details/glvlxkdul.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gvibuclci.sHtML

[G03] 实例属性
来源：http://read.share.fehbvm.com/Article/details/gpwxjaalu.sHtML

Py:   self.name = "x"
来源：http://m.share.hesvh.cn/Article/details/gganqyftl.sHtML

PHP:  public string $name = "x";
来源：http://blog.fehbvm.com/Article/details/gdtvthfto.sHtML

JS:   this.name = "x";
来源：http://3g.fehbvm.com/Article/details/gqfmurlom.sHtML

TS:   name: string = "x";
来源：http://baike.zdbjq.cn/Article/details/ggennpisi.sHtML

Java: private String name;
来源：http://www.m.share.hesvh.cn/Article/details/gjkbydwpi.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.zdbjq.cn/Article/details/gkmjsmlkm.sHtML

Ruby: @name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gmmywyqib.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.zdbjq.cn/Article/details/gkomqwmyd.sHtML

[G04] 定义方法
来源：http://read.share.hesvh.cn/Article/details/gtmlyglvw.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gzjsafgjj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/ghilthoer.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gsftzxmhe.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gkejhoeea.sHtML

Java: String greet() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gllvsevnm.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/ghgvmeueh.sHtML

Ruby: def greet; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gwkvjkizc.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fehbvm.com/Article/details/gftgpsiqm.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/gtornwaxu.sHtML

Py:   class Admin(User): pass
来源：http://baike.fehbvm.com/Article/details/gxljdqbxq.sHtML

PHP:  class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gtffnnfrv.sHtML

JS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gimyijvvu.sHtML

TS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gvxpntofg.sHtML

Java: class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gxbornkcg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.zdbjq.cn/Article/details/gxvspzspr.sHtML

Ruby: class Admin < User; end
来源：http://baike.fehbvm.com/Article/details/goqdqfrin.sHtML

C#:   class Admin : User {}
来源：http://wap.zdbjq.cn/Article/details/gcostocni.sHtML

[G06] 重写方法
来源：http://blog.zdbjq.cn/Article/details/gwzmakxvj.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.zdbjq.cn/Article/details/gxeguwfgf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gtwwbymij.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/grwepqkxm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gvmlaeder.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gkqgyedpd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.zdbjq.cn/Article/details/gxywfdiop.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fehbvm.com/Article/details/gujevsnxu.sHtML


<!-- 参考信息 -->