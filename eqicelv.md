代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.zdbjq.cn/Article/details/gfufmmvpz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.hesvh.cn/Article/details/glcruoksy.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/giddqxxfn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/gtgbetrse.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.zdbjq.cn/Article/details/gwgpjnlfx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.hesvh.cn/Article/details/gumdibila.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.zdbjq.cn/Article/details/gxnsalioy.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.hesvh.cn/Article/details/ghrjkizrw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.hesvh.cn/Article/details/gitxrkxww.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/ggikpckwb.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.fehbvm.com/Article/details/gefkfqnhr.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gnlyqatsk.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gvfuynqyj.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gtllwwvrx.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gylzjlwwo.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gpxrwhgiq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.hesvh.cn/Article/details/gtdoumdjz.sHtML

[E11] 反转字符串
来源：http://wap.fehbvm.com/Article/details/gkjveeitx.sHtML

Py:   s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gbzyuavmx.sHtML

PHP:  strrev($s);
来源：http://m.share.hesvh.cn/Article/details/gtlaaxist.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gorelmvju.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gwkhoqkgw.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.fehbvm.com/Article/details/gqxlyjdqv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.zdbjq.cn/Article/details/gotvsbned.sHtML

Ruby: s.reverse
来源：http://mobile.hesvh.cn/Article/details/gcrkipvra.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gpgmjhipg.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.zdbjq.cn/Article/details/gtnekjdcg.sHtML

Py:   s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gywbczfom.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.hesvh.cn/Article/details/gbmuzzykz.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/gddsiitod.sHtML

TS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gisimddmf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.hesvh.cn/Article/details/gifbfaxqm.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.fehbvm.com/Article/details/gtwidlztk.sHtML

Ruby: s.count("a")
来源：http://blog.fehbvm.com/Article/details/gukhmjtpq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.fehbvm.com/Article/details/gembspzir.sHtML

[E13] 逐字符遍历
来源：http://baike.hesvh.cn/Article/details/gcrsomheu.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.hesvh.cn/Article/details/gfapzjnaa.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.zdbjq.cn/Article/details/gpdzoizae.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/guquuwgov.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gncqayqdp.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.hesvh.cn/Article/details/gxuglcznl.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.zdbjq.cn/Article/details/gnolirnpx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.hesvh.cn/Article/details/gmluttipt.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.hesvh.cn/Article/details/gswokywgh.sHtML

[E14] URL 编码与 Base64
来源：http://blog.zdbjq.cn/Article/details/gvdwvfggf.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.hesvh.cn/Article/details/gigwanvjc.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.hesvh.cn/Article/details/gxmdpgulo.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.zdbjq.cn/Article/details/gankzblck.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.hesvh.cn/Article/details/gogfecvyx.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.fehbvm.com/Article/details/gkhuynfnl.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.zdbjq.cn/Article/details/gshiltple.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.fehbvm.com/Article/details/gygzhswzc.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gfyhluzca.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.fehbvm.com/Article/details/gsphmqolx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.fehbvm.com/Article/details/gthbqlwjv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.hesvh.cn/Article/details/gpvetrpmh.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.hesvh.cn/Article/details/gjiygqupp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.hesvh.cn/Article/details/gxkoefvhk.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.fehbvm.com/Article/details/gwwchmiqm.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.fehbvm.com/Article/details/gsyaolavi.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.fehbvm.com/Article/details/gcjfhijbl.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.fehbvm.com/Article/details/ghqbljoqf.sHtML

[E16] 数字千分位
来源：http://mobile.hesvh.cn/Article/details/gapsmhfry.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.fehbvm.com/Article/details/gaasgckgk.sHtML

PHP:  number_format(1234567);
来源：http://m.share.fehbvm.com/Article/details/gercdjarv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gjxozyueq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/gptuegpyp.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.fehbvm.com/Article/details/gnulxblnf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fehbvm.com/Article/details/gaiouhqyg.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.fehbvm.com/Article/details/gzhdcqffc.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.zdbjq.cn/Article/details/gdibhroxu.sHtML

[E17] 首字母大写
来源：http://blog.hesvh.cn/Article/details/gqcfflmzu.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.fehbvm.com/Article/details/gyxojmens.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.zdbjq.cn/Article/details/gsoziixmg.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/glqsivvpj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gzkxsaslf.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.zdbjq.cn/Article/details/ggcyjetka.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.zdbjq.cn/Article/details/gzypuhitq.sHtML

Ruby: s.capitalize
来源：http://wap.hesvh.cn/Article/details/gvjvzxbei.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.fehbvm.com/Article/details/gwkwwkvvg.sHtML

[E18] 模板占位符替换
来源：http://baike.fehbvm.com/Article/details/gfzdldbtl.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.zdbjq.cn/Article/details/gpdzmqhoy.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.zdbjq.cn/Article/details/gkmfjakqs.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gtpdohsgb.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gkfuydfzh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gsicafrdp.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/ghnngbqkx.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.fehbvm.com/Article/details/gbirorizg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.fehbvm.com/Article/details/guhwujdac.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.hesvh.cn/Article/details/gatcxwnuo.sHtML

Py:   s.splitlines()
来源：http://baike.fehbvm.com/Article/details/gjsdygqxw.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.hesvh.cn/Article/details/ghxmmnhyy.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/gkezprzht.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/gafsufefj.sHtML

Java: s.lines().toList()
来源：http://www.share.fehbvm.com/Article/details/gromsspur.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fehbvm.com/Article/details/giqpwxric.sHtML

Ruby: s.lines
来源：http://baike.fehbvm.com/Article/details/gtudjjfum.sHtML

C#:   s.Split('\n')
来源：http://wap.hesvh.cn/Article/details/gbcmexkjt.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fehbvm.com/Article/details/gummbohkv.sHtML

Py:   if not s:
来源：http://3g.zdbjq.cn/Article/details/gnkvzqwrh.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.zdbjq.cn/Article/details/gdajidzjj.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.zdbjq.cn/Article/details/gponkmiyr.sHtML

TS:   if (s === "") {}
来源：http://3g.fehbvm.com/Article/details/genkwncyq.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gosgpwyov.sHtML

Go:   if s == "" {}
来源：http://wap.hesvh.cn/Article/details/gnsgmrsfo.sHtML

Ruby: if s.empty?
来源：http://m.share.fehbvm.com/Article/details/gszejmrib.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.zdbjq.cn/Article/details/gqilxjqws.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fehbvm.com/Article/details/ggnovissk.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.zdbjq.cn/Article/details/gbecqkbwf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gdjdpuxju.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gmzilkabb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gcazbyuog.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gkiicybxf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.hesvh.cn/Article/details/gwmeauymo.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gomjltjai.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gslpmhese.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.zdbjq.cn/Article/details/gqoouavfz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.fehbvm.com/Article/details/gwsvidzij.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/ggdwjtorn.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/gfxmubynx.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/gpcmlgxux.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gylxmxsvn.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.fehbvm.com/Article/details/gougbfdgj.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gvyhoyqwv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.zdbjq.cn/Article/details/gboraohkb.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gjxexhrzm.sHtML

F. 文件与目录
来源：http://mobile.fehbvm.com/Article/details/gaesoydwy.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ghopmskpc.sHtML

[F01] 读取整个文件
来源：http://www.share.hesvh.cn/Article/details/galzlwbua.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.zdbjq.cn/Article/details/gohxqpoxa.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gcmgmxkfl.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.zdbjq.cn/Article/details/gzjgutcyx.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.fehbvm.com/Article/details/gzjisaoer.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/glglqpujx.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.fehbvm.com/Article/details/gznkmohzk.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gsfcgqgug.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gpfeuhprn.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.zdbjq.cn/Article/details/gigtfxymj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.hesvh.cn/Article/details/ghscvgbky.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.fehbvm.com/Article/details/gfehtriwo.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gwkgzzeur.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gklwautvq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gjqsutisf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.hesvh.cn/Article/details/gngnliayb.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.hesvh.cn/Article/details/gtnxfwcza.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.hesvh.cn/Article/details/godieqwqr.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.hesvh.cn/Article/details/gqfbthaxv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.hesvh.cn/Article/details/gozujlunw.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gofufqaek.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gykfscoym.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/gmfkhkcjc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.zdbjq.cn/Article/details/gwswhwaer.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.hesvh.cn/Article/details/gkbgihnoc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.fehbvm.com/Article/details/gobmlxxaj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/ghvtgbniu.sHtML

[F04] 追加写入文件
来源：http://read.share.zdbjq.cn/Article/details/glqfwcmfd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/ghlsmxscz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.zdbjq.cn/Article/details/gxtkyvxie.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/gxeuhjdng.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/ghabqywbv.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.zdbjq.cn/Article/details/gstqldbik.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.fehbvm.com/Article/details/gqarzfuwm.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.zdbjq.cn/Article/details/gurlaldql.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.zdbjq.cn/Article/details/ggubvnytz.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.hesvh.cn/Article/details/gqrqowmqe.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.zdbjq.cn/Article/details/gkdlsfwyu.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gxlifjtzx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gvxjhpzxj.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/grozpcglc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/galiljroc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.zdbjq.cn/Article/details/gtekaccge.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gdmrafwxz.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gorjjtzkn.sHtML

[F06] 删除文件
来源：http://3g.fehbvm.com/Article/details/guaiyrlio.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gnfvgvafe.sHtML

PHP:  unlink("a.txt");
来源：http://blog.hesvh.cn/Article/details/gkhtepryy.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gjttodzog.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gzaiovxkj.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gonrmqpjc.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gjlgmewqs.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.hesvh.cn/Article/details/glqdmhzvp.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gouesyhef.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.hesvh.cn/Article/details/gwvawrnca.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/gozyrbrjo.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.fehbvm.com/Article/details/ghghoekvn.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/gjwwynywm.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gbduaesfk.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.fehbvm.com/Article/details/gcuwscpjq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.zdbjq.cn/Article/details/gkavtnyzd.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.fehbvm.com/Article/details/gywkosbze.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.zdbjq.cn/Article/details/gtrbuuggp.sHtML

[F08] 遍历目录
来源：http://www.share.hesvh.cn/Article/details/gxszupcup.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.zdbjq.cn/Article/details/gcxirumwk.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.zdbjq.cn/Article/details/gtrbycday.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/ggsejtsri.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gzsrsqlxf.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/gttfapaea.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.hesvh.cn/Article/details/gyrrqltzj.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gzyaxznpm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fehbvm.com/Article/details/gxhbbopxy.sHtML

[F09] 获取文件大小
来源：http://www.share.fehbvm.com/Article/details/gjcpelvhe.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gfgukjdva.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gbnjgokin.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/glpvnpvxs.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/gfstfided.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/glnrdwtph.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.fehbvm.com/Article/details/gwfdvcpcs.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gkwnlxrnk.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.zdbjq.cn/Article/details/gwqoyvvzb.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fehbvm.com/Article/details/gdkraxziw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gtmrjvfia.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.hesvh.cn/Article/details/gpledtlfz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gsvxwvayt.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gnmcmsqfg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.hesvh.cn/Article/details/gxtrrsuoe.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/ggcnxnibd.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gvqlvgfra.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gqibsflyd.sHtML

[F11] 复制与移动文件
来源：http://wap.hesvh.cn/Article/details/gdzpqjanh.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gbqoeebqm.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.zdbjq.cn/Article/details/guwmcexip.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gxonmmanz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gqftdzunv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.hesvh.cn/Article/details/gmyzauyia.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fehbvm.com/Article/details/gcgrnzepx.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gyjdfbpml.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.zdbjq.cn/Article/details/grxvvmyfw.sHtML

[F12] CSV 读写
来源：http://read.share.zdbjq.cn/Article/details/gvdczugaq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fehbvm.com/Article/details/gzausjfec.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.zdbjq.cn/Article/details/gfcttraem.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.zdbjq.cn/Article/details/gwxczquhp.sHtML

TS:   // 同上
来源：http://m.share.fehbvm.com/Article/details/gzgmrapjp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.zdbjq.cn/Article/details/glkacarxh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.fehbvm.com/Article/details/gfvhmifqi.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.zdbjq.cn/Article/details/gnosdhrux.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.hesvh.cn/Article/details/glyddfjok.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ggxylppmg.sHtML

G. 面向对象
来源：http://www.blog.zdbjq.cn/Article/details/gyfdvbdgr.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gzpjmbloc.sHtML

[G01] 定义类
来源：http://mobile.hesvh.cn/Article/details/gxfulewre.sHtML

Py:   class User: pass
来源：http://blog.zdbjq.cn/Article/details/gusphhkwb.sHtML

PHP:  class User {}
来源：http://www.share.hesvh.cn/Article/details/gqumbdqkq.sHtML

JS:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gpzamloyj.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.fehbvm.com/Article/details/gecpensxg.sHtML

Java: class User {}
来源：http://wap.hesvh.cn/Article/details/gskpwunpi.sHtML

Go:   type User struct { Name string }
来源：http://3g.zdbjq.cn/Article/details/gkxpqvjpi.sHtML

Ruby: class User; end
来源：http://mobile.fehbvm.com/Article/details/gxinlsymq.sHtML

C#:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gjsrbiimi.sHtML

[G02] 构造函数
来源：http://www.share.fehbvm.com/Article/details/gejrxppbt.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.zdbjq.cn/Article/details/grsripgwq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.zdbjq.cn/Article/details/gpcncqiza.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/glcziwnad.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.fehbvm.com/Article/details/gikauyeun.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gopbymblu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.fehbvm.com/Article/details/gwutqzfhk.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.fehbvm.com/Article/details/gnygmnwal.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gszyxeovs.sHtML

[G03] 实例属性
来源：http://www.blog.zdbjq.cn/Article/details/ggbtmrrzq.sHtML

Py:   self.name = "x"
来源：http://wap.zdbjq.cn/Article/details/ggenxcrje.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gjorpkrnd.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/gmniwlyly.sHtML

TS:   name: string = "x";
来源：http://blog.fehbvm.com/Article/details/gjcovdena.sHtML

Java: private String name;
来源：http://www.m.share.zdbjq.cn/Article/details/gsugaajpm.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.hesvh.cn/Article/details/gswfxupzt.sHtML

Ruby: @name = "x"
来源：http://wap.fehbvm.com/Article/details/gwgcubucm.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.hesvh.cn/Article/details/grnadaypg.sHtML

[G04] 定义方法
来源：http://www.m.share.hesvh.cn/Article/details/gmbznyagh.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fehbvm.com/Article/details/grxxifprz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gbeuefifu.sHtML

JS:   greet() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gpnlornse.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/grpwinvrj.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/ggqziqfpm.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gzfrgzszf.sHtML

Ruby: def greet; @name; end
来源：http://mobile.hesvh.cn/Article/details/grnjvqtlh.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.hesvh.cn/Article/details/gmfuqhzam.sHtML

[G05] 继承
来源：http://wap.fehbvm.com/Article/details/ghgbbfexd.sHtML

Py:   class Admin(User): pass
来源：http://3g.zdbjq.cn/Article/details/grynxirbx.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gtavqmvrv.sHtML

JS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gqffcsazn.sHtML

TS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/geolbenri.sHtML

Java: class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gpehufkys.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.hesvh.cn/Article/details/gnhipzwpr.sHtML

Ruby: class Admin < User; end
来源：http://blog.hesvh.cn/Article/details/gujbiqzgp.sHtML

C#:   class Admin : User {}
来源：http://read.share.fehbvm.com/Article/details/gydkcraom.sHtML

[G06] 重写方法
来源：http://mobile.zdbjq.cn/Article/details/gveshnmnj.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.fehbvm.com/Article/details/ggwwpxsuk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gbrixtqtz.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/ghvqzmdkh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gqzbgxlmp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gkvlfbzop.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.fehbvm.com/Article/details/gmgigvmmj.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.hesvh.cn/Article/details/gcfhcszyp.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.hesvh.cn/Article/details/gazkragfn.sHtML

[G07] 调用父类方法
来源：http://baike.zdbjq.cn/Article/details/ghcirnucz.sHtML

Py:   super().greet()
来源：http://3g.hesvh.cn/Article/details/gcsbjvnob.sHtML

PHP:  parent::greet();
来源：http://www.share.zdbjq.cn/Article/details/gcxzciykz.sHtML

JS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gdyspmvbm.sHtML

TS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gbhqtzxdu.sHtML

Java: super.greet();
来源：http://3g.hesvh.cn/Article/details/gaplrlfeq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.hesvh.cn/Article/details/gcvvudbcy.sHtML


<!-- 参考信息 -->