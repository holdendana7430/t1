代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.zdbjq.cn/Article/details/gdcdscnro.sHtML

[E11] 反转字符串
来源：http://blog.hesvh.cn/Article/details/gpvzkvdww.sHtML

Py:   s[::-1]
来源：http://wap.hesvh.cn/Article/details/ggdabxfsm.sHtML

PHP:  strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/grocfpuff.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/girftjvdn.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gnipdqggc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gbhzsyned.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.zdbjq.cn/Article/details/gwuvwhuaj.sHtML

Ruby: s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gittficti.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gbrglzuis.sHtML

[E12] 统计某字符出现次数
来源：http://blog.zdbjq.cn/Article/details/gmxdfvqyp.sHtML

Py:   s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gemgftdvs.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.fehbvm.com/Article/details/gboixxhgc.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/gupcigvwk.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gcpdfzkcc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.zdbjq.cn/Article/details/gjlmlqrdo.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.fehbvm.com/Article/details/gdkybgwhq.sHtML

Ruby: s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gvyswxqli.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.zdbjq.cn/Article/details/gwxvlnowg.sHtML

[E13] 逐字符遍历
来源：http://blog.fehbvm.com/Article/details/gdmjmcrih.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.fehbvm.com/Article/details/grlguhlzb.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.hesvh.cn/Article/details/gbxltxnda.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gvwnkyvxj.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/gajdaahhy.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gtkmfszlg.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.fehbvm.com/Article/details/gtwcgeldx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.hesvh.cn/Article/details/gisprpmml.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gnekiegqy.sHtML

[E14] URL 编码与 Base64
来源：http://wap.zdbjq.cn/Article/details/gtvyndrqd.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.fehbvm.com/Article/details/goxghxsrx.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.zdbjq.cn/Article/details/gvdgkqtwc.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.zdbjq.cn/Article/details/gsxevsqxf.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.zdbjq.cn/Article/details/gusmnrzio.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.zdbjq.cn/Article/details/gourxrveq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.fehbvm.com/Article/details/gcyzntupa.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.fehbvm.com/Article/details/gsvhnblhq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.fehbvm.com/Article/details/gmiuuljfg.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.zdbjq.cn/Article/details/gimtkrrmn.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fehbvm.com/Article/details/guqczkawz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.fehbvm.com/Article/details/gtsthcjig.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.zdbjq.cn/Article/details/gunydeulg.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.hesvh.cn/Article/details/grxtvwmzg.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.hesvh.cn/Article/details/gcmrogaoe.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.hesvh.cn/Article/details/gbichoqqg.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.hesvh.cn/Article/details/glozqrofz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.fehbvm.com/Article/details/gmzyiwulh.sHtML

[E16] 数字千分位
来源：http://mobile.fehbvm.com/Article/details/gzcqhcxuo.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.fehbvm.com/Article/details/gmabrdbjj.sHtML

PHP:  number_format(1234567);
来源：http://m.share.hesvh.cn/Article/details/giggyznyn.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/gmqmjerqo.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/gocrnxbnv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.hesvh.cn/Article/details/gvxjcrdgu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.zdbjq.cn/Article/details/gzjpvdjou.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.fehbvm.com/Article/details/gkposbvzo.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.zdbjq.cn/Article/details/gulrhncst.sHtML

[E17] 首字母大写
来源：http://www.m.share.fehbvm.com/Article/details/gljhznqcb.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.fehbvm.com/Article/details/gykxnexns.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.fehbvm.com/Article/details/gqyxcjgsc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/gfliilzez.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gsjnkbdpf.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.fehbvm.com/Article/details/goohthwkh.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.zdbjq.cn/Article/details/gvfwhnsol.sHtML

Ruby: s.capitalize
来源：http://blog.fehbvm.com/Article/details/gfhtmwbrw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.zdbjq.cn/Article/details/ghdfdmrpx.sHtML

[E18] 模板占位符替换
来源：http://blog.hesvh.cn/Article/details/gpzedfelt.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.hesvh.cn/Article/details/gbcoqaejv.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.hesvh.cn/Article/details/glrfxqzng.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gwzavtiue.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gxswaydpr.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gpxuxccyf.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gpwreiatg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.hesvh.cn/Article/details/gxjokigyv.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.zdbjq.cn/Article/details/gzcibkduq.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.zdbjq.cn/Article/details/gnqtlyxxc.sHtML

Py:   s.splitlines()
来源：http://read.share.zdbjq.cn/Article/details/gvupuploc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.hesvh.cn/Article/details/gddpeqyvi.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gqslowrhz.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/ggyxqkfzq.sHtML

Java: s.lines().toList()
来源：http://m.share.fehbvm.com/Article/details/gcuppxhmv.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.fehbvm.com/Article/details/gbywtfpwb.sHtML

Ruby: s.lines
来源：http://www.share.hesvh.cn/Article/details/gdsbiqdve.sHtML

C#:   s.Split('\n')
来源：http://wap.zdbjq.cn/Article/details/gnneeygaq.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.fehbvm.com/Article/details/gseultvqd.sHtML

Py:   if not s:
来源：http://3g.zdbjq.cn/Article/details/geewvrxba.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.hesvh.cn/Article/details/gohgpekej.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.hesvh.cn/Article/details/ggbhmrxcr.sHtML

TS:   if (s === "") {}
来源：http://www.share.fehbvm.com/Article/details/ginainetw.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gfwfamvmt.sHtML

Go:   if s == "" {}
来源：http://baike.hesvh.cn/Article/details/gyrfcqodl.sHtML

Ruby: if s.empty?
来源：http://blog.zdbjq.cn/Article/details/gplrjxjyv.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.hesvh.cn/Article/details/gbjwjbfpk.sHtML

[E21] 超长截断加省略号
来源：http://mobile.zdbjq.cn/Article/details/gozwlvrrd.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fehbvm.com/Article/details/gpcyovenc.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.hesvh.cn/Article/details/geqlnbgtj.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gqaxbejfe.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/ggkfenltd.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gyldovicj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fehbvm.com/Article/details/gnjnzjrkf.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/giauspiyp.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gnjvcvkym.sHtML

[E22] 字节长度与字符长度
来源：http://blog.hesvh.cn/Article/details/gvkyssiit.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.hesvh.cn/Article/details/gmfogjycl.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gupfhpmzv.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gypysnjfr.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gmhuwhlis.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.zdbjq.cn/Article/details/gyjbxrzpb.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.fehbvm.com/Article/details/gxhoeikjs.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fehbvm.com/Article/details/gkkgjibkc.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gtdllxjos.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxvcfxhkn.sHtML

F. 文件与目录
来源：http://mobile.zdbjq.cn/Article/details/gzurrzvic.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gygamaxft.sHtML

[F01] 读取整个文件
来源：http://baike.fehbvm.com/Article/details/gfxxjkvqr.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.hesvh.cn/Article/details/gecychbmo.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/givdhzlrf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.hesvh.cn/Article/details/gprwfonzd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fehbvm.com/Article/details/glkmwasos.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gudqcxbaf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.hesvh.cn/Article/details/gbwqdrrsl.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gfaamcraz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/ghmagtcqz.sHtML

[F02] 逐行读取文件
来源：http://mobile.hesvh.cn/Article/details/gouwatsxf.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.zdbjq.cn/Article/details/gyzpsulbj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.hesvh.cn/Article/details/ggbtlzvbt.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gdifhdomp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gtamaabjb.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gwmecxjuj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.zdbjq.cn/Article/details/gqgdcpyqd.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.fehbvm.com/Article/details/gqhnjuewl.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.hesvh.cn/Article/details/grcnthxbx.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.zdbjq.cn/Article/details/gujlmdasz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.hesvh.cn/Article/details/grsempypk.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/gavgaldjw.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gyvlqklkm.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/grtnhfejr.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.fehbvm.com/Article/details/gxrsyfdpv.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.zdbjq.cn/Article/details/gsitueeuv.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.fehbvm.com/Article/details/gupneyuls.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/gpfbmzllp.sHtML

[F04] 追加写入文件
来源：http://www.m.share.zdbjq.cn/Article/details/gejjvszcn.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.zdbjq.cn/Article/details/geasemvrx.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.zdbjq.cn/Article/details/gfqkkwqmo.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/gnydrwcmp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/goekcqjej.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.zdbjq.cn/Article/details/gnfijjsej.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.fehbvm.com/Article/details/ggiciojxo.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.fehbvm.com/Article/details/gpldueyni.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.zdbjq.cn/Article/details/ghafctosu.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gznwywpll.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.fehbvm.com/Article/details/gjghumpvu.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gmwoioahs.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gfaptbxyc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gzozwotig.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gafxddgox.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.zdbjq.cn/Article/details/gqdmswjof.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gpuitkcos.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gusvmkauv.sHtML

[F06] 删除文件
来源：http://www.share.hesvh.cn/Article/details/gqncyldrm.sHtML

Py:   os.remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gshpsjkmd.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gumzmpobk.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gfqiotbga.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gckyezsme.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gfssuafjo.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gmawqmhwb.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gcsdnvwqm.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gtpplrvyr.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.hesvh.cn/Article/details/gctscvqos.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/ggpphfsac.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.fehbvm.com/Article/details/gcchrtayy.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gfocjwtjk.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gvzgqfnxt.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.zdbjq.cn/Article/details/gmehudptl.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.zdbjq.cn/Article/details/gntrnorcb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.fehbvm.com/Article/details/goekpuihg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.hesvh.cn/Article/details/garcdhyat.sHtML

[F08] 遍历目录
来源：http://mobile.fehbvm.com/Article/details/gxpcugkjr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.zdbjq.cn/Article/details/ghdthqtfy.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjkwihnse.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gpqyekblb.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/gtaaocldy.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gvrnzgsnj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.fehbvm.com/Article/details/gyguzjuny.sHtML

Ruby: Dir.children("dir")
来源：http://3g.hesvh.cn/Article/details/gcqiefxbm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.hesvh.cn/Article/details/gpyectywz.sHtML

[F09] 获取文件大小
来源：http://wap.fehbvm.com/Article/details/gmokupmcp.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.fehbvm.com/Article/details/gubxccctt.sHtML

PHP:  filesize("a.txt");
来源：http://3g.hesvh.cn/Article/details/gqbyycdzz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/geysjgpmy.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gbwfbgqkl.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/ghhhbgznz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fehbvm.com/Article/details/gumcybzwb.sHtML

Ruby: File.size("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gkzxbqbtc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.hesvh.cn/Article/details/gobegxbct.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.zdbjq.cn/Article/details/gigrpqlbj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gflsvyrtt.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gmzmuiund.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gcczvtmzn.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gfvfblmho.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.hesvh.cn/Article/details/gklqclyub.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gttgatayy.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gcutdzefg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gesbpxfbl.sHtML

[F11] 复制与移动文件
来源：http://wap.hesvh.cn/Article/details/gormlkilx.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/ghzmfmhlj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.hesvh.cn/Article/details/gkqfspows.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/goeahdbnn.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/guibxxaex.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gahpukxls.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.hesvh.cn/Article/details/gbzojuiyp.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gthytofqj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.fehbvm.com/Article/details/ghqecqgex.sHtML

[F12] CSV 读写
来源：http://www.share.fehbvm.com/Article/details/gjjjgnaka.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.fehbvm.com/Article/details/ghrmillha.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fehbvm.com/Article/details/gvqznyqqm.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fehbvm.com/Article/details/glpekkpqt.sHtML

TS:   // 同上
来源：http://3g.hesvh.cn/Article/details/gzdpfnemi.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fehbvm.com/Article/details/glpjqysnr.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.hesvh.cn/Article/details/ghokmrtqw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.zdbjq.cn/Article/details/gxhgbzpqt.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fehbvm.com/Article/details/gmcichrig.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gqrcsxnqu.sHtML

G. 面向对象
来源：http://3g.hesvh.cn/Article/details/gzhsjvuyv.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjicnzrks.sHtML

[G01] 定义类
来源：http://blog.zdbjq.cn/Article/details/gnhapznmy.sHtML

Py:   class User: pass
来源：http://mobile.zdbjq.cn/Article/details/gymgocavs.sHtML

PHP:  class User {}
来源：http://www.share.hesvh.cn/Article/details/gomyuzdpg.sHtML

JS:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gooiliqmv.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.hesvh.cn/Article/details/gbchnawwn.sHtML

Java: class User {}
来源：http://wap.fehbvm.com/Article/details/gjogyickr.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.zdbjq.cn/Article/details/gklpvxxyc.sHtML

Ruby: class User; end
来源：http://mobile.fehbvm.com/Article/details/gqdohtrzf.sHtML

C#:   class User {}
来源：http://m.share.hesvh.cn/Article/details/grpvpcmtg.sHtML

[G02] 构造函数
来源：http://m.share.zdbjq.cn/Article/details/ghzufosfm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.hesvh.cn/Article/details/gyvumeogl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.hesvh.cn/Article/details/gflefyrni.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/glppxdmuv.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/ghhbqzjiu.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gmtpjlkdp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fehbvm.com/Article/details/gamktrrhf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.fehbvm.com/Article/details/gmawdorid.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gwvpmdfmo.sHtML

[G03] 实例属性
来源：http://blog.fehbvm.com/Article/details/gnvapjkel.sHtML

Py:   self.name = "x"
来源：http://blog.fehbvm.com/Article/details/gteqvhgtu.sHtML

PHP:  public string $name = "x";
来源：http://wap.hesvh.cn/Article/details/gyetxvkdx.sHtML

JS:   this.name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gumfpvxli.sHtML

TS:   name: string = "x";
来源：http://m.share.zdbjq.cn/Article/details/ghckvrtjl.sHtML

Java: private String name;
来源：http://www.blog.fehbvm.com/Article/details/ggpciimae.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.fehbvm.com/Article/details/gossofnpx.sHtML

Ruby: @name = "x"
来源：http://m.share.fehbvm.com/Article/details/gzhlsufjr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.zdbjq.cn/Article/details/gesrvlhwt.sHtML

[G04] 定义方法
来源：http://read.share.zdbjq.cn/Article/details/gwujztoeu.sHtML

Py:   def greet(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/glhgmscwv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/ggkzgxzym.sHtML

JS:   greet() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gfaqvuquw.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/guvaphubo.sHtML

Java: String greet() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gdlnoocbn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gxrtxtrdx.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gxqvewcwd.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.hesvh.cn/Article/details/gxvflnouq.sHtML

[G05] 继承
来源：http://m.share.zdbjq.cn/Article/details/gwepyrlnq.sHtML

Py:   class Admin(User): pass
来源：http://blog.fehbvm.com/Article/details/gorhcxdkn.sHtML

PHP:  class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gomnjhjqz.sHtML

JS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gbisrqhpr.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbzzevjsm.sHtML

Java: class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gkwdrguio.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.fehbvm.com/Article/details/gvdxjjhwk.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.hesvh.cn/Article/details/gglatmolt.sHtML

C#:   class Admin : User {}
来源：http://www.share.fehbvm.com/Article/details/gdpcksmmk.sHtML

[G06] 重写方法
来源：http://baike.zdbjq.cn/Article/details/gwjqhrjsy.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.zdbjq.cn/Article/details/gtbacoaal.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gvixacasw.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gxuwdyvth.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/grtweisvx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gynknfsqf.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.hesvh.cn/Article/details/gaaekpabj.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.zdbjq.cn/Article/details/gbbowtotl.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.hesvh.cn/Article/details/gnpmyzgzi.sHtML

[G07] 调用父类方法
来源：http://blog.hesvh.cn/Article/details/gcljdzfcr.sHtML

Py:   super().greet()
来源：http://wap.hesvh.cn/Article/details/gwridslpg.sHtML

PHP:  parent::greet();
来源：http://baike.fehbvm.com/Article/details/gubmkvvrt.sHtML

JS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gualvhiom.sHtML

TS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gnxwyrqbq.sHtML

Java: super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gfpwologe.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.zdbjq.cn/Article/details/gudgogdsd.sHtML

Ruby: super
来源：http://www.blog.zdbjq.cn/Article/details/gfuedhztl.sHtML

C#:   base.Greet();
来源：http://read.share.fehbvm.com/Article/details/gghorzdrm.sHtML

[G08] 静态方法与属性
来源：http://mobile.fehbvm.com/Article/details/gkkkcunwg.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fehbvm.com/Article/details/gyrdprvrn.sHtML

PHP:  public static function f() {}
来源：http://3g.hesvh.cn/Article/details/gesvcbwip.sHtML

JS:   static f() {}
来源：http://mobile.hesvh.cn/Article/details/gnbumajsk.sHtML

TS:   static f(): void {}
来源：http://m.share.hesvh.cn/Article/details/gtuenfzgj.sHtML

Java: static void f() {}
来源：http://3g.fehbvm.com/Article/details/gjtbufltv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.fehbvm.com/Article/details/gmpntltax.sHtML

Ruby: def self.f; end
来源：http://www.share.zdbjq.cn/Article/details/gkpqysgdp.sHtML

C#:   public static void F() {}
来源：http://read.share.hesvh.cn/Article/details/glxitbwnn.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.zdbjq.cn/Article/details/goxrajinw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/gatcsvxlz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.hesvh.cn/Article/details/grjzjxfew.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.fehbvm.com/Article/details/gpqypmdtp.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.hesvh.cn/Article/details/gbepzlwqw.sHtML


<!-- 参考信息 -->