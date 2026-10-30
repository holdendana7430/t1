代发 wailian999

Ruby: s.reverse
来源：http://read.share.fehbvm.com/Article/details/grggdsfny.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/ghozcbycn.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.fehbvm.com/Article/details/gawzuroyq.sHtML

Py:   s.count("a")
来源：http://read.share.hesvh.cn/Article/details/gcvbdsecj.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.hesvh.cn/Article/details/gbovqpgrv.sHtML

JS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/gpstqrizu.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/gvaxcgvpv.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.fehbvm.com/Article/details/ganssgaef.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.hesvh.cn/Article/details/gnxchbtbe.sHtML

Ruby: s.count("a")
来源：http://blog.hesvh.cn/Article/details/gpskdgwgg.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.hesvh.cn/Article/details/gzjhwnkcm.sHtML

[E13] 逐字符遍历
来源：http://www.share.zdbjq.cn/Article/details/geoppgnry.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.hesvh.cn/Article/details/gbwkmmafr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.fehbvm.com/Article/details/gsxpozajf.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gddgwtemm.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gpegytrcp.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.fehbvm.com/Article/details/gareclkta.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.hesvh.cn/Article/details/gickajdxf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.zdbjq.cn/Article/details/gwohkqgry.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.hesvh.cn/Article/details/ggopamjgk.sHtML

[E14] URL 编码与 Base64
来源：http://wap.zdbjq.cn/Article/details/gnxzmxmpy.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fehbvm.com/Article/details/gjmkzozwr.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.zdbjq.cn/Article/details/gfeklxtxk.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.fehbvm.com/Article/details/gcfuzolnt.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.fehbvm.com/Article/details/gskcbcqqt.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fehbvm.com/Article/details/gsxkyisiy.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.zdbjq.cn/Article/details/ghgrfbpvg.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.zdbjq.cn/Article/details/ganegjodc.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.hesvh.cn/Article/details/genjvrryf.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.hesvh.cn/Article/details/gsngaqljv.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.hesvh.cn/Article/details/gapxmvikd.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gdfpmfcps.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.hesvh.cn/Article/details/gxrhadezn.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.zdbjq.cn/Article/details/gtnqajgmy.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.fehbvm.com/Article/details/gicoznlbg.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.hesvh.cn/Article/details/gwsjhxqau.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.hesvh.cn/Article/details/gicxeyxro.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.zdbjq.cn/Article/details/gtfkukegp.sHtML

[E16] 数字千分位
来源：http://mobile.fehbvm.com/Article/details/gsjpclisu.sHtML

Py:   f"{1234567:,}"
来源：http://3g.zdbjq.cn/Article/details/gxxbujlkk.sHtML

PHP:  number_format(1234567);
来源：http://3g.fehbvm.com/Article/details/goanhbxvx.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gzcypncjq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/gflsxkesz.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/gegdbmsfl.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.hesvh.cn/Article/details/ggyqkcvfj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.fehbvm.com/Article/details/ggnpndwvz.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.zdbjq.cn/Article/details/gxhdbgtkw.sHtML

[E17] 首字母大写
来源：http://3g.hesvh.cn/Article/details/gccwgidrz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.hesvh.cn/Article/details/glxqxcaqz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.hesvh.cn/Article/details/gviitwvwp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gqppeksum.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/ghiqbusyp.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.zdbjq.cn/Article/details/gdgpjemov.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.fehbvm.com/Article/details/gijqsgmdm.sHtML

Ruby: s.capitalize
来源：http://baike.zdbjq.cn/Article/details/gugylsebv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.hesvh.cn/Article/details/ggvvovmkr.sHtML

[E18] 模板占位符替换
来源：http://www.blog.zdbjq.cn/Article/details/gbsxwglji.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.fehbvm.com/Article/details/ghgvkxlus.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.fehbvm.com/Article/details/giunghvhy.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gftddvjos.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gkcnzlram.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.fehbvm.com/Article/details/ghiuoxejv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.fehbvm.com/Article/details/gwfjxlfgs.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.fehbvm.com/Article/details/gozbxgeal.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.zdbjq.cn/Article/details/gqcftouew.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fehbvm.com/Article/details/glnoursep.sHtML

Py:   s.splitlines()
来源：http://3g.hesvh.cn/Article/details/gpthkwvyr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gjmpvvnix.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/gvcnimoap.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gyoorxkdf.sHtML

Java: s.lines().toList()
来源：http://www.share.fehbvm.com/Article/details/gtkdbtqif.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.hesvh.cn/Article/details/gjlvhijpd.sHtML

Ruby: s.lines
来源：http://baike.fehbvm.com/Article/details/gigmqqymm.sHtML

C#:   s.Split('\n')
来源：http://www.share.hesvh.cn/Article/details/gyuupzpoc.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.hesvh.cn/Article/details/gmxifvmvs.sHtML

Py:   if not s:
来源：http://read.share.fehbvm.com/Article/details/gmgnrhfyr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.hesvh.cn/Article/details/gxhivbmhs.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.fehbvm.com/Article/details/goktllqcr.sHtML

TS:   if (s === "") {}
来源：http://wap.zdbjq.cn/Article/details/gfmhlzdys.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gaxyquztn.sHtML

Go:   if s == "" {}
来源：http://www.blog.hesvh.cn/Article/details/gaxaweivs.sHtML

Ruby: if s.empty?
来源：http://read.share.zdbjq.cn/Article/details/gmeoityht.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.fehbvm.com/Article/details/gkeadhemo.sHtML

[E21] 超长截断加省略号
来源：http://blog.fehbvm.com/Article/details/gwzsnrkwc.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.zdbjq.cn/Article/details/gmsqbnskw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/gedjxgicg.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/grghexijo.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gdxdfwcle.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gweracwoa.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.fehbvm.com/Article/details/geyzlpxmt.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gvwnmhxcd.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gsarlngdi.sHtML

[E22] 字节长度与字符长度
来源：http://baike.fehbvm.com/Article/details/ghwihefst.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.fehbvm.com/Article/details/gpbtegmdp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/guljxbhsp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/gcwnvhfjt.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gcbdamdjq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gpbdhfyob.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.hesvh.cn/Article/details/gutajcenn.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.hesvh.cn/Article/details/gycksbflq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gkijbdycw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/grykaglsv.sHtML

F. 文件与目录
来源：http://www.blog.zdbjq.cn/Article/details/gtvpspapv.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/guvswqzgw.sHtML

[F01] 读取整个文件
来源：http://mobile.fehbvm.com/Article/details/grxmamiap.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.fehbvm.com/Article/details/gjgxgiifl.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gtbiwlhch.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.hesvh.cn/Article/details/glrxnqxgn.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.fehbvm.com/Article/details/gvjnszqlq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gihrfnbus.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.fehbvm.com/Article/details/gksneoruh.sHtML

Ruby: File.read("a.txt")
来源：http://3g.zdbjq.cn/Article/details/ghsjknsve.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gsjkoxryz.sHtML

[F02] 逐行读取文件
来源：http://www.blog.fehbvm.com/Article/details/gjaekmetj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.zdbjq.cn/Article/details/gbsdawdxo.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.hesvh.cn/Article/details/gquwnwxyr.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/gjptesvqo.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gdsijlqzq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gmxahnmpi.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.hesvh.cn/Article/details/gjxxercbw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.zdbjq.cn/Article/details/gridmqfkd.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.fehbvm.com/Article/details/gfcdpajpl.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.hesvh.cn/Article/details/gfktraibs.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.hesvh.cn/Article/details/ghgetgdyx.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/glcqlbnuf.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gdvdknrfe.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gkawrybxf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.zdbjq.cn/Article/details/gcqtzktrl.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.hesvh.cn/Article/details/gnhpuxmpc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.hesvh.cn/Article/details/gwlsknivr.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/ghpaatulj.sHtML

[F04] 追加写入文件
来源：http://read.share.fehbvm.com/Article/details/gmfaicwxo.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gpblqviic.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.fehbvm.com/Article/details/gfahxyoyd.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gispqcubp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/gkprrefgh.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.fehbvm.com/Article/details/gliviegtz.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.hesvh.cn/Article/details/gkwqanzdf.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.fehbvm.com/Article/details/glvbdbabb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.zdbjq.cn/Article/details/gamaeewwm.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.hesvh.cn/Article/details/gveuedwgu.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.zdbjq.cn/Article/details/gqgfujirz.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gjixpnavv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gfgwdzxte.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gsbhjdcjy.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/glmttgasl.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fehbvm.com/Article/details/glrvrobsa.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.fehbvm.com/Article/details/gbpamoomv.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gadgtuwlw.sHtML

[F06] 删除文件
来源：http://www.m.share.fehbvm.com/Article/details/gvvptqmtl.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/givolprox.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gzunrevtd.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gxcvkhvuw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/giiiejpxk.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gaskljqbm.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gmpxiwxup.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fehbvm.com/Article/details/gqvimukpz.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gsjsnsrwr.sHtML

[F07] 创建目录（含多级）
来源：http://wap.hesvh.cn/Article/details/gphnfpwty.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/ggskjhhor.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gzuhjolzv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/ggmvcfepz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gkhjtrhwq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.zdbjq.cn/Article/details/gdyiblbos.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.hesvh.cn/Article/details/gugmielza.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.zdbjq.cn/Article/details/gufafdlnq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.hesvh.cn/Article/details/gsuycipuj.sHtML

[F08] 遍历目录
来源：http://wap.fehbvm.com/Article/details/gppgxirqq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.zdbjq.cn/Article/details/gfjikuesv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fehbvm.com/Article/details/gmvqkkurz.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/guqnikomm.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gjodcnerr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gygwptzwe.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.fehbvm.com/Article/details/gmchnwkbp.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fehbvm.com/Article/details/ghknuksju.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.zdbjq.cn/Article/details/grnqxscui.sHtML

[F09] 获取文件大小
来源：http://mobile.hesvh.cn/Article/details/guwbzauja.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.zdbjq.cn/Article/details/grqfajsoz.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gvrvswtfs.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/glszthves.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gxbvphemm.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gpmnvierg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fehbvm.com/Article/details/gywektobf.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gwkgqceba.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.zdbjq.cn/Article/details/gvxogicup.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.fehbvm.com/Article/details/gyazttfzl.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gkjrrueso.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.fehbvm.com/Article/details/gvdopbwfm.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gqyaqigbu.sHtML

TS:   path.extname("a.txt")
来源：http://blog.hesvh.cn/Article/details/gapxhwgsd.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.zdbjq.cn/Article/details/gsdaflvhr.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ggpopxoln.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gklofkrly.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gpbtrilnj.sHtML

[F11] 复制与移动文件
来源：http://baike.fehbvm.com/Article/details/gjzxkxuzy.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gftnqsbqd.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.fehbvm.com/Article/details/gpzuffwqv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gxfnlcnhb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gtajablyu.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.fehbvm.com/Article/details/gfaojcfhl.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fehbvm.com/Article/details/gefiwgrhc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gttuicxcn.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.hesvh.cn/Article/details/gmyjwujox.sHtML

[F12] CSV 读写
来源：http://baike.hesvh.cn/Article/details/ghpypgjni.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.zdbjq.cn/Article/details/gnqhbhqty.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.zdbjq.cn/Article/details/gqqlfjrgp.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.zdbjq.cn/Article/details/gywksjnai.sHtML

TS:   // 同上
来源：http://www.blog.zdbjq.cn/Article/details/gcflkdaoo.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fehbvm.com/Article/details/gdvvrfdmk.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.hesvh.cn/Article/details/gfcfwkzvf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.zdbjq.cn/Article/details/gsoficzhs.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.zdbjq.cn/Article/details/geqfzamzz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gstaxtdac.sHtML

G. 面向对象
来源：http://m.share.fehbvm.com/Article/details/gajcshhfq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqxlbsgln.sHtML

[G01] 定义类
来源：http://www.share.fehbvm.com/Article/details/gmiknkyvq.sHtML

Py:   class User: pass
来源：http://www.blog.fehbvm.com/Article/details/ghptevbyl.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/gjzxxtwqq.sHtML

JS:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/glggvbayc.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.hesvh.cn/Article/details/gbcohssng.sHtML

Java: class User {}
来源：http://wap.fehbvm.com/Article/details/gewlldqmd.sHtML

Go:   type User struct { Name string }
来源：http://3g.zdbjq.cn/Article/details/gkbozupzp.sHtML

Ruby: class User; end
来源：http://www.blog.fehbvm.com/Article/details/gichasask.sHtML

C#:   class User {}
来源：http://3g.fehbvm.com/Article/details/gvbbadjeb.sHtML

[G02] 构造函数
来源：http://3g.fehbvm.com/Article/details/gcltacunx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.zdbjq.cn/Article/details/gkkavgkqp.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.hesvh.cn/Article/details/gifgomcid.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gwltsyfou.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.zdbjq.cn/Article/details/ghojmwnpb.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gbwdkzcob.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fehbvm.com/Article/details/gqyanohro.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.zdbjq.cn/Article/details/ggnkexzym.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.hesvh.cn/Article/details/gdhkxrdnl.sHtML

[G03] 实例属性
来源：http://mobile.zdbjq.cn/Article/details/gmhrbyhms.sHtML

Py:   self.name = "x"
来源：http://m.share.fehbvm.com/Article/details/gcvpcgdlo.sHtML

PHP:  public string $name = "x";
来源：http://mobile.hesvh.cn/Article/details/gnnpqxvlu.sHtML

JS:   this.name = "x";
来源：http://blog.fehbvm.com/Article/details/gbfvctjpm.sHtML

TS:   name: string = "x";
来源：http://blog.fehbvm.com/Article/details/gseksxkdr.sHtML

Java: private String name;
来源：http://mobile.fehbvm.com/Article/details/glomlsfwt.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.hesvh.cn/Article/details/gparnuudm.sHtML

Ruby: @name = "x"
来源：http://3g.zdbjq.cn/Article/details/gaylqjser.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.hesvh.cn/Article/details/gvpanpqdh.sHtML

[G04] 定义方法
来源：http://baike.hesvh.cn/Article/details/gzrhxqchz.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gukevnyxa.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gubelxkuq.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/ggftlbrqi.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gdtugwrsa.sHtML

Java: String greet() { return name; }
来源：http://blog.fehbvm.com/Article/details/gnhkcuhdr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gndgtlugy.sHtML

Ruby: def greet; @name; end
来源：http://mobile.fehbvm.com/Article/details/gflqvkdxr.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fehbvm.com/Article/details/grvzlwqqf.sHtML

[G05] 继承
来源：http://3g.hesvh.cn/Article/details/gvxfqgdya.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/gadzxlyxy.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gkyfoodbk.sHtML

JS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gvzxboylm.sHtML

TS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/glipmybqa.sHtML

Java: class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gsjcfliph.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.hesvh.cn/Article/details/gsuoxsfbd.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/gwurmvkxs.sHtML

C#:   class Admin : User {}
来源：http://read.share.hesvh.cn/Article/details/gtbapznpz.sHtML

[G06] 重写方法
来源：http://mobile.zdbjq.cn/Article/details/gziggbnjn.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.fehbvm.com/Article/details/gvhckmpvk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gufuokuez.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gvgxcbdee.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/glmqivfoa.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gmyxugnkh.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.zdbjq.cn/Article/details/gxfhwmkgf.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.zdbjq.cn/Article/details/gvokhmrak.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.hesvh.cn/Article/details/gpdwsddhy.sHtML

[G07] 调用父类方法
来源：http://www.share.hesvh.cn/Article/details/gkirzuzxi.sHtML

Py:   super().greet()
来源：http://3g.fehbvm.com/Article/details/gywbdozuv.sHtML

PHP:  parent::greet();
来源：http://read.share.hesvh.cn/Article/details/gtkhjwiak.sHtML

JS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gidsnuope.sHtML

TS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/glajhunmx.sHtML

Java: super.greet();
来源：http://baike.zdbjq.cn/Article/details/ghrcuvblj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.zdbjq.cn/Article/details/gsfafvrkl.sHtML

Ruby: super
来源：http://blog.hesvh.cn/Article/details/gwfhjeqyn.sHtML

C#:   base.Greet();
来源：http://www.m.share.hesvh.cn/Article/details/gtmrpubok.sHtML

[G08] 静态方法与属性
来源：http://read.share.fehbvm.com/Article/details/gcgsdmwpt.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.zdbjq.cn/Article/details/gickuqlir.sHtML

PHP:  public static function f() {}
来源：http://read.share.zdbjq.cn/Article/details/gbtlyulaf.sHtML

JS:   static f() {}
来源：http://www.blog.hesvh.cn/Article/details/gbmsonwrr.sHtML

TS:   static f(): void {}
来源：http://www.share.hesvh.cn/Article/details/gydjedngj.sHtML

Java: static void f() {}
来源：http://baike.zdbjq.cn/Article/details/gguqihkdi.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fehbvm.com/Article/details/gccuttivo.sHtML

Ruby: def self.f; end
来源：http://blog.fehbvm.com/Article/details/gyqfuxuwy.sHtML

C#:   public static void F() {}
来源：http://baike.fehbvm.com/Article/details/ggcglfrum.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fehbvm.com/Article/details/gxpgzsdbb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fehbvm.com/Article/details/gaxwxxkhn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.hesvh.cn/Article/details/gpyxgreqr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.zdbjq.cn/Article/details/gfebhpgte.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.hesvh.cn/Article/details/ghljudtpo.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.zdbjq.cn/Article/details/gqljviezj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fehbvm.com/Article/details/gydkcqvnx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.hesvh.cn/Article/details/gibwoinbt.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fehbvm.com/Article/details/gqreitmsf.sHtML

[G10] 访问控制
来源：http://blog.hesvh.cn/Article/details/gdjdwkpww.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.fehbvm.com/Article/details/grizjhydj.sHtML

PHP:  public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/geuiwuwwy.sHtML

JS:   #private 字段；其余公开
来源：http://wap.zdbjq.cn/Article/details/gwkehrzos.sHtML


<!-- 参考信息 -->