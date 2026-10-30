代发 wailian999

Ruby: s.split(",");  s.split
来源：http://www.m.share.zdbjq.cn/Article/details/gsocqhgjf.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.fehbvm.com/Article/details/gfutktzuz.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.hesvh.cn/Article/details/gjxzknvqh.sHtML

Py:   ",".join(items)
来源：http://wap.hesvh.cn/Article/details/gnpnhiqhq.sHtML

PHP:  implode(",", $items);
来源：http://mobile.fehbvm.com/Article/details/gvfpgrcha.sHtML

JS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/grxfyoalj.sHtML

TS:   items.join(",")
来源：http://wap.zdbjq.cn/Article/details/ghdpoqdua.sHtML

Java: String.join(",", items)
来源：http://baike.hesvh.cn/Article/details/gufucjugm.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.hesvh.cn/Article/details/gmcoaaana.sHtML

Ruby: items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gkpifpurn.sHtML

C#:   string.Join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gaiwlephi.sHtML

[E09] 去除所有空白字符
来源：http://3g.zdbjq.cn/Article/details/gcxsprenk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.zdbjq.cn/Article/details/gxulsnlsv.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.zdbjq.cn/Article/details/gxdnmvhlt.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/glhtnvcne.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gibyppkyv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.zdbjq.cn/Article/details/gaylmylky.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.zdbjq.cn/Article/details/gqebfceak.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.fehbvm.com/Article/details/gqoclymlb.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gosqlmjpb.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.fehbvm.com/Article/details/gbypduzto.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.zdbjq.cn/Article/details/guhyaavec.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.fehbvm.com/Article/details/gyxobswtm.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gcuswrjdf.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/guzlgokwx.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gvldbsrfp.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gttnybuxp.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gjpvbibag.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.hesvh.cn/Article/details/ggdqudzuv.sHtML

[E11] 反转字符串
来源：http://3g.hesvh.cn/Article/details/grqfzvlta.sHtML

Py:   s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/gesrmnwgy.sHtML

PHP:  strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/glwbnttll.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gkusmexzd.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gntcppmyl.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gkvxhylnd.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gbdrzhukc.sHtML

Ruby: s.reverse
来源：http://mobile.zdbjq.cn/Article/details/glgcusfwo.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/glqsskcma.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gzxjpkagr.sHtML

Py:   s.count("a")
来源：http://m.share.fehbvm.com/Article/details/ghsmahqee.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.fehbvm.com/Article/details/gfqgbhant.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gdpyzpcje.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/ggvfsaguj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.zdbjq.cn/Article/details/graggkefn.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.hesvh.cn/Article/details/gxvcfapgz.sHtML

Ruby: s.count("a")
来源：http://wap.fehbvm.com/Article/details/gjwmrvoiz.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.fehbvm.com/Article/details/gkrilyiay.sHtML

[E13] 逐字符遍历
来源：http://www.share.fehbvm.com/Article/details/ghpzlhrtq.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.fehbvm.com/Article/details/gordwmetk.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.hesvh.cn/Article/details/geecvqzkx.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gpmjdmivf.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/ghhvmfdea.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.zdbjq.cn/Article/details/gsufwouas.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.zdbjq.cn/Article/details/gymcdpyko.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.fehbvm.com/Article/details/gtarzqtbo.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/ghnkljdgu.sHtML

[E14] URL 编码与 Base64
来源：http://wap.zdbjq.cn/Article/details/gfrooaepg.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.zdbjq.cn/Article/details/gxrlpsfpb.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.zdbjq.cn/Article/details/gbszyhpzr.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.zdbjq.cn/Article/details/gldjbuglu.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.zdbjq.cn/Article/details/gtoaixlae.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.hesvh.cn/Article/details/gfpcrvdcr.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.zdbjq.cn/Article/details/gsdbjmzxd.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.zdbjq.cn/Article/details/glgdjxfde.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.zdbjq.cn/Article/details/grmdlnqjq.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.fehbvm.com/Article/details/gquidiibj.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.zdbjq.cn/Article/details/gghkolptq.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.fehbvm.com/Article/details/groifdcmd.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.fehbvm.com/Article/details/gygwqtuhx.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.zdbjq.cn/Article/details/gdfbfxwgy.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.hesvh.cn/Article/details/gyajqvtkp.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.hesvh.cn/Article/details/grxvhnsyz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.fehbvm.com/Article/details/gtimnwwig.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.fehbvm.com/Article/details/gctnblgiw.sHtML

[E16] 数字千分位
来源：http://mobile.zdbjq.cn/Article/details/gilenijas.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.fehbvm.com/Article/details/gnzsnbeln.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fehbvm.com/Article/details/ghtvgjmkf.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/gkkcmfxhg.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/gbfqvsdky.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.hesvh.cn/Article/details/gbrpnbhzy.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.zdbjq.cn/Article/details/gzwehzyxk.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.hesvh.cn/Article/details/gwnaozeix.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.zdbjq.cn/Article/details/gcfetlpfk.sHtML

[E17] 首字母大写
来源：http://mobile.zdbjq.cn/Article/details/gxazkbkwf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.zdbjq.cn/Article/details/gwyzvkbmn.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.zdbjq.cn/Article/details/gsdyygpzq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gqijghcyt.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gnnlrlaay.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.zdbjq.cn/Article/details/ggltfteox.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/ghrtycema.sHtML

Ruby: s.capitalize
来源：http://baike.hesvh.cn/Article/details/gqwesolhy.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.zdbjq.cn/Article/details/gttzyfoej.sHtML

[E18] 模板占位符替换
来源：http://m.share.fehbvm.com/Article/details/geuikgkdc.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.zdbjq.cn/Article/details/gdpannunt.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.hesvh.cn/Article/details/gszdiiewa.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gamipzniv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/giaujsutt.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gjfsgblqe.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gcotcswbp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.zdbjq.cn/Article/details/gmarfspem.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.hesvh.cn/Article/details/gqnflevae.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gxfnqzckr.sHtML

Py:   s.splitlines()
来源：http://www.blog.fehbvm.com/Article/details/gcasauslg.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.fehbvm.com/Article/details/gpyaekyuv.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/gnzxesdci.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gboqtepgy.sHtML

Java: s.lines().toList()
来源：http://www.blog.zdbjq.cn/Article/details/ggfhphryp.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.hesvh.cn/Article/details/gajkbqyky.sHtML

Ruby: s.lines
来源：http://m.share.zdbjq.cn/Article/details/gcpdyrfkn.sHtML

C#:   s.Split('\n')
来源：http://m.share.fehbvm.com/Article/details/gmujtkuur.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.zdbjq.cn/Article/details/ggfaqdmde.sHtML

Py:   if not s:
来源：http://blog.hesvh.cn/Article/details/gjlqzjikk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fehbvm.com/Article/details/gegbxvtxz.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.fehbvm.com/Article/details/gshtogwbb.sHtML

TS:   if (s === "") {}
来源：http://wap.zdbjq.cn/Article/details/goxpgryuu.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gkkbcsmcu.sHtML

Go:   if s == "" {}
来源：http://read.share.hesvh.cn/Article/details/gjjohptsf.sHtML

Ruby: if s.empty?
来源：http://www.blog.fehbvm.com/Article/details/gjvvotzxt.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmctxuxma.sHtML

[E21] 超长截断加省略号
来源：http://mobile.fehbvm.com/Article/details/gzjkkvbog.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.hesvh.cn/Article/details/gfkollkki.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/ggerzxggm.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gobwhzybx.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gpaxtkhaf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gefbfohmx.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.zdbjq.cn/Article/details/gfyzmjvaf.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gprkxldbg.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gfywjfxig.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.zdbjq.cn/Article/details/ggitzlxcj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.hesvh.cn/Article/details/gljkidsbl.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gbijtrmhq.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gvhmaqneg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gcvltqhbf.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.hesvh.cn/Article/details/gjlpbamwh.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.fehbvm.com/Article/details/gblkhorbp.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.hesvh.cn/Article/details/guuaxouxa.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.zdbjq.cn/Article/details/gwtdrfffu.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gsmckfbxs.sHtML

F. 文件与目录
来源：http://m.share.zdbjq.cn/Article/details/gywrnmsbg.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/giavqavwo.sHtML

[F01] 读取整个文件
来源：http://mobile.fehbvm.com/Article/details/gpumusfbe.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.fehbvm.com/Article/details/gnotyqtox.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gjfcxhnva.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.zdbjq.cn/Article/details/glpnttsgi.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gjlrihnbm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gvasmnlon.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.zdbjq.cn/Article/details/geslnrgvp.sHtML

Ruby: File.read("a.txt")
来源：http://wap.zdbjq.cn/Article/details/ggijogjig.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gbxdfzylu.sHtML

[F02] 逐行读取文件
来源：http://www.share.hesvh.cn/Article/details/gkzwxetmr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.zdbjq.cn/Article/details/glxqyjxnw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.fehbvm.com/Article/details/gbacpewzc.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/gelzncmxf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/gxuswzwxd.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gforuxrob.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.fehbvm.com/Article/details/gcwodhgln.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.zdbjq.cn/Article/details/grdwuiukn.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.fehbvm.com/Article/details/glhtsjupz.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.hesvh.cn/Article/details/gicihvpqg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.zdbjq.cn/Article/details/gumygefyq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/grmolivvc.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gpymfgqra.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/gnxueymjq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.hesvh.cn/Article/details/gdhvzfnvo.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.hesvh.cn/Article/details/gijnddeql.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.hesvh.cn/Article/details/gsygttbcn.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gyvrgpjda.sHtML

[F04] 追加写入文件
来源：http://read.share.fehbvm.com/Article/details/gajxccgxl.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fehbvm.com/Article/details/giynefkpn.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fehbvm.com/Article/details/gejolovji.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/gpvdfsqrz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/gqnrdekks.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.zdbjq.cn/Article/details/guimkgtkj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.hesvh.cn/Article/details/gumpgeubw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.fehbvm.com/Article/details/gcvjpgdkv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.fehbvm.com/Article/details/gqcavxeca.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.zdbjq.cn/Article/details/gkrgqxnwh.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.hesvh.cn/Article/details/giuqsbacs.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gcbmlrskk.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gkkkjmeun.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/grckyhfbn.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gnwlrivqo.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.hesvh.cn/Article/details/gqamtjkku.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fehbvm.com/Article/details/guqkdcohg.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gjxntcuxi.sHtML

[F06] 删除文件
来源：http://www.blog.fehbvm.com/Article/details/giozrfgyz.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gmqvzvdpj.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fehbvm.com/Article/details/gbamkdhtc.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/greayozlo.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gyehxysom.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gzccfjnpw.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gulystdvq.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gvjxaqyqa.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gqnjugebz.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.fehbvm.com/Article/details/ggkjkwisb.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/gvmxpvsjb.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.zdbjq.cn/Article/details/gayqifuhd.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/guhhlfxno.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/gkrdvcqfk.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.fehbvm.com/Article/details/gaggdjgqm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.zdbjq.cn/Article/details/gwprjuhsv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.hesvh.cn/Article/details/gvcfhccyi.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.fehbvm.com/Article/details/gwjwlqzog.sHtML

[F08] 遍历目录
来源：http://wap.zdbjq.cn/Article/details/glxllhccj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.fehbvm.com/Article/details/gkshechpa.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.zdbjq.cn/Article/details/gqftiatij.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/gjiafpusm.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gdlwyzthh.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gohxioqia.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.zdbjq.cn/Article/details/gbiwdzrxe.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.fehbvm.com/Article/details/gqxybhopq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.hesvh.cn/Article/details/gjdcfwrpr.sHtML

[F09] 获取文件大小
来源：http://3g.zdbjq.cn/Article/details/gwlliayei.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.hesvh.cn/Article/details/gckisvugn.sHtML

PHP:  filesize("a.txt");
来源：http://wap.fehbvm.com/Article/details/grrnngyev.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gtnibytmy.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/gaajbgbfm.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gsmahchgd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.hesvh.cn/Article/details/gxzkgrcur.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gjgjmrpuq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.zdbjq.cn/Article/details/gyqkybjpx.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.hesvh.cn/Article/details/gtqfzkafc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/grqdbkfjq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.hesvh.cn/Article/details/ghcjvadtj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gojfmduyu.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gisltmrah.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.fehbvm.com/Article/details/gednrdlhi.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gldufyomk.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/ghhwdondk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gffkblnvm.sHtML

[F11] 复制与移动文件
来源：http://read.share.hesvh.cn/Article/details/gprumbpez.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/glofwxodi.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.hesvh.cn/Article/details/gvqsnazme.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gdjmxxnzj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gfwnqtnnq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.fehbvm.com/Article/details/gkttzlmcc.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.zdbjq.cn/Article/details/guicvzjay.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/ghimauupm.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.hesvh.cn/Article/details/ggapjfchl.sHtML

[F12] CSV 读写
来源：http://www.share.hesvh.cn/Article/details/gkqastnom.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.hesvh.cn/Article/details/gupzobjhr.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.zdbjq.cn/Article/details/gazahdtrv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.zdbjq.cn/Article/details/gcohfjpry.sHtML

TS:   // 同上
来源：http://www.share.zdbjq.cn/Article/details/gphgcjvjm.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.hesvh.cn/Article/details/gvirxwqlf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.fehbvm.com/Article/details/gxvrdhbuh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.hesvh.cn/Article/details/gvdxghzyh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.fehbvm.com/Article/details/gwvmveflc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwyoulmpo.sHtML

G. 面向对象
来源：http://read.share.hesvh.cn/Article/details/glsaoziwh.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvztcmdsl.sHtML

[G01] 定义类
来源：http://www.share.zdbjq.cn/Article/details/gukclrgvs.sHtML

Py:   class User: pass
来源：http://blog.zdbjq.cn/Article/details/gmpynjoug.sHtML

PHP:  class User {}
来源：http://read.share.fehbvm.com/Article/details/gbmuzmpun.sHtML

JS:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gcwxifzjg.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.fehbvm.com/Article/details/gkurqokrs.sHtML

Java: class User {}
来源：http://3g.zdbjq.cn/Article/details/gtgxjfxbn.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.zdbjq.cn/Article/details/gulubjxfw.sHtML

Ruby: class User; end
来源：http://www.share.hesvh.cn/Article/details/gzutvkora.sHtML

C#:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/gfjaucfcy.sHtML

[G02] 构造函数
来源：http://baike.hesvh.cn/Article/details/givkhoqyq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.hesvh.cn/Article/details/gcauuzkja.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.zdbjq.cn/Article/details/gklejjyzv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gyqpbraqv.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/gtwxizzht.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gdlobpngf.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.hesvh.cn/Article/details/guiyxbjjx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.hesvh.cn/Article/details/geyrddwxz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.hesvh.cn/Article/details/gfbctboty.sHtML

[G03] 实例属性
来源：http://baike.zdbjq.cn/Article/details/gtlegexrl.sHtML

Py:   self.name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gvnmntxwl.sHtML

PHP:  public string $name = "x";
来源：http://m.share.hesvh.cn/Article/details/gumlphtkh.sHtML

JS:   this.name = "x";
来源：http://baike.hesvh.cn/Article/details/glawnbjnn.sHtML

TS:   name: string = "x";
来源：http://blog.zdbjq.cn/Article/details/gaauihzgd.sHtML

Java: private String name;
来源：http://baike.fehbvm.com/Article/details/gjakqhzde.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.zdbjq.cn/Article/details/gxcxiqlxd.sHtML

Ruby: @name = "x"
来源：http://read.share.hesvh.cn/Article/details/gltdxjecb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.hesvh.cn/Article/details/gtvtoogpp.sHtML

[G04] 定义方法
来源：http://www.blog.fehbvm.com/Article/details/gllsnkwvp.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gwqhafdcm.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gezxoagob.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gszeinmkh.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gsnonbsho.sHtML

Java: String greet() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gbsmxcmxc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gnrufseui.sHtML

Ruby: def greet; @name; end
来源：http://3g.fehbvm.com/Article/details/gxnsnnhef.sHtML

C#:   public string Greet() => Name;
来源：http://baike.hesvh.cn/Article/details/gtfagnhrn.sHtML

[G05] 继承
来源：http://www.m.share.fehbvm.com/Article/details/gehbkslce.sHtML

Py:   class Admin(User): pass
来源：http://blog.zdbjq.cn/Article/details/gelpuozdj.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gkfbgtxub.sHtML

JS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gzemkqwrz.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gewhslxfh.sHtML

Java: class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gbafroacu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.zdbjq.cn/Article/details/gszarmqgv.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fehbvm.com/Article/details/gibbvpgpe.sHtML

C#:   class Admin : User {}
来源：http://wap.hesvh.cn/Article/details/gtwcaltvs.sHtML

[G06] 重写方法
来源：http://wap.fehbvm.com/Article/details/guhosdffe.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.fehbvm.com/Article/details/gtoctjcnv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gwsxmpuwz.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnghwkxas.sHtML


<!-- 参考信息 -->