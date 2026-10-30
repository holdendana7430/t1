代发 wailian999

Ruby: s.split(",");  s.split
来源：http://3g.fehbvm.com/Article/details/gnomentdh.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.zdbjq.cn/Article/details/gmolmqavy.sHtML

[E08] 数组按分隔符合并
来源：http://3g.hesvh.cn/Article/details/gropsnvha.sHtML

Py:   ",".join(items)
来源：http://3g.hesvh.cn/Article/details/gcddgqfmq.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.hesvh.cn/Article/details/ggupfabil.sHtML

JS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gcgjmfeke.sHtML

TS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/gcgmafogb.sHtML

Java: String.join(",", items)
来源：http://blog.zdbjq.cn/Article/details/gkctjogry.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.fehbvm.com/Article/details/gcgdiykwn.sHtML

Ruby: items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gnbmtempe.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/geyjygsjx.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.zdbjq.cn/Article/details/gutjgvbfj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.zdbjq.cn/Article/details/gcvraazav.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.hesvh.cn/Article/details/gvptkirsk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/ghaedfhnl.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gtedzfhti.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.zdbjq.cn/Article/details/glopfijfe.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.hesvh.cn/Article/details/gozwcbbah.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.fehbvm.com/Article/details/gsxwadari.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.fehbvm.com/Article/details/grcpqljtj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.hesvh.cn/Article/details/gxrehviue.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gwunxzxgw.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fehbvm.com/Article/details/gnhiccosf.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gbhkqekde.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gtwyppoqa.sHtML

Java: String.format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gekjqebwo.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gbudjpezp.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gbtfwsyhy.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.zdbjq.cn/Article/details/gesfpdpxp.sHtML

[E11] 反转字符串
来源：http://m.share.zdbjq.cn/Article/details/gonnihqry.sHtML

Py:   s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gjfcjyusk.sHtML

PHP:  strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gkwbtjtfv.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gevsgtdkx.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gtrluianj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.hesvh.cn/Article/details/ggffthwzf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.zdbjq.cn/Article/details/gymuqzonb.sHtML

Ruby: s.reverse
来源：http://baike.zdbjq.cn/Article/details/gtpndyptr.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/gbjayaliv.sHtML

[E12] 统计某字符出现次数
来源：http://3g.zdbjq.cn/Article/details/gvdsxnudn.sHtML

Py:   s.count("a")
来源：http://baike.fehbvm.com/Article/details/gwmcrhuam.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.hesvh.cn/Article/details/gzpcolqio.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/glmcjmixm.sHtML

TS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/gysdctvnd.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.zdbjq.cn/Article/details/gyrbixyqo.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.hesvh.cn/Article/details/gdzstouab.sHtML

Ruby: s.count("a")
来源：http://3g.fehbvm.com/Article/details/gvbdlutzr.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.hesvh.cn/Article/details/grccdzwuv.sHtML

[E13] 逐字符遍历
来源：http://wap.hesvh.cn/Article/details/gjgelcwzk.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.zdbjq.cn/Article/details/gvkeijasx.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjmnkdabp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/glhblbxjc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gyvyjsben.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.zdbjq.cn/Article/details/glopbeqog.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.hesvh.cn/Article/details/gyvyxevlw.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.hesvh.cn/Article/details/gknyoliwn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.zdbjq.cn/Article/details/gonwcwqca.sHtML

[E14] URL 编码与 Base64
来源：http://blog.zdbjq.cn/Article/details/gbqaslcqs.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.hesvh.cn/Article/details/gabtwhenw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.hesvh.cn/Article/details/gkcoizhoi.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.zdbjq.cn/Article/details/gugblpuzc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.hesvh.cn/Article/details/gladtdzrd.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.hesvh.cn/Article/details/ghchrucyv.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.fehbvm.com/Article/details/gzyjpatrs.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.fehbvm.com/Article/details/gvibxszqe.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.fehbvm.com/Article/details/guwikegmp.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.zdbjq.cn/Article/details/gusejwybv.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.fehbvm.com/Article/details/gpdrghztw.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gpwfhwcah.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.hesvh.cn/Article/details/gtfkzeluo.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.hesvh.cn/Article/details/gckvxdwfw.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.fehbvm.com/Article/details/gotfbzhif.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.fehbvm.com/Article/details/gyzwivtdn.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.hesvh.cn/Article/details/gkyquffic.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.fehbvm.com/Article/details/giagpetra.sHtML

[E16] 数字千分位
来源：http://read.share.zdbjq.cn/Article/details/gaquiaewr.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.hesvh.cn/Article/details/gcqisfuyq.sHtML

PHP:  number_format(1234567);
来源：http://www.share.zdbjq.cn/Article/details/gjpesssjb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/gdvfsggnx.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/geqnlnkaw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.fehbvm.com/Article/details/ggmuuduiv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.hesvh.cn/Article/details/gxfjyaybo.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.zdbjq.cn/Article/details/getgjccgy.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.hesvh.cn/Article/details/gztbxshcb.sHtML

[E17] 首字母大写
来源：http://www.share.hesvh.cn/Article/details/gyousvovp.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.hesvh.cn/Article/details/geeaahtxi.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.fehbvm.com/Article/details/gmwvmbblx.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gzhqpoqwy.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gpfozvsxj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.zdbjq.cn/Article/details/gazrtnwfc.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/ggosokybd.sHtML

Ruby: s.capitalize
来源：http://www.blog.zdbjq.cn/Article/details/gzdmluqfg.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.hesvh.cn/Article/details/gsyfqqnhm.sHtML

[E18] 模板占位符替换
来源：http://www.share.fehbvm.com/Article/details/gpfurfljc.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.zdbjq.cn/Article/details/gvnsfsesu.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.fehbvm.com/Article/details/gufhybvda.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gownkipua.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gnbwypayp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gprmmddoy.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gfdutwcrc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.zdbjq.cn/Article/details/ghjjdxdln.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.hesvh.cn/Article/details/gzgcsvors.sHtML

[E19] 多行文本按行拆分
来源：http://wap.fehbvm.com/Article/details/gtieumura.sHtML

Py:   s.splitlines()
来源：http://www.blog.zdbjq.cn/Article/details/gpbjkvuqn.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.fehbvm.com/Article/details/gglkxxfng.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gxchhktbt.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/gbaelzdjx.sHtML

Java: s.lines().toList()
来源：http://blog.fehbvm.com/Article/details/gdsfulxgt.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.fehbvm.com/Article/details/giytijthp.sHtML

Ruby: s.lines
来源：http://m.share.hesvh.cn/Article/details/gmvyyffac.sHtML

C#:   s.Split('\n')
来源：http://www.blog.hesvh.cn/Article/details/gpgfncdps.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.zdbjq.cn/Article/details/gnfmmznbp.sHtML

Py:   if not s:
来源：http://wap.zdbjq.cn/Article/details/gglxjmvmj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.zdbjq.cn/Article/details/gmdiavprg.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.fehbvm.com/Article/details/gyymvfygi.sHtML

TS:   if (s === "") {}
来源：http://3g.zdbjq.cn/Article/details/gdopclxuo.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gbsoxvuts.sHtML

Go:   if s == "" {}
来源：http://baike.zdbjq.cn/Article/details/ghqsnzqsw.sHtML

Ruby: if s.empty?
来源：http://www.share.hesvh.cn/Article/details/gpfelismy.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.hesvh.cn/Article/details/gjgxsentq.sHtML

[E21] 超长截断加省略号
来源：http://blog.zdbjq.cn/Article/details/gnofjlpjq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.zdbjq.cn/Article/details/glujtlepy.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gswebewll.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gstxgjaoe.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gnebrmkre.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gryqxsljd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.zdbjq.cn/Article/details/gdgnnfrxw.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gljebdrqu.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gbtotanby.sHtML

[E22] 字节长度与字符长度
来源：http://baike.zdbjq.cn/Article/details/gpdnyptvm.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.zdbjq.cn/Article/details/gldkaslzz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gdnqhaajr.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/glvrsdkzd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gsxiezsce.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.hesvh.cn/Article/details/ghhopxpoz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fehbvm.com/Article/details/gurlptrmo.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gwwrgooey.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.hesvh.cn/Article/details/gkeblmgdx.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gpjzlmicu.sHtML

F. 文件与目录
来源：http://3g.fehbvm.com/Article/details/grotxiggc.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxouphyjs.sHtML

[F01] 读取整个文件
来源：http://www.blog.fehbvm.com/Article/details/gmaumoeki.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.zdbjq.cn/Article/details/giewwgvpe.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gfpqleqco.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.zdbjq.cn/Article/details/ggobtayoi.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gtymqbiki.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gkvukzsey.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.hesvh.cn/Article/details/gelhvehpk.sHtML

Ruby: File.read("a.txt")
来源：http://3g.hesvh.cn/Article/details/gayurkhfi.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/guxqfggin.sHtML

[F02] 逐行读取文件
来源：http://www.share.zdbjq.cn/Article/details/gpothnwcy.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.zdbjq.cn/Article/details/gpumtgzvs.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/glrbdahrr.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gtrmzyvcx.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gfwbskzte.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/goaegwlfq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.fehbvm.com/Article/details/gnkvpmbvm.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.fehbvm.com/Article/details/gshssxnsz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.hesvh.cn/Article/details/gdbvqpqoj.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fehbvm.com/Article/details/gvyjnammu.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.hesvh.cn/Article/details/gxhxqmhff.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gsxosdqtj.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/gsakzfadu.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/ghzftyqbp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.fehbvm.com/Article/details/gxdqpnefl.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.hesvh.cn/Article/details/gymkzinuv.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.zdbjq.cn/Article/details/ghpakyfeb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gfqqksdmv.sHtML

[F04] 追加写入文件
来源：http://www.blog.fehbvm.com/Article/details/giwyibeyz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.hesvh.cn/Article/details/gqhhvfmyb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.hesvh.cn/Article/details/gbuvbyihz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gggjfregl.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gpehfsfmf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.zdbjq.cn/Article/details/gobstozfu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gfjeznuml.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.fehbvm.com/Article/details/gpfccwxgz.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.zdbjq.cn/Article/details/gaqxtfulo.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.zdbjq.cn/Article/details/gfbdxsxqr.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.zdbjq.cn/Article/details/gbiotoogw.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fehbvm.com/Article/details/gmgcmyxxs.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gskwaeilo.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/ggmvgnuje.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/grtmvqgtk.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.zdbjq.cn/Article/details/ggxwfopee.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gsptqjslw.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gjspcheni.sHtML

[F06] 删除文件
来源：http://wap.fehbvm.com/Article/details/goooxgeig.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gcgahywnh.sHtML

PHP:  unlink("a.txt");
来源：http://blog.hesvh.cn/Article/details/gjcbxnhtu.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/ghzmyuyuf.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gdwstlfuq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/ggfskczjv.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/ggwildxxs.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gkdsgdsyp.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gftmydhgb.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.hesvh.cn/Article/details/gjvhxuojw.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gldbbrxcy.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.zdbjq.cn/Article/details/gppxnmoda.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/grjvdswoh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/gtxagdefb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.zdbjq.cn/Article/details/gpzqhnpkk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.fehbvm.com/Article/details/gmxxljfos.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.fehbvm.com/Article/details/gfapzwfyy.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.hesvh.cn/Article/details/gttbesjfl.sHtML

[F08] 遍历目录
来源：http://read.share.hesvh.cn/Article/details/gdksjssuk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.hesvh.cn/Article/details/gbvrdtkom.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.fehbvm.com/Article/details/gxqqsmnmx.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/gvfijzivg.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/gwdwvclgq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/gjidlomom.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.zdbjq.cn/Article/details/gntlouwwh.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fehbvm.com/Article/details/gbvvapvtm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fehbvm.com/Article/details/gocwweedj.sHtML

[F09] 获取文件大小
来源：http://www.share.hesvh.cn/Article/details/gfwuxtbak.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.hesvh.cn/Article/details/gqylyrdod.sHtML

PHP:  filesize("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gkuhkwxmm.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/gqroinact.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gsiwdrrdg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gwkrymnrh.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.hesvh.cn/Article/details/gnknzfzws.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gouourity.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.fehbvm.com/Article/details/gydtiqmzo.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.hesvh.cn/Article/details/gahpiigjw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gvcntrthq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.fehbvm.com/Article/details/gwgonksbx.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gljsanhex.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.hesvh.cn/Article/details/ghfqyksma.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.zdbjq.cn/Article/details/gwnanlynp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gpaqdiruz.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gzpwlukmk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/guvomegri.sHtML

[F11] 复制与移动文件
来源：http://wap.zdbjq.cn/Article/details/gzleovdbc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gikgkbctd.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.fehbvm.com/Article/details/gpwindpou.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/guaewrozf.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gjcmxhsth.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.hesvh.cn/Article/details/gzkcismcr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.zdbjq.cn/Article/details/gvzdlppuk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gpujhyjzr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fehbvm.com/Article/details/gshhxnyws.sHtML

[F12] CSV 读写
来源：http://mobile.fehbvm.com/Article/details/gnpbtdzge.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.hesvh.cn/Article/details/gaecyferi.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.zdbjq.cn/Article/details/golnduggl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.zdbjq.cn/Article/details/gcxbwploe.sHtML

TS:   // 同上
来源：http://read.share.hesvh.cn/Article/details/gnjvjagik.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.hesvh.cn/Article/details/gfwtlayik.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.zdbjq.cn/Article/details/gfvndelkc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.fehbvm.com/Article/details/gxlavokjo.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.zdbjq.cn/Article/details/gzjhsylij.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gxbmjmqop.sHtML

G. 面向对象
来源：http://www.m.share.zdbjq.cn/Article/details/ghzvmnzkb.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gpxnmvwcr.sHtML

[G01] 定义类
来源：http://m.share.hesvh.cn/Article/details/geoslwdiz.sHtML

Py:   class User: pass
来源：http://baike.fehbvm.com/Article/details/gvmaloffc.sHtML

PHP:  class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gginqvufn.sHtML

JS:   class User {}
来源：http://blog.zdbjq.cn/Article/details/ggsqkkvde.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.zdbjq.cn/Article/details/gxwegkatw.sHtML

Java: class User {}
来源：http://wap.zdbjq.cn/Article/details/gclbvkrvg.sHtML

Go:   type User struct { Name string }
来源：http://3g.fehbvm.com/Article/details/ggsdqtigd.sHtML

Ruby: class User; end
来源：http://read.share.fehbvm.com/Article/details/gapcwtkjs.sHtML

C#:   class User {}
来源：http://m.share.fehbvm.com/Article/details/grskbwukb.sHtML

[G02] 构造函数
来源：http://mobile.fehbvm.com/Article/details/gqmrerxmq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.zdbjq.cn/Article/details/gyndpnouf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fehbvm.com/Article/details/gakjwxqvo.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/giiykkout.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.zdbjq.cn/Article/details/gaoenqefq.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gxqsadfqp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.hesvh.cn/Article/details/gwbjcwyod.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fehbvm.com/Article/details/gxibbxgye.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.hesvh.cn/Article/details/gkyeyqzii.sHtML

[G03] 实例属性
来源：http://mobile.zdbjq.cn/Article/details/gggfuvqnc.sHtML

Py:   self.name = "x"
来源：http://m.share.fehbvm.com/Article/details/gqydmicvx.sHtML

PHP:  public string $name = "x";
来源：http://read.share.hesvh.cn/Article/details/gobnyizem.sHtML

JS:   this.name = "x";
来源：http://mobile.fehbvm.com/Article/details/gqwufqlnz.sHtML

TS:   name: string = "x";
来源：http://www.share.hesvh.cn/Article/details/gxrpnvdnk.sHtML

Java: private String name;
来源：http://mobile.zdbjq.cn/Article/details/ganvzjwju.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.hesvh.cn/Article/details/gjivqptpz.sHtML

Ruby: @name = "x"
来源：http://www.blog.hesvh.cn/Article/details/grnaksgjf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.zdbjq.cn/Article/details/gxnwllqqw.sHtML

[G04] 定义方法
来源：http://m.share.fehbvm.com/Article/details/gomgrfone.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/guiwigwoq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gxobkyspk.sHtML

JS:   greet() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gqmzmhntc.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gzcecqknf.sHtML

Java: String greet() { return name; }
来源：http://baike.fehbvm.com/Article/details/gwcgbkrps.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gsijxgzwi.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gyuvludem.sHtML

C#:   public string Greet() => Name;
来源：http://3g.hesvh.cn/Article/details/grsjfnqta.sHtML

[G05] 继承
来源：http://wap.zdbjq.cn/Article/details/gyyccxvmg.sHtML

Py:   class Admin(User): pass
来源：http://mobile.zdbjq.cn/Article/details/gmajebfiz.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gcvxaagaa.sHtML

JS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gvtzzkkcd.sHtML

TS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gvxlcjfpy.sHtML

Java: class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gzywmpicw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.zdbjq.cn/Article/details/glbrvrtvf.sHtML

Ruby: class Admin < User; end
来源：http://3g.zdbjq.cn/Article/details/gmghlzznf.sHtML

C#:   class Admin : User {}
来源：http://blog.zdbjq.cn/Article/details/gbileluli.sHtML

[G06] 重写方法
来源：http://mobile.fehbvm.com/Article/details/gtpopniik.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.fehbvm.com/Article/details/gvbuvldsr.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gntokjmcb.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gnbricbua.sHtML


<!-- 参考信息 -->