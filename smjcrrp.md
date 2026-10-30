代发 wailian999

[E14] URL 编码与 Base64
来源：http://mobile.hesvh.cn/Article/details/ghjhdzipa.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.zdbjq.cn/Article/details/gzjthdmwo.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.fehbvm.com/Article/details/gibuirjoe.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.hesvh.cn/Article/details/guliugsjv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.hesvh.cn/Article/details/ggmbfciby.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/giihgakzc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.zdbjq.cn/Article/details/ghwczlwzm.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.fehbvm.com/Article/details/gzlefbnfj.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.hesvh.cn/Article/details/guhdgexop.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.hesvh.cn/Article/details/gubebwbyq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.hesvh.cn/Article/details/gebtteazm.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.zdbjq.cn/Article/details/gewymtjcg.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.fehbvm.com/Article/details/ggbhfycuu.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.zdbjq.cn/Article/details/gafenqkat.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.hesvh.cn/Article/details/gifucixin.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.hesvh.cn/Article/details/gxyjvgdry.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.fehbvm.com/Article/details/gmqcpcewj.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.zdbjq.cn/Article/details/gazuthdej.sHtML

[E16] 数字千分位
来源：http://3g.hesvh.cn/Article/details/gdsizfitr.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.fehbvm.com/Article/details/gyfbijroj.sHtML

PHP:  number_format(1234567);
来源：http://m.share.zdbjq.cn/Article/details/gvxlscyug.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/gqpjfzoex.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/gbvdkgfuq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.fehbvm.com/Article/details/gljwxfztr.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.hesvh.cn/Article/details/guifluwwu.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.fehbvm.com/Article/details/ghlpcepim.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.hesvh.cn/Article/details/gmzhthrll.sHtML

[E17] 首字母大写
来源：http://3g.fehbvm.com/Article/details/gqealtnnz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.zdbjq.cn/Article/details/gsczzyuld.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.fehbvm.com/Article/details/gpfsvwpoi.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/goazexpks.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/ghhehexkj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.hesvh.cn/Article/details/gxxilxviq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.fehbvm.com/Article/details/ghtcqkiok.sHtML

Ruby: s.capitalize
来源：http://read.share.hesvh.cn/Article/details/gcylxnyov.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.zdbjq.cn/Article/details/ghkzlyngk.sHtML

[E18] 模板占位符替换
来源：http://baike.hesvh.cn/Article/details/gypafnvsp.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.zdbjq.cn/Article/details/gddlaemvt.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.zdbjq.cn/Article/details/gmkuvmenz.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gducefcbl.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gyfmljznz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gaaastwkv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gnajjvdqv.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.fehbvm.com/Article/details/gohsihbho.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.hesvh.cn/Article/details/glsaviisj.sHtML

[E19] 多行文本按行拆分
来源：http://wap.fehbvm.com/Article/details/gdsnzzboa.sHtML

Py:   s.splitlines()
来源：http://baike.fehbvm.com/Article/details/gipvkcfls.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gvdygythi.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/gkiougznz.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gmudotjup.sHtML

Java: s.lines().toList()
来源：http://www.m.share.hesvh.cn/Article/details/guxqrwbes.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.hesvh.cn/Article/details/ggjiyxrwq.sHtML

Ruby: s.lines
来源：http://3g.hesvh.cn/Article/details/ghoqzpkdv.sHtML

C#:   s.Split('\n')
来源：http://baike.fehbvm.com/Article/details/gnuashrqa.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.fehbvm.com/Article/details/gjvcqvxtw.sHtML

Py:   if not s:
来源：http://wap.hesvh.cn/Article/details/gbsxcbczv.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.hesvh.cn/Article/details/giupoqzmm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.hesvh.cn/Article/details/grytbngqz.sHtML

TS:   if (s === "") {}
来源：http://www.share.zdbjq.cn/Article/details/gjkutcnsr.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gbmugkfsz.sHtML

Go:   if s == "" {}
来源：http://blog.zdbjq.cn/Article/details/gchkwhgau.sHtML

Ruby: if s.empty?
来源：http://mobile.fehbvm.com/Article/details/gsxgahsbq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.hesvh.cn/Article/details/gjicfyyji.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.fehbvm.com/Article/details/gtivxwkcr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.fehbvm.com/Article/details/gbkifpnjg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gaovmqppf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gfqdgxsqs.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gkwitrkfi.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/ghglthlts.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.hesvh.cn/Article/details/gygutcqga.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/gzhhjxffp.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gmptaoaqj.sHtML

[E22] 字节长度与字符长度
来源：http://blog.hesvh.cn/Article/details/gpifwzuxc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.zdbjq.cn/Article/details/gmhxeacft.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gsdigosbu.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gcgratmkl.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gcjxmeuft.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.zdbjq.cn/Article/details/grancmkxz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.fehbvm.com/Article/details/gdxtethlk.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fehbvm.com/Article/details/gjxgyyspa.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.hesvh.cn/Article/details/glpgtiypy.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ggrarzfxz.sHtML

F. 文件与目录
来源：http://www.share.zdbjq.cn/Article/details/gbkryrfva.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/grpavgomh.sHtML

[F01] 读取整个文件
来源：http://www.share.fehbvm.com/Article/details/geiycujlc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.zdbjq.cn/Article/details/gjhccaarf.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gawescdsw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.zdbjq.cn/Article/details/guejhbscq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gcmdkjuqi.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/giuujbyoo.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fehbvm.com/Article/details/ggeglzryg.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gvonuzmsj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.zdbjq.cn/Article/details/grsrfzihk.sHtML

[F02] 逐行读取文件
来源：http://www.share.hesvh.cn/Article/details/goshizdph.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.fehbvm.com/Article/details/gqrrzqpfl.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.hesvh.cn/Article/details/grpxtqquw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/ghgvpddrd.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gmesedpvc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gicklzyvy.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.fehbvm.com/Article/details/gckxvhgrp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.hesvh.cn/Article/details/ghisxhxbv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.fehbvm.com/Article/details/gfhdpcuom.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fehbvm.com/Article/details/gyuvsppba.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.fehbvm.com/Article/details/gukzsifxi.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gzufcnfqk.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/ghrgzuezm.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gnhbedvjh.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.fehbvm.com/Article/details/glpdzquso.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.fehbvm.com/Article/details/godyhusce.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.hesvh.cn/Article/details/glpcbqnmq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gvwmjlfyg.sHtML

[F04] 追加写入文件
来源：http://www.blog.fehbvm.com/Article/details/gbqbdibwz.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.zdbjq.cn/Article/details/gvzylwcdr.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.hesvh.cn/Article/details/gwkiaquqz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gzvjncccz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/gfhwsmwoz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.hesvh.cn/Article/details/gynaodjib.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.zdbjq.cn/Article/details/gppgbefhi.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.fehbvm.com/Article/details/gfnbuvzfs.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.hesvh.cn/Article/details/gldvexqsq.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.hesvh.cn/Article/details/gtnhqrlke.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.hesvh.cn/Article/details/gwpbnyjhf.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gavlfgfvb.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gdqdfehnt.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gywohqqin.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gxvvahocr.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.hesvh.cn/Article/details/ggiqfltwa.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.fehbvm.com/Article/details/gakzzcrsa.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gxqtwetkb.sHtML

[F06] 删除文件
来源：http://baike.zdbjq.cn/Article/details/gjjmninqe.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gpzpjolqk.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gsvuxowip.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/guxgccfgi.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gbltnoyjp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/ghmrtadqa.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gujblumja.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.hesvh.cn/Article/details/glgnojrjv.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/guzpzsbyc.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.hesvh.cn/Article/details/gwrjwcwrs.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/ghvcctebw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.hesvh.cn/Article/details/ghdxwatbc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gvfapslxv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gsozsnjbc.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.zdbjq.cn/Article/details/gcvjghcue.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.hesvh.cn/Article/details/gckcofgtl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.fehbvm.com/Article/details/gwfnhznjx.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.zdbjq.cn/Article/details/gqahwvjal.sHtML

[F08] 遍历目录
来源：http://mobile.hesvh.cn/Article/details/ggztnugps.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.hesvh.cn/Article/details/gebkvsepx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.zdbjq.cn/Article/details/geqojztqd.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/giswpmtee.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/gibvfvdgk.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gvgnxkxjo.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.zdbjq.cn/Article/details/ghasrpsci.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gsvickjmn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.hesvh.cn/Article/details/gwmnhqwuq.sHtML

[F09] 获取文件大小
来源：http://3g.hesvh.cn/Article/details/gzmuoquyw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gekvnblnq.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gibvohngo.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gajeovihi.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gqxmertax.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/ggoisroec.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.hesvh.cn/Article/details/gthscvbnh.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gfwxhwxtv.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.zdbjq.cn/Article/details/gboqjzcbm.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fehbvm.com/Article/details/gvhixibmi.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gsfvlggtz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.hesvh.cn/Article/details/gsidvuxrv.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/goldmayvp.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.fehbvm.com/Article/details/glykpkurs.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.zdbjq.cn/Article/details/gvwaxxlcm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/ggjecowzp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gkecybxmu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/govjylahm.sHtML

[F11] 复制与移动文件
来源：http://mobile.fehbvm.com/Article/details/gbjljddbs.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gosmfavcd.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.hesvh.cn/Article/details/gyvplbiux.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/grcukegot.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/greyivkda.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fehbvm.com/Article/details/gziwfgsbl.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.fehbvm.com/Article/details/glxuvixaq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gebidaovl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.zdbjq.cn/Article/details/gdmajydmk.sHtML

[F12] CSV 读写
来源：http://baike.fehbvm.com/Article/details/gpvbnmmoj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.hesvh.cn/Article/details/gcmuzbzfk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.fehbvm.com/Article/details/glukvdhyu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.zdbjq.cn/Article/details/gmjxnsvtj.sHtML

TS:   // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/gahgpyqgb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.zdbjq.cn/Article/details/garjvpxvs.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.fehbvm.com/Article/details/gikxrxvac.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.zdbjq.cn/Article/details/gialhmase.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.hesvh.cn/Article/details/goixjzpuk.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gfvtcadzg.sHtML

G. 面向对象
来源：http://baike.zdbjq.cn/Article/details/gfcnlfavw.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gdljjndjv.sHtML

[G01] 定义类
来源：http://www.blog.fehbvm.com/Article/details/gbfdjezeg.sHtML

Py:   class User: pass
来源：http://blog.hesvh.cn/Article/details/gfikqrnju.sHtML

PHP:  class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gedxspzvn.sHtML

JS:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gtiwnrzso.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.fehbvm.com/Article/details/gmrrljkre.sHtML

Java: class User {}
来源：http://m.share.hesvh.cn/Article/details/gncomsccn.sHtML

Go:   type User struct { Name string }
来源：http://read.share.zdbjq.cn/Article/details/grhkfxfjf.sHtML

Ruby: class User; end
来源：http://3g.hesvh.cn/Article/details/gxlihskdp.sHtML

C#:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gztuhcnbs.sHtML

[G02] 构造函数
来源：http://blog.fehbvm.com/Article/details/gnhivsyuu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.hesvh.cn/Article/details/guofbgzzq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.hesvh.cn/Article/details/gfwzdnwnr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gyguahiha.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.hesvh.cn/Article/details/gukwuikzm.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gbziqeqhw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.hesvh.cn/Article/details/gafgiyerd.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.zdbjq.cn/Article/details/gebmrivlb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.hesvh.cn/Article/details/gdavuubrd.sHtML

[G03] 实例属性
来源：http://3g.hesvh.cn/Article/details/gsomcqtzl.sHtML

Py:   self.name = "x"
来源：http://www.share.hesvh.cn/Article/details/gbjdrihks.sHtML

PHP:  public string $name = "x";
来源：http://mobile.zdbjq.cn/Article/details/glwoxcywc.sHtML

JS:   this.name = "x";
来源：http://wap.zdbjq.cn/Article/details/gzdrevsce.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/gaifnmjbh.sHtML

Java: private String name;
来源：http://blog.fehbvm.com/Article/details/gxboaagyz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fehbvm.com/Article/details/gzjjfrfct.sHtML

Ruby: @name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gdwdhfgsp.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.hesvh.cn/Article/details/geozwgsmb.sHtML

[G04] 定义方法
来源：http://m.share.hesvh.cn/Article/details/gnzzzivxi.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gzzourrcn.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gmurjsuxt.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gblcsmyhu.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gqweczmlm.sHtML

Java: String greet() { return name; }
来源：http://blog.hesvh.cn/Article/details/gqtmirdms.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gxusomwvr.sHtML

Ruby: def greet; @name; end
来源：http://mobile.fehbvm.com/Article/details/gbdrfhqgr.sHtML

C#:   public string Greet() => Name;
来源：http://blog.zdbjq.cn/Article/details/gofftpvuh.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/gskbkgeaf.sHtML

Py:   class Admin(User): pass
来源：http://www.share.hesvh.cn/Article/details/gzpfuabsf.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gldmxepnm.sHtML

JS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gegiiypoy.sHtML

TS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/godnnuwqe.sHtML

Java: class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gkhzrofxx.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fehbvm.com/Article/details/glyroejmi.sHtML

Ruby: class Admin < User; end
来源：http://m.share.zdbjq.cn/Article/details/gqiuehnnc.sHtML

C#:   class Admin : User {}
来源：http://3g.zdbjq.cn/Article/details/gxnxixfax.sHtML

[G06] 重写方法
来源：http://wap.hesvh.cn/Article/details/gbbzetiyb.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.hesvh.cn/Article/details/geadznbot.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gkwblfora.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gddawmcgq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gnycjqgtz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gugckeafr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.zdbjq.cn/Article/details/glijhnjbr.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.hesvh.cn/Article/details/gzfgaxnzi.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.hesvh.cn/Article/details/grtvqleui.sHtML

[G07] 调用父类方法
来源：http://blog.zdbjq.cn/Article/details/gmlsfunzr.sHtML

Py:   super().greet()
来源：http://m.share.hesvh.cn/Article/details/gtgyxgezh.sHtML

PHP:  parent::greet();
来源：http://m.share.zdbjq.cn/Article/details/gswgzxvua.sHtML

JS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gnnitdhxd.sHtML

TS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/guztgcfax.sHtML

Java: super.greet();
来源：http://wap.fehbvm.com/Article/details/gpbnftahh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fehbvm.com/Article/details/gweupbcou.sHtML

Ruby: super
来源：http://read.share.zdbjq.cn/Article/details/gbdzeqlbz.sHtML

C#:   base.Greet();
来源：http://www.blog.fehbvm.com/Article/details/goyjljtul.sHtML

[G08] 静态方法与属性
来源：http://www.share.hesvh.cn/Article/details/gtpsltbya.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.fehbvm.com/Article/details/gbmozyihi.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gojfvjfgs.sHtML

JS:   static f() {}
来源：http://3g.zdbjq.cn/Article/details/glrhlsvaj.sHtML

TS:   static f(): void {}
来源：http://baike.hesvh.cn/Article/details/gyvznjzmn.sHtML

Java: static void f() {}
来源：http://m.share.fehbvm.com/Article/details/gttrssljb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.zdbjq.cn/Article/details/gdkyljnfv.sHtML

Ruby: def self.f; end
来源：http://m.share.hesvh.cn/Article/details/gwyaydajh.sHtML

C#:   public static void F() {}
来源：http://3g.hesvh.cn/Article/details/gxjmpysfp.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.hesvh.cn/Article/details/gbmcznrpx.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.zdbjq.cn/Article/details/gcovozmeb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfmvkydqw.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.hesvh.cn/Article/details/gupqmlqqi.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.fehbvm.com/Article/details/grgrsvlfp.sHtML

Java: interface Shape { double area(); }
来源：http://blog.hesvh.cn/Article/details/gheuprzhn.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.fehbvm.com/Article/details/grgdewhci.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.hesvh.cn/Article/details/gompztwpq.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.hesvh.cn/Article/details/gaxysawog.sHtML

[G10] 访问控制
来源：http://www.m.share.fehbvm.com/Article/details/gokbjarfh.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.zdbjq.cn/Article/details/gabtgnbxe.sHtML

PHP:  public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gsxcmoabr.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.hesvh.cn/Article/details/gyyiasmpb.sHtML

TS:   public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/goapzkuhm.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.hesvh.cn/Article/details/gcrcklcfh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.fehbvm.com/Article/details/gigmdnsym.sHtML

Ruby: public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gysyzoztb.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.fehbvm.com/Article/details/gaxriafia.sHtML

[G11] getter / setter
来源：http://www.m.share.fehbvm.com/Article/details/gdigblicf.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.zdbjq.cn/Article/details/gfnlavzog.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gqcwjqlcf.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gdqzmgygc.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gfkwwxyek.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gxhpxotxa.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gaejlqofv.sHtML

Ruby: attr_accessor :name
来源：http://m.share.hesvh.cn/Article/details/gpjhxrnzu.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.hesvh.cn/Article/details/gbklykdpq.sHtML

[G12] 对象转字符串
来源：http://mobile.hesvh.cn/Article/details/ghbvvhfod.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gknxabhru.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/ghohdzwik.sHtML

JS:   toString() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gcmmixlhb.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gngywhlhn.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.fehbvm.com/Article/details/gdobolxuk.sHtML


<!-- 参考信息 -->