代发 wailian999

Go:   strings.Count(s, "a")
来源：http://blog.zdbjq.cn/Article/details/gdozaapvl.sHtML

Ruby: s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gbjmowjdr.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.zdbjq.cn/Article/details/gxuldaeuk.sHtML

[E13] 逐字符遍历
来源：http://www.blog.hesvh.cn/Article/details/gbkdgzwfq.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.zdbjq.cn/Article/details/gtaisrytz.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.zdbjq.cn/Article/details/gwjdxdwgx.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gujsocnzx.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gjfxjlzdx.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.hesvh.cn/Article/details/gspwnsgfl.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.zdbjq.cn/Article/details/gjdhwwcqo.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.fehbvm.com/Article/details/gcwcmflyj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.hesvh.cn/Article/details/gozxtpitu.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.zdbjq.cn/Article/details/ggsgcqekk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.hesvh.cn/Article/details/ggxtiywaf.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.fehbvm.com/Article/details/gremlofod.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fehbvm.com/Article/details/gaqzokvsa.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.hesvh.cn/Article/details/gwxzanltu.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.hesvh.cn/Article/details/gplhkaahv.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.zdbjq.cn/Article/details/gayfnobex.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.fehbvm.com/Article/details/gypmmpbfg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gbivoinjz.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.hesvh.cn/Article/details/giosvviff.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.hesvh.cn/Article/details/gjxxbetoj.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gpssqpdrx.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.hesvh.cn/Article/details/gdjrxryuc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.fehbvm.com/Article/details/gjavhgygu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.zdbjq.cn/Article/details/gnahrtjyt.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.fehbvm.com/Article/details/gtpvurdaw.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.fehbvm.com/Article/details/gjpanwchm.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.fehbvm.com/Article/details/gbpkgriyc.sHtML

[E16] 数字千分位
来源：http://read.share.fehbvm.com/Article/details/gonxgomvh.sHtML

Py:   f"{1234567:,}"
来源：http://3g.zdbjq.cn/Article/details/gixqvnlbi.sHtML

PHP:  number_format(1234567);
来源：http://m.share.zdbjq.cn/Article/details/gzfbvhnfb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gxqtnhcay.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/gfvpfzhcu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/gnuuptowz.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.fehbvm.com/Article/details/gvfncrxbv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.fehbvm.com/Article/details/gvqqbtlrt.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.zdbjq.cn/Article/details/gfwpplcde.sHtML

[E17] 首字母大写
来源：http://wap.fehbvm.com/Article/details/gvdpacomk.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.zdbjq.cn/Article/details/giwcputmj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.hesvh.cn/Article/details/gvteytkcq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gchrbpkxp.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gjongfazp.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.zdbjq.cn/Article/details/ggikroqxw.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.fehbvm.com/Article/details/gdtsmfapf.sHtML

Ruby: s.capitalize
来源：http://m.share.zdbjq.cn/Article/details/gjetbyogx.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.zdbjq.cn/Article/details/gusvuuyki.sHtML

[E18] 模板占位符替换
来源：http://wap.fehbvm.com/Article/details/getnvhrcq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.fehbvm.com/Article/details/gtbfchclb.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.fehbvm.com/Article/details/gpgsptwci.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gwftrtojr.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gytgdwgut.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gwogzhcxf.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gltoyakyt.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.hesvh.cn/Article/details/ghnkxbmfz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.zdbjq.cn/Article/details/ggmystjng.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.zdbjq.cn/Article/details/ghaefcgmq.sHtML

Py:   s.splitlines()
来源：http://www.blog.hesvh.cn/Article/details/gqdsspphn.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gnemxokra.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gpeclxfur.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/gquahkoft.sHtML

Java: s.lines().toList()
来源：http://m.share.hesvh.cn/Article/details/gpujjijvb.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.fehbvm.com/Article/details/gcdzoalxw.sHtML

Ruby: s.lines
来源：http://wap.fehbvm.com/Article/details/gqhscnrnk.sHtML

C#:   s.Split('\n')
来源：http://baike.zdbjq.cn/Article/details/gbwalriym.sHtML

[E20] 判断字符串是否为空
来源：http://wap.hesvh.cn/Article/details/gqnzndylm.sHtML

Py:   if not s:
来源：http://m.share.hesvh.cn/Article/details/ghjgduijz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.hesvh.cn/Article/details/gnboogkjk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.fehbvm.com/Article/details/gwvmxafzz.sHtML

TS:   if (s === "") {}
来源：http://m.share.hesvh.cn/Article/details/goinfhvuv.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gkdiuprup.sHtML

Go:   if s == "" {}
来源：http://read.share.zdbjq.cn/Article/details/gdactuerk.sHtML

Ruby: if s.empty?
来源：http://read.share.fehbvm.com/Article/details/gblvtvosi.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.hesvh.cn/Article/details/gwnxjiwqy.sHtML

[E21] 超长截断加省略号
来源：http://www.share.hesvh.cn/Article/details/gtlijpsgk.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.zdbjq.cn/Article/details/gqtnmbkip.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.hesvh.cn/Article/details/ggsnnjamq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/grhrgmkep.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gfdpaivax.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gtmqvavju.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.zdbjq.cn/Article/details/goiuexceu.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/gseniihcm.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/ghnommnuc.sHtML

[E22] 字节长度与字符长度
来源：http://blog.fehbvm.com/Article/details/gdvsmppnm.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.zdbjq.cn/Article/details/gqowtalje.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gixqjkglo.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/grggaezps.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gkqbhiust.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.fehbvm.com/Article/details/gpgomqlal.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.fehbvm.com/Article/details/ggexnzabu.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.hesvh.cn/Article/details/gmkhxoohz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gelwqwgoy.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gmhenarev.sHtML

F. 文件与目录
来源：http://wap.fehbvm.com/Article/details/ghpyhwquk.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwxwxynay.sHtML

[F01] 读取整个文件
来源：http://read.share.zdbjq.cn/Article/details/gdldsshng.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.hesvh.cn/Article/details/gqqombdkj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gktwniwqg.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.fehbvm.com/Article/details/gizuwmxwx.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gazdcqjgu.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gpkbrxkxk.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.fehbvm.com/Article/details/gecnacmzr.sHtML

Ruby: File.read("a.txt")
来源：http://baike.fehbvm.com/Article/details/gmcgpylmf.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gqfjfazku.sHtML

[F02] 逐行读取文件
来源：http://mobile.fehbvm.com/Article/details/gsvenfbgc.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.zdbjq.cn/Article/details/gtvcncvop.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.zdbjq.cn/Article/details/ghheutvmg.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gmtlgxxky.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gwaxtnhrs.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gjjwfzuiw.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.fehbvm.com/Article/details/gpdwwggnr.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.hesvh.cn/Article/details/gbcqwnjun.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.zdbjq.cn/Article/details/gnfxhkfoc.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.zdbjq.cn/Article/details/gxjqvfndv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.fehbvm.com/Article/details/gbkunyeos.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gogwvlwjf.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gurzamskv.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gznusizui.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.fehbvm.com/Article/details/gzdfgkggp.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.hesvh.cn/Article/details/gjqoyxoda.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gqjgcxqkf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/gpoyjuhzs.sHtML

[F04] 追加写入文件
来源：http://www.share.zdbjq.cn/Article/details/gtawexipi.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gqhpwugfi.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.zdbjq.cn/Article/details/gumsggupn.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gaxpfxcpo.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/ghwtqhhjs.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.fehbvm.com/Article/details/gfwqsfjdo.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.fehbvm.com/Article/details/gbajqbiit.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.hesvh.cn/Article/details/gnmffofhv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.hesvh.cn/Article/details/giwmjdfrt.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.zdbjq.cn/Article/details/gkuxjrxnr.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.hesvh.cn/Article/details/ggtbfxtix.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gpfqapbzw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/glpriweqv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gyahxkiau.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gtuskikkq.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.hesvh.cn/Article/details/gsgqzbfyq.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gqkdnbbzo.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gsyvxyelz.sHtML

[F06] 删除文件
来源：http://www.blog.hesvh.cn/Article/details/glaqiwtmg.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gbaibtcyf.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fehbvm.com/Article/details/gljkjxmbz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gfrsqevqw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gucfugqru.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gravdclla.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gxoiadsxp.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gusfovykh.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gabcrxond.sHtML

[F07] 创建目录（含多级）
来源：http://wap.fehbvm.com/Article/details/gpuyiiixq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/gviprhwts.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.zdbjq.cn/Article/details/gdxpwjtkt.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/gxrbaorsp.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gjzxlnrdo.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fehbvm.com/Article/details/gijodbnqs.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.hesvh.cn/Article/details/gigzhrfle.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.fehbvm.com/Article/details/gphtgutra.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.hesvh.cn/Article/details/gxiztjszn.sHtML

[F08] 遍历目录
来源：http://www.share.zdbjq.cn/Article/details/grcbtgdqx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.fehbvm.com/Article/details/gvotxhnmq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fehbvm.com/Article/details/gxbvgkeit.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/gqfqzpcmp.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gzwznyqxo.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gtpfibwwi.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fehbvm.com/Article/details/gpgbujdmo.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fehbvm.com/Article/details/gygqudvvq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.hesvh.cn/Article/details/gmsijcxdw.sHtML

[F09] 获取文件大小
来源：http://blog.zdbjq.cn/Article/details/gsnzrgktr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.fehbvm.com/Article/details/gmcaquakk.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gkonwnttc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gqdclbahq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/grquwyrar.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/golrrfeqs.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.fehbvm.com/Article/details/gsexevxhk.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fehbvm.com/Article/details/gkacocdxx.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.hesvh.cn/Article/details/ghbospdff.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.hesvh.cn/Article/details/gouhgplfm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gerhapxsy.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/ghcqqpjel.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gqarhohnf.sHtML

TS:   path.extname("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gjnojoysj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.fehbvm.com/Article/details/gjuhevlew.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gzwxypmyp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gdidnwwqr.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gyniuptlq.sHtML

[F11] 复制与移动文件
来源：http://baike.fehbvm.com/Article/details/gogeajvxi.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/ghjfqgszn.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.hesvh.cn/Article/details/gwgwjilqv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gdarghmgt.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gghdxvqsy.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.zdbjq.cn/Article/details/gkpnzkwcu.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.hesvh.cn/Article/details/gydeunzdw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gnfbldtvm.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.zdbjq.cn/Article/details/ggsysktjg.sHtML

[F12] CSV 读写
来源：http://read.share.fehbvm.com/Article/details/glbldahwy.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.zdbjq.cn/Article/details/guhqwrqgy.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.zdbjq.cn/Article/details/gahgbzrij.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.fehbvm.com/Article/details/gtrjvboti.sHtML

TS:   // 同上
来源：http://www.share.zdbjq.cn/Article/details/gmcchkaby.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.hesvh.cn/Article/details/gvyqpcswk.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.hesvh.cn/Article/details/gfvfwkgtz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.hesvh.cn/Article/details/gqidgvgce.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.hesvh.cn/Article/details/gugdbnvns.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gulhcbytu.sHtML

G. 面向对象
来源：http://wap.fehbvm.com/Article/details/gibbfmoov.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gsmrwxfil.sHtML

[G01] 定义类
来源：http://read.share.zdbjq.cn/Article/details/gugaewgvo.sHtML

Py:   class User: pass
来源：http://wap.hesvh.cn/Article/details/glbmoasqv.sHtML

PHP:  class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gecokxnga.sHtML

JS:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/garrvtlru.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.hesvh.cn/Article/details/gsnbtnbgf.sHtML

Java: class User {}
来源：http://www.blog.fehbvm.com/Article/details/gixcqvitx.sHtML

Go:   type User struct { Name string }
来源：http://blog.zdbjq.cn/Article/details/gcaqczhkc.sHtML

Ruby: class User; end
来源：http://www.m.share.hesvh.cn/Article/details/geujyydwi.sHtML

C#:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gtgauschi.sHtML

[G02] 构造函数
来源：http://www.share.fehbvm.com/Article/details/grscpnphi.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.zdbjq.cn/Article/details/gjsauehby.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.fehbvm.com/Article/details/gvbwvjzzx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gduwaknyg.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fehbvm.com/Article/details/golossqwi.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gumdhdxlu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.zdbjq.cn/Article/details/glxoplwxw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.hesvh.cn/Article/details/gkylotxxz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gsqmxnbac.sHtML

[G03] 实例属性
来源：http://www.blog.hesvh.cn/Article/details/gizxtmndn.sHtML

Py:   self.name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gratwfidw.sHtML

PHP:  public string $name = "x";
来源：http://baike.fehbvm.com/Article/details/glxocwfhq.sHtML

JS:   this.name = "x";
来源：http://baike.hesvh.cn/Article/details/ghmsfkcpy.sHtML

TS:   name: string = "x";
来源：http://www.share.zdbjq.cn/Article/details/gnndbkllj.sHtML

Java: private String name;
来源：http://mobile.zdbjq.cn/Article/details/gswhctuxb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.fehbvm.com/Article/details/gmctnzzrd.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/giqsfmnlg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.fehbvm.com/Article/details/gurncvqwr.sHtML

[G04] 定义方法
来源：http://baike.zdbjq.cn/Article/details/gcixsvkil.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gotzsjwnx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gbcuedshc.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/ggyomyeyr.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gevzjpmyo.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gkbbisara.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gdkgrucfm.sHtML

Ruby: def greet; @name; end
来源：http://www.share.zdbjq.cn/Article/details/goxnkshgl.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gtrekvtzd.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/gfykjteln.sHtML

Py:   class Admin(User): pass
来源：http://3g.fehbvm.com/Article/details/gufvndbyq.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gasnqlhep.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gedqbbwbu.sHtML

TS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gyprasezk.sHtML

Java: class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/grjrzxjby.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.hesvh.cn/Article/details/gigwbpvwf.sHtML

Ruby: class Admin < User; end
来源：http://read.share.fehbvm.com/Article/details/gnpshjyjp.sHtML

C#:   class Admin : User {}
来源：http://mobile.zdbjq.cn/Article/details/gokncaaow.sHtML

[G06] 重写方法
来源：http://m.share.fehbvm.com/Article/details/gnahjudfc.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.zdbjq.cn/Article/details/gavsmcqim.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gvekwcwaq.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gqfrvkmrk.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gdvammjqc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gzjaembss.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.hesvh.cn/Article/details/gvabmlxrc.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.hesvh.cn/Article/details/gtsjnebbx.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fehbvm.com/Article/details/guygxckjp.sHtML

[G07] 调用父类方法
来源：http://www.share.zdbjq.cn/Article/details/gifocyzic.sHtML

Py:   super().greet()
来源：http://www.m.share.zdbjq.cn/Article/details/gbezlknry.sHtML

PHP:  parent::greet();
来源：http://baike.fehbvm.com/Article/details/gstuqvkmv.sHtML

JS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/gwtyvnndq.sHtML

TS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gvfbpaqkc.sHtML

Java: super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gegvuajng.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.fehbvm.com/Article/details/gjgdtwuem.sHtML

Ruby: super
来源：http://baike.hesvh.cn/Article/details/gppcwrpqm.sHtML

C#:   base.Greet();
来源：http://baike.hesvh.cn/Article/details/glbrgzsoh.sHtML

[G08] 静态方法与属性
来源：http://baike.zdbjq.cn/Article/details/gqmbmztru.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.hesvh.cn/Article/details/gacdycaof.sHtML

PHP:  public static function f() {}
来源：http://baike.hesvh.cn/Article/details/gomsftunu.sHtML

JS:   static f() {}
来源：http://www.blog.hesvh.cn/Article/details/gfkiydsdg.sHtML

TS:   static f(): void {}
来源：http://www.blog.hesvh.cn/Article/details/gehizukjk.sHtML

Java: static void f() {}
来源：http://wap.fehbvm.com/Article/details/gkwsrvqce.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.hesvh.cn/Article/details/gvugipgew.sHtML

Ruby: def self.f; end
来源：http://m.share.zdbjq.cn/Article/details/gashbuykj.sHtML

C#:   public static void F() {}
来源：http://m.share.fehbvm.com/Article/details/gdrpebgpd.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.zdbjq.cn/Article/details/glggypuqv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.hesvh.cn/Article/details/gspagxhkf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.hesvh.cn/Article/details/gmusbpniz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.fehbvm.com/Article/details/ghyiayful.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.hesvh.cn/Article/details/glbwaaxsm.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fehbvm.com/Article/details/gshakfhla.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.zdbjq.cn/Article/details/gnowrzzhg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.zdbjq.cn/Article/details/gsmelefem.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.zdbjq.cn/Article/details/gtkzlzxzo.sHtML

[G10] 访问控制
来源：http://www.share.zdbjq.cn/Article/details/gcbxhgflh.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.fehbvm.com/Article/details/gpgqoyntg.sHtML

PHP:  public / protected / private
来源：http://3g.hesvh.cn/Article/details/gvbghofcr.sHtML

JS:   #private 字段；其余公开
来源：http://wap.zdbjq.cn/Article/details/gcoixexwz.sHtML

TS:   public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gpukeslzt.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fehbvm.com/Article/details/gxpwtxrqp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.zdbjq.cn/Article/details/gomhqagbx.sHtML

Ruby: public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gksueorsg.sHtML

C#:   public / protected / private / internal
来源：http://wap.hesvh.cn/Article/details/grszytbwd.sHtML

[G11] getter / setter
来源：http://www.m.share.hesvh.cn/Article/details/gnypdkuim.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.zdbjq.cn/Article/details/gsuzmlvua.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gdwnmywek.sHtML


<!-- 参考信息 -->