代发 wailian999

PHP:  substr_count($s, "a");
来源：http://m.share.fehbvm.com/Article/details/gjxemexcl.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/glusojhox.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gcyenahcv.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.hesvh.cn/Article/details/glspnvqog.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.zdbjq.cn/Article/details/gdblezgne.sHtML

Ruby: s.count("a")
来源：http://blog.hesvh.cn/Article/details/goeifahlh.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.zdbjq.cn/Article/details/gudtfzbrg.sHtML

[E13] 逐字符遍历
来源：http://wap.zdbjq.cn/Article/details/gtbwmnslv.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.zdbjq.cn/Article/details/goocscdoo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcwsniqxg.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/ghvigoqsp.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/grsneqkcx.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gsffpiwow.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.fehbvm.com/Article/details/gljdcjlda.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.zdbjq.cn/Article/details/guvkjrjfg.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gdbpscnbe.sHtML

[E14] URL 编码与 Base64
来源：http://baike.zdbjq.cn/Article/details/gvwxawxbh.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fehbvm.com/Article/details/gzebooair.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.hesvh.cn/Article/details/gcdvnehwp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.hesvh.cn/Article/details/glbufixar.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.fehbvm.com/Article/details/ggwfqpqkx.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gdebvojce.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.hesvh.cn/Article/details/gupvsapfp.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.fehbvm.com/Article/details/gmdbkqxnd.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.hesvh.cn/Article/details/gfqcgxejg.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.hesvh.cn/Article/details/gxclonsvu.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.zdbjq.cn/Article/details/gmjanurgi.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fehbvm.com/Article/details/gamtwcjxz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fehbvm.com/Article/details/gbbodhguq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.hesvh.cn/Article/details/gziqocsbx.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.fehbvm.com/Article/details/gnimarcwu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.zdbjq.cn/Article/details/gypnfpepx.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.hesvh.cn/Article/details/gzakkbsth.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.zdbjq.cn/Article/details/gwtzopcfb.sHtML

[E16] 数字千分位
来源：http://m.share.hesvh.cn/Article/details/gkkncflux.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.fehbvm.com/Article/details/gnxgnonav.sHtML

PHP:  number_format(1234567);
来源：http://mobile.zdbjq.cn/Article/details/gzlatqjcc.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/ggydshpiq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/glihgshvg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.hesvh.cn/Article/details/grahtrawg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.zdbjq.cn/Article/details/gndbeslxl.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.fehbvm.com/Article/details/glqmwygys.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.hesvh.cn/Article/details/ghpieyfvj.sHtML

[E17] 首字母大写
来源：http://m.share.zdbjq.cn/Article/details/gflkzrqjk.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.zdbjq.cn/Article/details/gtjhyniuv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.hesvh.cn/Article/details/gyzuwvlmp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/gkktavywb.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gltbgtwok.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.hesvh.cn/Article/details/gdaibuagm.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.hesvh.cn/Article/details/gijybsydl.sHtML

Ruby: s.capitalize
来源：http://wap.fehbvm.com/Article/details/gvkgptitv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.hesvh.cn/Article/details/gdolwvxyp.sHtML

[E18] 模板占位符替换
来源：http://baike.zdbjq.cn/Article/details/gfoohvqok.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fehbvm.com/Article/details/gjsobnfjk.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.fehbvm.com/Article/details/glxrjsthl.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gjucyfptj.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gefsazrmc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gjtvmvijh.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gkpwlzbhe.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.hesvh.cn/Article/details/gfhtqunxm.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.hesvh.cn/Article/details/gbfbdrzbl.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.hesvh.cn/Article/details/gmrlhqbyc.sHtML

Py:   s.splitlines()
来源：http://3g.hesvh.cn/Article/details/guphtepwi.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gkloazidz.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/gbdrvpnmu.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/gbxbzaczw.sHtML

Java: s.lines().toList()
来源：http://3g.zdbjq.cn/Article/details/gwjhtjzii.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.fehbvm.com/Article/details/gfwwbexco.sHtML

Ruby: s.lines
来源：http://blog.zdbjq.cn/Article/details/gkettxeyk.sHtML

C#:   s.Split('\n')
来源：http://mobile.zdbjq.cn/Article/details/gmzxyqayc.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.hesvh.cn/Article/details/gfpvqtxjn.sHtML

Py:   if not s:
来源：http://read.share.hesvh.cn/Article/details/gfhjcesfa.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.zdbjq.cn/Article/details/gtviyuzbc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/gfckpglks.sHtML

TS:   if (s === "") {}
来源：http://m.share.fehbvm.com/Article/details/gndixgire.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gwtraplbx.sHtML

Go:   if s == "" {}
来源：http://blog.fehbvm.com/Article/details/gciowygde.sHtML

Ruby: if s.empty?
来源：http://blog.fehbvm.com/Article/details/gjhlxtuqk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.fehbvm.com/Article/details/gmdiunhve.sHtML

[E21] 超长截断加省略号
来源：http://baike.fehbvm.com/Article/details/gizcdvhyv.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.hesvh.cn/Article/details/gqqlyuiws.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gxhkhxvsr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gdvozpgjk.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gtbdydgue.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gdiibierq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.zdbjq.cn/Article/details/gqpyubsny.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gapwfqtql.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/genqzpxbf.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.zdbjq.cn/Article/details/gklnpmnyu.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.fehbvm.com/Article/details/gfaihimvk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/goictrgji.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gxdjxgftv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gbizwergo.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.fehbvm.com/Article/details/gbkmitiuu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.hesvh.cn/Article/details/gobefnssd.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fehbvm.com/Article/details/gvhoygeam.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.zdbjq.cn/Article/details/galsulazs.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gglxrlaac.sHtML

F. 文件与目录
来源：http://mobile.fehbvm.com/Article/details/gzzrfwkwg.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjgofjvbs.sHtML

[F01] 读取整个文件
来源：http://www.share.zdbjq.cn/Article/details/glcegyyik.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.fehbvm.com/Article/details/gxhzipgmd.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/glscamemj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fehbvm.com/Article/details/gmgqfmtrc.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.fehbvm.com/Article/details/gwruroxgz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gtpcttzku.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.zdbjq.cn/Article/details/ghpytxmfa.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gfeaoayui.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.zdbjq.cn/Article/details/ghaezxxhl.sHtML

[F02] 逐行读取文件
来源：http://3g.hesvh.cn/Article/details/gpdidviaq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.zdbjq.cn/Article/details/gwicmeqys.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.hesvh.cn/Article/details/gnglhavlr.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gcnkuxtvo.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/ghzlvjiin.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gxnycrrds.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.zdbjq.cn/Article/details/greyqvtxf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.zdbjq.cn/Article/details/gfkbaojzp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.zdbjq.cn/Article/details/gafsytxme.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.zdbjq.cn/Article/details/grmamkjgj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.fehbvm.com/Article/details/ghkqjbvrm.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gprupbtet.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gknnnlhzv.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gqsiuqmpw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.fehbvm.com/Article/details/gmunkfije.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.fehbvm.com/Article/details/gtewnvdum.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gwaltylmy.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/grwmpkqdd.sHtML

[F04] 追加写入文件
来源：http://www.m.share.fehbvm.com/Article/details/gaogkpggd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.hesvh.cn/Article/details/gvctmtubv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.fehbvm.com/Article/details/gijqpdwxp.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gjvatsfcp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/gcwwhnjqn.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.hesvh.cn/Article/details/gflkmjelw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.hesvh.cn/Article/details/gpqxgwnud.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.zdbjq.cn/Article/details/gebxuhgck.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.fehbvm.com/Article/details/gbhfbqaif.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.hesvh.cn/Article/details/gatoybwrr.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.zdbjq.cn/Article/details/glezenlsw.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gbpnjzgmh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gdcocknqm.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gaknbbnqi.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gcrbngila.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.zdbjq.cn/Article/details/gmqaziqft.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.fehbvm.com/Article/details/ghzmhwezv.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gaisnunlo.sHtML

[F06] 删除文件
来源：http://blog.hesvh.cn/Article/details/gridczlxs.sHtML

Py:   os.remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/grlzezeql.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gnqlmtmfx.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gmjenlxmy.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gteprqugt.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gdmlfiakc.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gcxftpssg.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gagnzwzzp.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.zdbjq.cn/Article/details/ggfndhffh.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.hesvh.cn/Article/details/gjqjpnmrp.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/gcejtnrqa.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.zdbjq.cn/Article/details/gdkcbaeuc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gezabrofo.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gxbpetrba.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.fehbvm.com/Article/details/gjsgknquc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.hesvh.cn/Article/details/ggebuxprx.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.zdbjq.cn/Article/details/gxgaircbz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.fehbvm.com/Article/details/gqhtfpmyr.sHtML

[F08] 遍历目录
来源：http://wap.hesvh.cn/Article/details/gisbjvcpf.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.zdbjq.cn/Article/details/giilxbzjy.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.zdbjq.cn/Article/details/gniviwisn.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/gnojiogpz.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gisyvabvg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gxihakbyp.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.hesvh.cn/Article/details/glahpmzvk.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gxqarslot.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.zdbjq.cn/Article/details/gxcvvvkrh.sHtML

[F09] 获取文件大小
来源：http://baike.hesvh.cn/Article/details/gqqwqgpoe.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gvpdckqlq.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gdyewryad.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gfszhthze.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/glmciwuko.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/genmvyvcp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.hesvh.cn/Article/details/gchtzyjvq.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fehbvm.com/Article/details/guwxxouzk.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.hesvh.cn/Article/details/gyprnhkes.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.hesvh.cn/Article/details/gytjbtpua.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/ggjwcrfkc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.hesvh.cn/Article/details/gjpuzmgfl.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/goohnimdm.sHtML

TS:   path.extname("a.txt")
来源：http://baike.hesvh.cn/Article/details/gsnpyohdw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.zdbjq.cn/Article/details/gobyglcyt.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gquqqpzkr.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gnzoxlgng.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gdoqjajja.sHtML

[F11] 复制与移动文件
来源：http://blog.hesvh.cn/Article/details/gskgtoykf.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gnhyitunv.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.zdbjq.cn/Article/details/gfogzjftu.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/glqbtiwks.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gibvuwzna.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.zdbjq.cn/Article/details/gwbfkmpae.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.zdbjq.cn/Article/details/gnirszhjf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gsivmeilk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fehbvm.com/Article/details/gmhpknmkb.sHtML

[F12] CSV 读写
来源：http://baike.zdbjq.cn/Article/details/gguwmzrqp.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.zdbjq.cn/Article/details/gcgsmythh.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.hesvh.cn/Article/details/gbaciaghy.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.hesvh.cn/Article/details/gjgphogus.sHtML

TS:   // 同上
来源：http://blog.fehbvm.com/Article/details/gcgybycnl.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fehbvm.com/Article/details/gbyxibfys.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.fehbvm.com/Article/details/gxsyetnek.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.hesvh.cn/Article/details/gxfocceep.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.zdbjq.cn/Article/details/gktqhqkzl.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gyvppxkfw.sHtML

G. 面向对象
来源：http://read.share.zdbjq.cn/Article/details/gtwuepztm.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gqovqfanf.sHtML

[G01] 定义类
来源：http://baike.fehbvm.com/Article/details/gyrgslnkp.sHtML

Py:   class User: pass
来源：http://www.m.share.fehbvm.com/Article/details/gnhaoosat.sHtML

PHP:  class User {}
来源：http://www.share.hesvh.cn/Article/details/gwweevege.sHtML

JS:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gkkcfrqwz.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.fehbvm.com/Article/details/gtsnfnsqp.sHtML

Java: class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gyxozymgf.sHtML

Go:   type User struct { Name string }
来源：http://m.share.hesvh.cn/Article/details/gxtwgtdnw.sHtML

Ruby: class User; end
来源：http://www.blog.hesvh.cn/Article/details/gnmmkxfmz.sHtML

C#:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gdrlvyoaz.sHtML

[G02] 构造函数
来源：http://www.blog.fehbvm.com/Article/details/garemepak.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.zdbjq.cn/Article/details/geieeghvu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.hesvh.cn/Article/details/gtqymqtut.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gpsxzqjna.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/gdiilmflq.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/grzngnsho.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fehbvm.com/Article/details/gbyslgbkr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.fehbvm.com/Article/details/giozrqezg.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.hesvh.cn/Article/details/gevoyukxz.sHtML

[G03] 实例属性
来源：http://3g.hesvh.cn/Article/details/gibhfigax.sHtML

Py:   self.name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gzdcqullh.sHtML

PHP:  public string $name = "x";
来源：http://3g.zdbjq.cn/Article/details/gfvemflfj.sHtML

JS:   this.name = "x";
来源：http://blog.fehbvm.com/Article/details/gfvhviylt.sHtML

TS:   name: string = "x";
来源：http://m.share.fehbvm.com/Article/details/gcyualgcv.sHtML

Java: private String name;
来源：http://www.share.fehbvm.com/Article/details/gtdwhcfjk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.zdbjq.cn/Article/details/gyafmmvyb.sHtML

Ruby: @name = "x"
来源：http://read.share.fehbvm.com/Article/details/gjkxdtwkp.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.hesvh.cn/Article/details/gqdnlqnmg.sHtML

[G04] 定义方法
来源：http://blog.hesvh.cn/Article/details/goukejwkx.sHtML

Py:   def greet(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/ghtuqaobb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gfsvqgmpg.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gbguksoit.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/glcmjnmjq.sHtML

Java: String greet() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gmfdojekd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gxvzdgxom.sHtML

Ruby: def greet; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gjxkclatv.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fehbvm.com/Article/details/gbdewuydh.sHtML

[G05] 继承
来源：http://wap.fehbvm.com/Article/details/gskuagwec.sHtML

Py:   class Admin(User): pass
来源：http://m.share.hesvh.cn/Article/details/guqffunmo.sHtML

PHP:  class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gkujveyzd.sHtML

JS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gmcmvujzq.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gnjyzrrnq.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gebdqdorf.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.fehbvm.com/Article/details/glcbnppld.sHtML

Ruby: class Admin < User; end
来源：http://3g.fehbvm.com/Article/details/gqsyfuclf.sHtML

C#:   class Admin : User {}
来源：http://m.share.hesvh.cn/Article/details/glwhtjtip.sHtML

[G06] 重写方法
来源：http://read.share.hesvh.cn/Article/details/gifijgeqv.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.zdbjq.cn/Article/details/guszeubff.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/girdilsnc.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gwxsldwqb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gnmydheuh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/ggyblandx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.zdbjq.cn/Article/details/gxqycitff.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.zdbjq.cn/Article/details/gmzcyzinn.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.hesvh.cn/Article/details/gblplqqrm.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/gtrzjpxix.sHtML

Py:   super().greet()
来源：http://mobile.fehbvm.com/Article/details/gqzxalrgq.sHtML

PHP:  parent::greet();
来源：http://wap.fehbvm.com/Article/details/gjrcwrbec.sHtML

JS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gczazymfm.sHtML

TS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gjyqedjqv.sHtML

Java: super.greet();
来源：http://m.share.fehbvm.com/Article/details/gjuorruze.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.zdbjq.cn/Article/details/gxjjilrrk.sHtML

Ruby: super
来源：http://blog.hesvh.cn/Article/details/gmgycdbhp.sHtML

C#:   base.Greet();
来源：http://wap.fehbvm.com/Article/details/gcjaelpba.sHtML

[G08] 静态方法与属性
来源：http://baike.zdbjq.cn/Article/details/giftjnvvf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.zdbjq.cn/Article/details/gxnytvllv.sHtML

PHP:  public static function f() {}
来源：http://mobile.hesvh.cn/Article/details/gntozduzd.sHtML

JS:   static f() {}
来源：http://www.blog.hesvh.cn/Article/details/gjxlwvgsn.sHtML

TS:   static f(): void {}
来源：http://read.share.fehbvm.com/Article/details/ggifhteoi.sHtML

Java: static void f() {}
来源：http://baike.fehbvm.com/Article/details/gfamlpomz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fehbvm.com/Article/details/gkgozgbpw.sHtML

Ruby: def self.f; end
来源：http://read.share.zdbjq.cn/Article/details/gumbujadm.sHtML

C#:   public static void F() {}
来源：http://baike.fehbvm.com/Article/details/gycjuobxr.sHtML

[G09] 接口 / 抽象类
来源：http://3g.zdbjq.cn/Article/details/gdatucxmw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.hesvh.cn/Article/details/gbxlmdcxx.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.zdbjq.cn/Article/details/glyynzkpp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.hesvh.cn/Article/details/gtrehbvra.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.fehbvm.com/Article/details/geevcecql.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gogoovpqm.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.zdbjq.cn/Article/details/guwukfbck.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.zdbjq.cn/Article/details/gdghrguvh.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.fehbvm.com/Article/details/gmxubtchd.sHtML

[G10] 访问控制
来源：http://blog.zdbjq.cn/Article/details/gzpojwsgm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.hesvh.cn/Article/details/gutjfossq.sHtML

PHP:  public / protected / private
来源：http://wap.hesvh.cn/Article/details/ghfovztad.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fehbvm.com/Article/details/gfbylrtmj.sHtML

TS:   public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gikifrare.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fehbvm.com/Article/details/gbrqbiphc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fehbvm.com/Article/details/grfbvxchb.sHtML

Ruby: public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/ghgturpmk.sHtML


<!-- 参考信息 -->