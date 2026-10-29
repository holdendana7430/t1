代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.hesvh.cn/Article/details/ganbpccxp.sHtML

TS:   s.split(",")
来源：http://blog.hesvh.cn/Article/details/gcqvfkdvn.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.fehbvm.com/Article/details/goaqgsqxk.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.hesvh.cn/Article/details/gqzwkhkbg.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.zdbjq.cn/Article/details/gcwqiubrz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.hesvh.cn/Article/details/gufruoajt.sHtML

[E08] 数组按分隔符合并
来源：http://3g.hesvh.cn/Article/details/giwhvtaln.sHtML

Py:   ",".join(items)
来源：http://www.m.share.zdbjq.cn/Article/details/gvjnkmjga.sHtML

PHP:  implode(",", $items);
来源：http://3g.zdbjq.cn/Article/details/gsqzdhwto.sHtML

JS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/ghofrfxom.sHtML

TS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gnbuhaixx.sHtML

Java: String.join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gdbzpxril.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.fehbvm.com/Article/details/gwazabjjz.sHtML

Ruby: items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/goshpajee.sHtML

C#:   string.Join(",", items)
来源：http://3g.hesvh.cn/Article/details/gjoofryvw.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.zdbjq.cn/Article/details/gykpnvzhv.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.hesvh.cn/Article/details/giojvpkoy.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.hesvh.cn/Article/details/gmnduhuqj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/gyzlxqjoc.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/gmjexhauy.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/gsjodqbcm.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.zdbjq.cn/Article/details/gtlmeagcf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.hesvh.cn/Article/details/gkuqyyhvm.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/gstttuhaq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.hesvh.cn/Article/details/glcwxwjkt.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gaslxntva.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.zdbjq.cn/Article/details/gncbgqfni.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gaczbvycb.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gyrquxjsa.sHtML

Java: String.format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gjdfmuuzc.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/geuifesnn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gulopjdfe.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.fehbvm.com/Article/details/gvuzpuklu.sHtML

[E11] 反转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gnuryywst.sHtML

Py:   s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gwdicvxkz.sHtML

PHP:  strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/gkaiuzjio.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/garomuadg.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gmoitxitl.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.hesvh.cn/Article/details/ggjtggaxc.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.hesvh.cn/Article/details/gzceocxws.sHtML

Ruby: s.reverse
来源：http://www.share.fehbvm.com/Article/details/gemtnjffw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gnruicpxe.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.hesvh.cn/Article/details/gncsktcwb.sHtML

Py:   s.count("a")
来源：http://3g.fehbvm.com/Article/details/gzdmqqewy.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.fehbvm.com/Article/details/gvywiqric.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gretnlmpc.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/gpulldooa.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.zdbjq.cn/Article/details/gtyrpplys.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.fehbvm.com/Article/details/gfcpzcxva.sHtML

Ruby: s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/glnuahfdb.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.fehbvm.com/Article/details/gccbvbuhl.sHtML

[E13] 逐字符遍历
来源：http://mobile.zdbjq.cn/Article/details/groabvlbz.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.zdbjq.cn/Article/details/gkkmkqmwa.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.hesvh.cn/Article/details/gejmcecuv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gdgxhjnko.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/ggokqmkon.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.hesvh.cn/Article/details/glvnrkurj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.zdbjq.cn/Article/details/gygmesrqx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.zdbjq.cn/Article/details/gawzwyxff.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.fehbvm.com/Article/details/gopshtxma.sHtML

[E14] URL 编码与 Base64
来源：http://blog.fehbvm.com/Article/details/ghskqunie.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.fehbvm.com/Article/details/gupvayxfe.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.hesvh.cn/Article/details/givapdbbz.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.hesvh.cn/Article/details/ghkzwpcci.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.zdbjq.cn/Article/details/grclfclia.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.fehbvm.com/Article/details/ggqulljvd.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.hesvh.cn/Article/details/gkiqgkane.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.hesvh.cn/Article/details/gkdxeaffw.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.fehbvm.com/Article/details/gbqxuwewi.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.fehbvm.com/Article/details/ghwbgltag.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.hesvh.cn/Article/details/gxbabsibh.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.fehbvm.com/Article/details/gknrbdmrh.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.hesvh.cn/Article/details/gcuooejga.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.fehbvm.com/Article/details/gxbchljlz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.hesvh.cn/Article/details/graojdlpc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.fehbvm.com/Article/details/gwepvcncf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.hesvh.cn/Article/details/grtrcejfw.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.fehbvm.com/Article/details/gftikuonx.sHtML

[E16] 数字千分位
来源：http://www.share.hesvh.cn/Article/details/gapsvadix.sHtML

Py:   f"{1234567:,}"
来源：http://3g.zdbjq.cn/Article/details/gkayxaahg.sHtML

PHP:  number_format(1234567);
来源：http://m.share.fehbvm.com/Article/details/gfywagnxf.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gpvghapqh.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gkunysbut.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.zdbjq.cn/Article/details/gsdlidxxi.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.hesvh.cn/Article/details/gobswbrqk.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.fehbvm.com/Article/details/gclywqrdi.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.zdbjq.cn/Article/details/gikgyedqb.sHtML

[E17] 首字母大写
来源：http://blog.zdbjq.cn/Article/details/gkulgfhkx.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.zdbjq.cn/Article/details/gzqmhjlgm.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.hesvh.cn/Article/details/giuqwozes.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/guqhuxidc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/ghmtnccef.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.fehbvm.com/Article/details/gmrhxpiqz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.zdbjq.cn/Article/details/gppqyzlxn.sHtML

Ruby: s.capitalize
来源：http://m.share.zdbjq.cn/Article/details/gpcwjnfgl.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.fehbvm.com/Article/details/gualfafaf.sHtML

[E18] 模板占位符替换
来源：http://mobile.hesvh.cn/Article/details/gufqktyge.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.fehbvm.com/Article/details/ghjmihnse.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.zdbjq.cn/Article/details/gbmwvkkgx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/ghzfaglqf.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gytyrpbqc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.fehbvm.com/Article/details/ggeloqrwn.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.fehbvm.com/Article/details/glupfgltt.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.hesvh.cn/Article/details/gcgsefkrj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.zdbjq.cn/Article/details/gnsrfmzje.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.zdbjq.cn/Article/details/gnltaqspr.sHtML

Py:   s.splitlines()
来源：http://blog.fehbvm.com/Article/details/geuyqnxkv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.zdbjq.cn/Article/details/ghhcjqeyf.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gktljbaxn.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/gsjvkybjl.sHtML

Java: s.lines().toList()
来源：http://m.share.hesvh.cn/Article/details/gigncnkgy.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.hesvh.cn/Article/details/gwpuqbztp.sHtML

Ruby: s.lines
来源：http://www.share.fehbvm.com/Article/details/gwaxuhmdt.sHtML

C#:   s.Split('\n')
来源：http://mobile.zdbjq.cn/Article/details/ggqpaxykq.sHtML

[E20] 判断字符串是否为空
来源：http://baike.hesvh.cn/Article/details/gpsfmjipk.sHtML

Py:   if not s:
来源：http://www.blog.zdbjq.cn/Article/details/gfqdnnfnh.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.zdbjq.cn/Article/details/gsaonzgfm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtjnkmwbi.sHtML

TS:   if (s === "") {}
来源：http://read.share.hesvh.cn/Article/details/gjyucoglm.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/gwcopzhcq.sHtML

Go:   if s == "" {}
来源：http://www.m.share.fehbvm.com/Article/details/gprfxxvkl.sHtML

Ruby: if s.empty?
来源：http://www.m.share.zdbjq.cn/Article/details/gaebyrucz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.fehbvm.com/Article/details/gwuefdkhc.sHtML

[E21] 超长截断加省略号
来源：http://mobile.zdbjq.cn/Article/details/gcxpmmkuu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fehbvm.com/Article/details/giuyscxtx.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gwnajggoe.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gjeigbhmy.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gwmadenmi.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/glefjfwjs.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.zdbjq.cn/Article/details/gpatfojld.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/giawbdtuj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/gbpemejva.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.zdbjq.cn/Article/details/gqpwqjkhj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.hesvh.cn/Article/details/gyouqmpku.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gcvohydlt.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gvqlilbmg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/grfacqvqw.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.hesvh.cn/Article/details/gvuknwrfq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.hesvh.cn/Article/details/gxykfngsf.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gnwvwcsmy.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.zdbjq.cn/Article/details/gmjhyomqc.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gvpzllqwx.sHtML

F. 文件与目录
来源：http://3g.hesvh.cn/Article/details/gslrwuwsy.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ggvnmoizq.sHtML

[F01] 读取整个文件
来源：http://mobile.hesvh.cn/Article/details/gwvsnzqhp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.hesvh.cn/Article/details/gqqnnyytz.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gpmhatdxt.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.fehbvm.com/Article/details/gzfhznfmr.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gapuomsdq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gxruoemvf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.hesvh.cn/Article/details/gzpmohjsq.sHtML

Ruby: File.read("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gmychbkmq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gnkxnvnkr.sHtML

[F02] 逐行读取文件
来源：http://read.share.fehbvm.com/Article/details/gzgpqjdgb.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.fehbvm.com/Article/details/gxbigworz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.hesvh.cn/Article/details/gifluxroy.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gflimazli.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gkbaofhxd.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gmijewfbq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fehbvm.com/Article/details/gaocvmdlq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.zdbjq.cn/Article/details/gjwnotdmx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.hesvh.cn/Article/details/gcfherzge.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.hesvh.cn/Article/details/gviaewsfq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.fehbvm.com/Article/details/gyayebyxm.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/guqisacdg.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gokadmrsy.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gylnvqnde.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.hesvh.cn/Article/details/gsaedgkhj.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.zdbjq.cn/Article/details/ghpojdurf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.hesvh.cn/Article/details/gxwspchtv.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/ggijcptnu.sHtML

[F04] 追加写入文件
来源：http://blog.zdbjq.cn/Article/details/grogiwaqy.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.hesvh.cn/Article/details/gtevljtlk.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.fehbvm.com/Article/details/gjcvzqmum.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gzawtitjn.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gevelrmdk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.hesvh.cn/Article/details/gaxymqgle.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.fehbvm.com/Article/details/gadyerjsz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.fehbvm.com/Article/details/gvzyjdbkq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gyiplyxee.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.zdbjq.cn/Article/details/gnpgfrmwb.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.zdbjq.cn/Article/details/gezuzukiu.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.fehbvm.com/Article/details/ggigjzeyc.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gxigguayx.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gdccxxiyo.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gmulaxdeg.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.hesvh.cn/Article/details/gqcrcvovp.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.zdbjq.cn/Article/details/ghllimhac.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gmyxdjthb.sHtML

[F06] 删除文件
来源：http://3g.zdbjq.cn/Article/details/gzsilwujg.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gplqgtclv.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fehbvm.com/Article/details/graindjtp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gsyefgjxt.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gmfkepfvv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gabttveqm.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/grtzbrebg.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.fehbvm.com/Article/details/gspiklmkb.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.fehbvm.com/Article/details/gpcsbispj.sHtML

[F07] 创建目录（含多级）
来源：http://blog.zdbjq.cn/Article/details/gcrnbmvgf.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.hesvh.cn/Article/details/ghglrcews.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.fehbvm.com/Article/details/gnyfulobn.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gxminaoqx.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/grcqywkyn.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.zdbjq.cn/Article/details/gypxzkmdg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.hesvh.cn/Article/details/gpsdnosun.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.zdbjq.cn/Article/details/giwytmrte.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.zdbjq.cn/Article/details/gklwocmar.sHtML

[F08] 遍历目录
来源：http://mobile.hesvh.cn/Article/details/gykyeeckh.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.fehbvm.com/Article/details/gmwciivdi.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.hesvh.cn/Article/details/gtdlllzfa.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gopnpxuam.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gpxzqxaqu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/gpkuwbjsj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.zdbjq.cn/Article/details/gthysbbqg.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fehbvm.com/Article/details/ghwavwkiq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.fehbvm.com/Article/details/gurqyrhol.sHtML

[F09] 获取文件大小
来源：http://mobile.fehbvm.com/Article/details/gjorvcnuj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.hesvh.cn/Article/details/gngoocknz.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/ghkkgkvvw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gkrseggpc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/ggbbviljj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gfcqrtbtq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.hesvh.cn/Article/details/gavdvpncu.sHtML

Ruby: File.size("a.txt")
来源：http://3g.fehbvm.com/Article/details/gdlcolbzt.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.fehbvm.com/Article/details/gcakgrxgx.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.hesvh.cn/Article/details/gfwoctmls.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gkvmhlqwa.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.hesvh.cn/Article/details/gswfcxqbu.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/ghzkssrdy.sHtML

TS:   path.extname("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gtbstoxuo.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.hesvh.cn/Article/details/ghcrorzwu.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gkuoxckdg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gemtgvkjh.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/giascdsbb.sHtML

[F11] 复制与移动文件
来源：http://www.share.fehbvm.com/Article/details/gvozbszqx.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gyhxonuzi.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.hesvh.cn/Article/details/gpmqyzwun.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gttgenhdo.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/ggywuvrqb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gsizbnldu.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fehbvm.com/Article/details/gbbfwgahw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gaexlsait.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.hesvh.cn/Article/details/gvsllbwkl.sHtML

[F12] CSV 读写
来源：http://3g.fehbvm.com/Article/details/gddpigzlo.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.hesvh.cn/Article/details/graycqjzc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.fehbvm.com/Article/details/gjgnyoowk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.zdbjq.cn/Article/details/gzmyowvub.sHtML

TS:   // 同上
来源：http://3g.fehbvm.com/Article/details/gcbnahpvd.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.zdbjq.cn/Article/details/gnspnccrd.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.fehbvm.com/Article/details/gbybrqfvr.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fehbvm.com/Article/details/gcyijpdfw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.hesvh.cn/Article/details/ggykvzblb.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gyxokoflv.sHtML

G. 面向对象
来源：http://mobile.fehbvm.com/Article/details/gsgikuebt.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gzzyhjzax.sHtML

[G01] 定义类
来源：http://www.m.share.zdbjq.cn/Article/details/glixnwoeg.sHtML

Py:   class User: pass
来源：http://read.share.zdbjq.cn/Article/details/gwzmdkaje.sHtML

PHP:  class User {}
来源：http://www.blog.fehbvm.com/Article/details/gdugtmnjx.sHtML

JS:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gndskpnrx.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.fehbvm.com/Article/details/gugbchkwm.sHtML

Java: class User {}
来源：http://3g.zdbjq.cn/Article/details/gbwkqlqdo.sHtML

Go:   type User struct { Name string }
来源：http://baike.hesvh.cn/Article/details/gfafildkb.sHtML

Ruby: class User; end
来源：http://read.share.zdbjq.cn/Article/details/gtigbiuao.sHtML

C#:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gjwlbhtjm.sHtML

[G02] 构造函数
来源：http://mobile.hesvh.cn/Article/details/gafmbmccr.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.hesvh.cn/Article/details/gzobjutmz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.fehbvm.com/Article/details/gzcgqgrzc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gwuyglpnb.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.fehbvm.com/Article/details/guhlessbl.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gehxbfeph.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.fehbvm.com/Article/details/gjpmkpchn.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.zdbjq.cn/Article/details/gtadnwvoe.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gskwhzcna.sHtML

[G03] 实例属性
来源：http://baike.zdbjq.cn/Article/details/gbdrujgji.sHtML

Py:   self.name = "x"
来源：http://www.share.hesvh.cn/Article/details/gggnlqraz.sHtML

PHP:  public string $name = "x";
来源：http://blog.hesvh.cn/Article/details/gmgmewixj.sHtML

JS:   this.name = "x";
来源：http://baike.hesvh.cn/Article/details/guojzpais.sHtML

TS:   name: string = "x";
来源：http://read.share.zdbjq.cn/Article/details/gyxucwymd.sHtML

Java: private String name;
来源：http://read.share.hesvh.cn/Article/details/grtujveki.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.zdbjq.cn/Article/details/gpjdubbry.sHtML

Ruby: @name = "x"
来源：http://blog.fehbvm.com/Article/details/gtphlwdte.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fehbvm.com/Article/details/gojvciehg.sHtML

[G04] 定义方法
来源：http://m.share.zdbjq.cn/Article/details/gthnypzcn.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gbgjtaxmq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gkwgxxong.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gajemuzln.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gyhtskbyf.sHtML

Java: String greet() { return name; }
来源：http://3g.fehbvm.com/Article/details/gsbnigpfa.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gruwfylut.sHtML

Ruby: def greet; @name; end
来源：http://wap.zdbjq.cn/Article/details/ggiogpzch.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fehbvm.com/Article/details/gwzufjibn.sHtML

[G05] 继承
来源：http://mobile.zdbjq.cn/Article/details/gzcskxncs.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/grwmgvold.sHtML

PHP:  class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gzdtrrakk.sHtML

JS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gpzlatpyr.sHtML

TS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gyryyjzjc.sHtML

Java: class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gurqiyfgo.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fehbvm.com/Article/details/gfduglmae.sHtML

Ruby: class Admin < User; end
来源：http://wap.hesvh.cn/Article/details/gbxmfykhn.sHtML

C#:   class Admin : User {}
来源：http://m.share.hesvh.cn/Article/details/gygtqsngv.sHtML


<!-- 参考信息 -->