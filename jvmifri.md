代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.fehbvm.com/Article/details/gfinhnwlu.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.fehbvm.com/Article/details/gvdcgjsgs.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.hesvh.cn/Article/details/gxwtkslaa.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.fehbvm.com/Article/details/gzaasuyqd.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.hesvh.cn/Article/details/gdhephdie.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.zdbjq.cn/Article/details/gzadqpxce.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.hesvh.cn/Article/details/gfcvzpaze.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.hesvh.cn/Article/details/gyoicexxm.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.fehbvm.com/Article/details/gxawdfsmv.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.hesvh.cn/Article/details/ghieyqjtr.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.hesvh.cn/Article/details/goxdqbdoh.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.hesvh.cn/Article/details/gniyocqsl.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.hesvh.cn/Article/details/gaakpedgb.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.zdbjq.cn/Article/details/gmclmzlbe.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.hesvh.cn/Article/details/gozqcfagw.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fehbvm.com/Article/details/gmsdewfee.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.hesvh.cn/Article/details/gbrrpsfzn.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.fehbvm.com/Article/details/gzgjoddhz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.hesvh.cn/Article/details/givfgnonq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.zdbjq.cn/Article/details/gvqyfnolr.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fehbvm.com/Article/details/gyatayhvi.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.zdbjq.cn/Article/details/gjxkjjjik.sHtML

[E16] 数字千分位
来源：http://3g.hesvh.cn/Article/details/gnmhehfpr.sHtML

Py:   f"{1234567:,}"
来源：http://blog.zdbjq.cn/Article/details/grpvthxrx.sHtML

PHP:  number_format(1234567);
来源：http://mobile.hesvh.cn/Article/details/gzlsrrieh.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/gsuuwulqr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/gwuzbjuge.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.fehbvm.com/Article/details/gosrxzvic.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.hesvh.cn/Article/details/gopbpyhyi.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.fehbvm.com/Article/details/gjfgyyuzr.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.zdbjq.cn/Article/details/gctaxzhzw.sHtML

[E17] 首字母大写
来源：http://baike.zdbjq.cn/Article/details/gkjzcmuzg.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.fehbvm.com/Article/details/gziloqxit.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.zdbjq.cn/Article/details/gjfbhxgnn.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/grytcgxhg.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/guzvctudm.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.zdbjq.cn/Article/details/getorpsuz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.fehbvm.com/Article/details/gjkvwgsna.sHtML

Ruby: s.capitalize
来源：http://m.share.zdbjq.cn/Article/details/gugobfgdz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.zdbjq.cn/Article/details/gaebidcde.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fehbvm.com/Article/details/geehdapoq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.zdbjq.cn/Article/details/gdmeccxjv.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.zdbjq.cn/Article/details/gdhxqfsdv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gabsgttqd.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gwpemrfir.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gitfapnnd.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gvdcsjeqx.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.zdbjq.cn/Article/details/gszyjajrb.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.zdbjq.cn/Article/details/gilnxztth.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.hesvh.cn/Article/details/ggjmyoygw.sHtML

Py:   s.splitlines()
来源：http://blog.hesvh.cn/Article/details/gnwazjrja.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.fehbvm.com/Article/details/gidfqkmkm.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/gmvtmaefw.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gbsdtebkm.sHtML

Java: s.lines().toList()
来源：http://read.share.hesvh.cn/Article/details/gmjxejxhh.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.hesvh.cn/Article/details/gmfiyyazt.sHtML

Ruby: s.lines
来源：http://wap.hesvh.cn/Article/details/gdfxvgzsr.sHtML

C#:   s.Split('\n')
来源：http://read.share.fehbvm.com/Article/details/grsjuqimt.sHtML

[E20] 判断字符串是否为空
来源：http://3g.zdbjq.cn/Article/details/gbkoxqhxn.sHtML

Py:   if not s:
来源：http://www.share.hesvh.cn/Article/details/gdfvkpqkr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.hesvh.cn/Article/details/gvzxmziiz.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.fehbvm.com/Article/details/gyifyisnl.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.fehbvm.com/Article/details/gbhsndkay.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/gnledvhge.sHtML

Go:   if s == "" {}
来源：http://www.m.share.fehbvm.com/Article/details/gxobusvsd.sHtML

Ruby: if s.empty?
来源：http://www.blog.zdbjq.cn/Article/details/grhmuavkl.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.fehbvm.com/Article/details/gayajrfbt.sHtML

[E21] 超长截断加省略号
来源：http://blog.fehbvm.com/Article/details/glicdjnqi.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.zdbjq.cn/Article/details/gaavknnry.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gglfxaggx.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gisdiqgel.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/ggscwfeuo.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/glquionns.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fehbvm.com/Article/details/gtjffdzjz.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gfhvywuwg.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/giukrwbyf.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.zdbjq.cn/Article/details/gjdodjapq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.hesvh.cn/Article/details/gnbumsymr.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gvnhiumgo.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/glcvxvgkp.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gjbvoivsd.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.fehbvm.com/Article/details/gvccqixyw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.hesvh.cn/Article/details/gvdiyyxbr.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.hesvh.cn/Article/details/gbrcazwpq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gqbptlimj.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gwcbiejnr.sHtML

F. 文件与目录
来源：http://wap.zdbjq.cn/Article/details/grejxtfqj.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gscdejvhd.sHtML

[F01] 读取整个文件
来源：http://mobile.hesvh.cn/Article/details/gtphyuhxb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.hesvh.cn/Article/details/gjmakqshn.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.hesvh.cn/Article/details/gjrnjsfqo.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.fehbvm.com/Article/details/ghaoqmtot.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/geymmadza.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/grdhbtane.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.zdbjq.cn/Article/details/gzvqaqhgg.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gnjktwwxr.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gpkzyuzrp.sHtML

[F02] 逐行读取文件
来源：http://mobile.zdbjq.cn/Article/details/gnjcplqmg.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.hesvh.cn/Article/details/gfjgktycv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.fehbvm.com/Article/details/gepiizrck.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/gsiycchyu.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/glzjirvfz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gplliftxy.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.fehbvm.com/Article/details/gpihwtyuc.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.zdbjq.cn/Article/details/gulevpkzw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.hesvh.cn/Article/details/grjhsuoce.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.hesvh.cn/Article/details/gbcfnkood.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.zdbjq.cn/Article/details/gvmafozcs.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gtbunwmiv.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/glgejtfqe.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/gccwhzlnw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.hesvh.cn/Article/details/gpjtbvhok.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.hesvh.cn/Article/details/grhflvqjw.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.hesvh.cn/Article/details/gntkkodga.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/gmzkswulp.sHtML

[F04] 追加写入文件
来源：http://www.m.share.zdbjq.cn/Article/details/gztjfliix.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gndxgrljs.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.zdbjq.cn/Article/details/gzcwmvibc.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gqoffwlem.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/gkfwjiped.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.hesvh.cn/Article/details/grtqmkskt.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.zdbjq.cn/Article/details/gondjevfo.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.zdbjq.cn/Article/details/gjqgxqocj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.hesvh.cn/Article/details/gotlzfanu.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.zdbjq.cn/Article/details/gppnpcokd.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.hesvh.cn/Article/details/goixtesvg.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gwgzeouwl.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gwigxsnyb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gshmcjghy.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gugiqokee.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fehbvm.com/Article/details/grikrybfd.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.fehbvm.com/Article/details/ghqwbbnou.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gamcvoixd.sHtML

[F06] 删除文件
来源：http://mobile.fehbvm.com/Article/details/ggffcnsqc.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gbmvcvqde.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gkpcysjuc.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gqmuwywvd.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/getgirrto.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gugjqpujy.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gtphfoiak.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/glsvybrgi.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.hesvh.cn/Article/details/ghljfohvo.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.zdbjq.cn/Article/details/gyvgvxjpk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/gpcfytinj.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.hesvh.cn/Article/details/ggooaxrqv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gkmhoeqrg.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/gegblnvlf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.zdbjq.cn/Article/details/gvutzvyoh.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.zdbjq.cn/Article/details/gtpdoyevl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.zdbjq.cn/Article/details/gspiyfpmk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.zdbjq.cn/Article/details/gbjiljslb.sHtML

[F08] 遍历目录
来源：http://www.blog.hesvh.cn/Article/details/gqskhaylz.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.zdbjq.cn/Article/details/gqfwpzflz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.zdbjq.cn/Article/details/gsfwriysi.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gjsxzpvtd.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/gxbvkfxuy.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/ggfejuvzn.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.fehbvm.com/Article/details/gctqbliry.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fehbvm.com/Article/details/gqtsudaqe.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/giispkkst.sHtML

[F09] 获取文件大小
来源：http://baike.zdbjq.cn/Article/details/gqvnkekha.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.fehbvm.com/Article/details/gzzpbphti.sHtML

PHP:  filesize("a.txt");
来源：http://blog.fehbvm.com/Article/details/ghvbrtdyd.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gshzjljcr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/ggtbeqqfy.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gokxnyddw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fehbvm.com/Article/details/gdwrwvugi.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gchkrqwml.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.fehbvm.com/Article/details/gaxfkryar.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fehbvm.com/Article/details/gkjcgxoag.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gsmqrlgjs.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.zdbjq.cn/Article/details/gkucimzov.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gaeioqrpm.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gedzlleoh.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.zdbjq.cn/Article/details/gqmjfbydq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gbmhkphrw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gkvcyneeh.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gifkftbaw.sHtML

[F11] 复制与移动文件
来源：http://m.share.fehbvm.com/Article/details/gzfugyexx.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gloprtqur.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gwmdcoagf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/glqdbsfsi.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gqoxcldim.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.hesvh.cn/Article/details/glaahlcwe.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.hesvh.cn/Article/details/gesufbuvd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gbszozqmz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fehbvm.com/Article/details/gmmwqmyct.sHtML

[F12] CSV 读写
来源：http://mobile.fehbvm.com/Article/details/gehupholq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.hesvh.cn/Article/details/goxuglixy.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.zdbjq.cn/Article/details/gqpvkklfn.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.zdbjq.cn/Article/details/gjrhfmiep.sHtML

TS:   // 同上
来源：http://read.share.zdbjq.cn/Article/details/ggsmkgpeu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.zdbjq.cn/Article/details/gxpdfzwoh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.fehbvm.com/Article/details/gycondjye.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.hesvh.cn/Article/details/gzoogmply.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.zdbjq.cn/Article/details/gdbcnpfip.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gwotynuaq.sHtML

G. 面向对象
来源：http://www.share.zdbjq.cn/Article/details/gbroghqhf.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gnzcjszwz.sHtML

[G01] 定义类
来源：http://blog.fehbvm.com/Article/details/gwqxmwmuw.sHtML

Py:   class User: pass
来源：http://read.share.zdbjq.cn/Article/details/gslymnmfo.sHtML

PHP:  class User {}
来源：http://read.share.fehbvm.com/Article/details/gkaienurx.sHtML

JS:   class User {}
来源：http://wap.fehbvm.com/Article/details/gxdvxousa.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fehbvm.com/Article/details/gkzhqqcgw.sHtML

Java: class User {}
来源：http://www.m.share.hesvh.cn/Article/details/goqhusyie.sHtML

Go:   type User struct { Name string }
来源：http://3g.fehbvm.com/Article/details/gesalgejj.sHtML

Ruby: class User; end
来源：http://www.m.share.fehbvm.com/Article/details/gwqmjmrfl.sHtML

C#:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gyzxrqjvi.sHtML

[G02] 构造函数
来源：http://blog.hesvh.cn/Article/details/gjcwrlbci.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.fehbvm.com/Article/details/gvvnqojcm.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.hesvh.cn/Article/details/gucwnpyba.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gkpuaqpem.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.fehbvm.com/Article/details/gtuqdqonk.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/ghtsnldio.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.zdbjq.cn/Article/details/ghwpawzws.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.hesvh.cn/Article/details/glsltngqk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gvwdjsmxp.sHtML

[G03] 实例属性
来源：http://baike.fehbvm.com/Article/details/gsgizrzgj.sHtML

Py:   self.name = "x"
来源：http://wap.zdbjq.cn/Article/details/gqilhugft.sHtML

PHP:  public string $name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gjpmyhgzx.sHtML

JS:   this.name = "x";
来源：http://wap.zdbjq.cn/Article/details/gjiztcrlx.sHtML

TS:   name: string = "x";
来源：http://wap.fehbvm.com/Article/details/gosvombxh.sHtML

Java: private String name;
来源：http://mobile.hesvh.cn/Article/details/gwmltgszj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.zdbjq.cn/Article/details/gwsqphptm.sHtML

Ruby: @name = "x"
来源：http://www.share.fehbvm.com/Article/details/gmvwhntxe.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.zdbjq.cn/Article/details/gjrggovvs.sHtML

[G04] 定义方法
来源：http://3g.fehbvm.com/Article/details/gvlukbkbf.sHtML

Py:   def greet(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gdeegsqhf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gmbvpxwgw.sHtML

JS:   greet() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gvdnzipxn.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/grltedpnf.sHtML

Java: String greet() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gfbckegtc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gbmwixuhi.sHtML

Ruby: def greet; @name; end
来源：http://www.share.hesvh.cn/Article/details/gryqtichh.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fehbvm.com/Article/details/ggivigari.sHtML

[G05] 继承
来源：http://wap.hesvh.cn/Article/details/guppzdvif.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fehbvm.com/Article/details/ggopbljpd.sHtML

PHP:  class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gwnkaalhi.sHtML

JS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gixrzgcdp.sHtML

TS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/griajrzye.sHtML

Java: class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gdnmohbbu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.fehbvm.com/Article/details/gzretxvur.sHtML

Ruby: class Admin < User; end
来源：http://3g.hesvh.cn/Article/details/goomdmujw.sHtML

C#:   class Admin : User {}
来源：http://www.share.fehbvm.com/Article/details/gqiqfkhhl.sHtML

[G06] 重写方法
来源：http://mobile.zdbjq.cn/Article/details/gugkznfcw.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.zdbjq.cn/Article/details/gutlfovtv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gxpusnuwh.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gdvbkqnrs.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gueprrost.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gdccdetnk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fehbvm.com/Article/details/gyjgfovlp.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.hesvh.cn/Article/details/gtyvuvoaf.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.fehbvm.com/Article/details/glygaxtie.sHtML

[G07] 调用父类方法
来源：http://www.m.share.hesvh.cn/Article/details/gguipgibk.sHtML

Py:   super().greet()
来源：http://wap.fehbvm.com/Article/details/ghhuyyqag.sHtML

PHP:  parent::greet();
来源：http://www.m.share.hesvh.cn/Article/details/gybrwndpz.sHtML

JS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gtpkqurjn.sHtML

TS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gndodbiux.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/gusvvzrcu.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fehbvm.com/Article/details/gwwwokxeq.sHtML

Ruby: super
来源：http://3g.zdbjq.cn/Article/details/gxlknnyaj.sHtML

C#:   base.Greet();
来源：http://3g.zdbjq.cn/Article/details/gyfalxbhs.sHtML

[G08] 静态方法与属性
来源：http://wap.fehbvm.com/Article/details/gxdndnfju.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.hesvh.cn/Article/details/gtfemcmnc.sHtML

PHP:  public static function f() {}
来源：http://www.blog.zdbjq.cn/Article/details/ggfyeimtn.sHtML

JS:   static f() {}
来源：http://www.share.zdbjq.cn/Article/details/graousdty.sHtML

TS:   static f(): void {}
来源：http://m.share.fehbvm.com/Article/details/gbrltjhpa.sHtML

Java: static void f() {}
来源：http://baike.zdbjq.cn/Article/details/gnunqlrkl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.hesvh.cn/Article/details/gmfwfqsyb.sHtML

Ruby: def self.f; end
来源：http://www.blog.zdbjq.cn/Article/details/gqcgprogd.sHtML

C#:   public static void F() {}
来源：http://wap.hesvh.cn/Article/details/ghlnpjush.sHtML

[G09] 接口 / 抽象类
来源：http://3g.hesvh.cn/Article/details/gfjpcqxvl.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.zdbjq.cn/Article/details/gsfglkzeb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.fehbvm.com/Article/details/gdhahrydm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.hesvh.cn/Article/details/gehcrlnsf.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.zdbjq.cn/Article/details/gzpjzaeqz.sHtML

Java: interface Shape { double area(); }
来源：http://wap.zdbjq.cn/Article/details/gzstsulzv.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.hesvh.cn/Article/details/gfiglyilz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.hesvh.cn/Article/details/gmezmzjlz.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.hesvh.cn/Article/details/gbkowohjn.sHtML

[G10] 访问控制
来源：http://read.share.zdbjq.cn/Article/details/gjrhmlggg.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.zdbjq.cn/Article/details/gtebptebf.sHtML

PHP:  public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gnmvyzood.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.zdbjq.cn/Article/details/gnxcgxveg.sHtML

TS:   public / protected / private
来源：http://baike.hesvh.cn/Article/details/gycgqurzx.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.hesvh.cn/Article/details/gejdxgjzz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.hesvh.cn/Article/details/ghxdsghyd.sHtML

Ruby: public / protected / private
来源：http://wap.hesvh.cn/Article/details/gaefktsde.sHtML

C#:   public / protected / private / internal
来源：http://m.share.hesvh.cn/Article/details/gmcxfaxsd.sHtML

[G11] getter / setter
来源：http://mobile.fehbvm.com/Article/details/gwgpkmpai.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.zdbjq.cn/Article/details/gsfaksmzf.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/goydlcbrt.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/gdfyzedup.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/glfltrcys.sHtML

Java: public String getName() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gwhicmmxw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gsksdqoik.sHtML

Ruby: attr_accessor :name
来源：http://read.share.fehbvm.com/Article/details/gljqovmsg.sHtML

C#:   public string Name { get; set; }
来源：http://3g.fehbvm.com/Article/details/gdocojuhz.sHtML

[G12] 对象转字符串
来源：http://www.blog.hesvh.cn/Article/details/gwmqrodjz.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gvyusgcsr.sHtML


<!-- 参考信息 -->