代发 wailian999

Go:   strings.Count(s, "a")
来源：http://m.share.fanxiaobao.xyz/Article/details/gngyvpnpu.sHtML

Ruby: s.count("a")
来源：http://www.share.fanxiaobao.xyz/Article/details/gufgqwjae.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrraeftx.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gangcgswi.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswzqumft.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.fanxiaobao.xyz/Article/details/gymwewuou.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gaagvwvrw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjceooliw.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.fanxiaobao.xyz/Article/details/gdaqmwbrq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gqsphuice.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gegrmhuog.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdwtsntk.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmkvwmkq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fanxiaobao.xyz/Article/details/gpmjvqkzr.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwljpxhvp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fanxiaobao.xyz/Article/details/giyfhoqnz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gpzsvwqpt.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gonbqcebg.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fanxiaobao.xyz/Article/details/glbnmqzgp.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.fanxiaobao.xyz/Article/details/goyhuipws.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.fanxiaobao.xyz/Article/details/gwcnsrcwn.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpqtrhhe.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/geuzwbztl.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.fanxiaobao.xyz/Article/details/gllivbarh.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbykktff.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gbyosjkje.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.fanxiaobao.xyz/Article/details/gcexwmdms.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/guifljaks.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjeqibbxb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gppfnzcsf.sHtML

[E16] 数字千分位
来源：http://www.blog.fanxiaobao.xyz/Article/details/grobmptnx.sHtML

Py:   f"{1234567:,}"
来源：http://wap.fanxiaobao.xyz/Article/details/grlinylou.sHtML

PHP:  number_format(1234567);
来源：http://wap.fanxiaobao.xyz/Article/details/guqigdftx.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqlolrvj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.fanxiaobao.xyz/Article/details/gdurzghos.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.fanxiaobao.xyz/Article/details/gzbnztcbe.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fanxiaobao.xyz/Article/details/gslxteute.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.fanxiaobao.xyz/Article/details/gysyxuxht.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.fanxiaobao.xyz/Article/details/gccswzdwy.sHtML

[E17] 首字母大写
来源：http://m.share.fanxiaobao.xyz/Article/details/gllhiiikt.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.fanxiaobao.xyz/Article/details/gteuhxtrd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.fanxiaobao.xyz/Article/details/giuwfklme.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gktwwbzfl.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdphcrkc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gdpvepihf.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.fanxiaobao.xyz/Article/details/gidhhpabh.sHtML

Ruby: s.capitalize
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhkyloyk.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqcjpdko.sHtML

[E18] 模板占位符替换
来源：http://3g.fanxiaobao.xyz/Article/details/gkruufrhh.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.fanxiaobao.xyz/Article/details/gwvgbfbpq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfurivgl.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.fanxiaobao.xyz/Article/details/gfqrhtjxk.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvykunlys.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.fanxiaobao.xyz/Article/details/gjdmtgrgh.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.fanxiaobao.xyz/Article/details/gftojocgw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.fanxiaobao.xyz/Article/details/gxlyhhgep.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gijrbrczg.sHtML

[E19] 多行文本按行拆分
来源：http://baike.fanxiaobao.xyz/Article/details/gcoijxjyc.sHtML

Py:   s.splitlines()
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfhubcer.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkdnjuus.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebfsbrib.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsisjzdqf.sHtML

Java: s.lines().toList()
来源：http://3g.fanxiaobao.xyz/Article/details/gwzzidqkm.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.fanxiaobao.xyz/Article/details/gfwzydyjo.sHtML

Ruby: s.lines
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbddscwc.sHtML

C#:   s.Split('\n')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhxlabcn.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwnlbuad.sHtML

Py:   if not s:
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtlcphks.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.fanxiaobao.xyz/Article/details/gsvjpscdp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fanxiaobao.xyz/Article/details/guiznimgc.sHtML

TS:   if (s === "") {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/guloyiefn.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gcellbcbw.sHtML

Go:   if s == "" {}
来源：http://baike.fanxiaobao.xyz/Article/details/gpgiieues.sHtML

Ruby: if s.empty?
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgnuzpmx.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.fanxiaobao.xyz/Article/details/genwwzngp.sHtML

[E21] 超长截断加省略号
来源：http://blog.fanxiaobao.xyz/Article/details/gytbmlhuc.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzyglwcd.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.fanxiaobao.xyz/Article/details/glvzjxkjq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfkhdwaq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fanxiaobao.xyz/Article/details/gshskbpaa.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.fanxiaobao.xyz/Article/details/gsjwlpjiz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.fanxiaobao.xyz/Article/details/gewtiuovb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmfdjnrj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.fanxiaobao.xyz/Article/details/gbpwitlvh.sHtML

[E22] 字节长度与字符长度
来源：http://baike.fanxiaobao.xyz/Article/details/gecyhciiu.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.fanxiaobao.xyz/Article/details/glcskxlkb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fanxiaobao.xyz/Article/details/gaywgjhia.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnczbdibd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdcvamno.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.fanxiaobao.xyz/Article/details/gbdmjtxdc.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.fanxiaobao.xyz/Article/details/gbemtcfdt.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fanxiaobao.xyz/Article/details/grafdgqgq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstfjvyig.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/ghkpypgca.sHtML

F. 文件与目录
来源：http://3g.fanxiaobao.xyz/Article/details/ggwwhcwxz.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxmutlai.sHtML

[F01] 读取整个文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaykzfczb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.fanxiaobao.xyz/Article/details/giudpstnd.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/gijexqldc.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.fanxiaobao.xyz/Article/details/gymsfhjip.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.fanxiaobao.xyz/Article/details/gtteddqaf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntvfcmip.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.fanxiaobao.xyz/Article/details/gshxydesl.sHtML

Ruby: File.read("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gyglngwty.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.fanxiaobao.xyz/Article/details/gbhxhzvce.sHtML

[F02] 逐行读取文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfxlflqf.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.fanxiaobao.xyz/Article/details/guquuyxjz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.fanxiaobao.xyz/Article/details/geqgkpnid.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fanxiaobao.xyz/Article/details/ghwocpeqp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmilsxuu.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.fanxiaobao.xyz/Article/details/gtdarojrq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gijhtrbyo.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofksqtxu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcibxdsxr.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fanxiaobao.xyz/Article/details/gzfqntlpo.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.fanxiaobao.xyz/Article/details/gvqgouesg.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gtojvcqmb.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fanxiaobao.xyz/Article/details/gqzjfhgkl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fanxiaobao.xyz/Article/details/gubpumfdw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.fanxiaobao.xyz/Article/details/gpaedirze.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfnfoust.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.fanxiaobao.xyz/Article/details/gjumtknff.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/gblcjtkup.sHtML

[F04] 追加写入文件
来源：http://baike.fanxiaobao.xyz/Article/details/gtfouogfk.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.fanxiaobao.xyz/Article/details/gdodwpeaq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.fanxiaobao.xyz/Article/details/gmgfoqubm.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glyhlobxl.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwkpeojw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczbbdhxf.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fanxiaobao.xyz/Article/details/gekoehewp.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.fanxiaobao.xyz/Article/details/geawsstpt.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.fanxiaobao.xyz/Article/details/goosmnxyx.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gtwkdyqzi.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyrwgmpw.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojyjsxin.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqhipqid.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gzbikagcf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.fanxiaobao.xyz/Article/details/gdbmqssrf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplmifzxn.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gnldqmytv.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grlgaphme.sHtML

[F06] 删除文件
来源：http://baike.fanxiaobao.xyz/Article/details/gysttdppg.sHtML

Py:   os.remove("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gighzirwc.sHtML

PHP:  unlink("a.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/gjytttapq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gaztltnly.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gjziebcfh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.fanxiaobao.xyz/Article/details/gngfzghjk.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gbswmzfsq.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gnwnjxres.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.fanxiaobao.xyz/Article/details/gdnktapxp.sHtML

[F07] 创建目录（含多级）
来源：http://wap.fanxiaobao.xyz/Article/details/gptdvlaho.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjsxzktup.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.fanxiaobao.xyz/Article/details/gicgtnqno.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fanxiaobao.xyz/Article/details/gaduvuqnc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfunkrfjl.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.fanxiaobao.xyz/Article/details/gevxvjgjy.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.fanxiaobao.xyz/Article/details/gleukdeas.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.fanxiaobao.xyz/Article/details/ghrbwexhu.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.fanxiaobao.xyz/Article/details/govhryyiq.sHtML

[F08] 遍历目录
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gloucipdk.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixhmaxzu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtxylleb.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgsfyaji.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshraiigp.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakxmlurl.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.fanxiaobao.xyz/Article/details/glapzwwgh.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fanxiaobao.xyz/Article/details/gujjcnjev.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fanxiaobao.xyz/Article/details/gnrylmnnv.sHtML

[F09] 获取文件大小
来源：http://baike.fanxiaobao.xyz/Article/details/gkqrlgtrl.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gcrijafdj.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.fanxiaobao.xyz/Article/details/gibcxlkuw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fanxiaobao.xyz/Article/details/gaaqtfvhu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fanxiaobao.xyz/Article/details/geignnznh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpympuyw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggsqdjxqu.sHtML

Ruby: File.size("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gpzkytftc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.fanxiaobao.xyz/Article/details/gjtbstksz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fanxiaobao.xyz/Article/details/gozregrng.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gcqgxoxqo.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/govtzsnbt.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gfyforvwp.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gnodydzqp.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.fanxiaobao.xyz/Article/details/gopzkgsvz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfumwuzhm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gzqueganb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gjcrhzrue.sHtML

[F11] 复制与移动文件
来源：http://wap.fanxiaobao.xyz/Article/details/gmryoxoeg.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbrikdlps.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.fanxiaobao.xyz/Article/details/geitbuhbq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/ghigdozgt.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gxlsgmcuy.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpnsoqado.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.fanxiaobao.xyz/Article/details/gqxdfehgu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtorvhat.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdehqneyu.sHtML

[F12] CSV 读写
来源：http://wap.fanxiaobao.xyz/Article/details/gvirpduwf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.fanxiaobao.xyz/Article/details/gohrpfvuk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwstrfvd.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.fanxiaobao.xyz/Article/details/gydhmmeyy.sHtML

TS:   // 同上
来源：http://3g.fanxiaobao.xyz/Article/details/gtqpoqhpe.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqhioghh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxmsoyfz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gacyxikwb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giczsopme.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gioutsrqk.sHtML

G. 面向对象
来源：http://baike.fanxiaobao.xyz/Article/details/gwdekhrej.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfddutuf.sHtML

[G01] 定义类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdtcpcwp.sHtML

Py:   class User: pass
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhrsskwi.sHtML

PHP:  class User {}
来源：http://mobile.fanxiaobao.xyz/Article/details/glnzenffw.sHtML

JS:   class User {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gapcumqll.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfibkypvn.sHtML

Java: class User {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gpnctecpj.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtezbumgs.sHtML

Ruby: class User; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxikiejb.sHtML

C#:   class User {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gotpcjtay.sHtML

[G02] 构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaevcnwol.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fanxiaobao.xyz/Article/details/ghsclzbkc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gucazfmad.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjrwiaepd.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjkrmylz.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gjbzhbsmg.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.fanxiaobao.xyz/Article/details/gthrnxcys.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fanxiaobao.xyz/Article/details/geuhnbjxt.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyflswtlz.sHtML

[G03] 实例属性
来源：http://read.share.fanxiaobao.xyz/Article/details/gnsvtpkyl.sHtML

Py:   self.name = "x"
来源：http://wap.fanxiaobao.xyz/Article/details/gioslsnkw.sHtML

PHP:  public string $name = "x";
来源：http://blog.fanxiaobao.xyz/Article/details/gjckllcjf.sHtML

JS:   this.name = "x";
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmburoxx.sHtML

TS:   name: string = "x";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvevhzzsx.sHtML

Java: private String name;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnlbnbzx.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwenrxdjw.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnprcwwhk.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gifrsfwtx.sHtML

[G04] 定义方法
来源：http://www.share.fanxiaobao.xyz/Article/details/gsfzgaozp.sHtML

Py:   def greet(self): return self.name
来源：http://baike.fanxiaobao.xyz/Article/details/gisklbhso.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gsnjnqtru.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpupuarf.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gdsnghfsv.sHtML

Java: String greet() { return name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbkqgemox.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fanxiaobao.xyz/Article/details/gomwqoomh.sHtML

Ruby: def greet; @name; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gphpcdqbe.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.fanxiaobao.xyz/Article/details/golbhuecc.sHtML

[G05] 继承
来源：http://3g.fanxiaobao.xyz/Article/details/gepmhvhoo.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fanxiaobao.xyz/Article/details/guqdmufnb.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gbscjesch.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/grjayhvyq.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbbnpwxp.sHtML

Java: class Admin extends User {}
来源：http://wap.fanxiaobao.xyz/Article/details/glzpyyhkl.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.fanxiaobao.xyz/Article/details/gooueyrvw.sHtML

Ruby: class Admin < User; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gqiioqmjr.sHtML

C#:   class Admin : User {}
来源：http://wap.fanxiaobao.xyz/Article/details/grzaiqfez.sHtML

[G06] 重写方法
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqmulftg.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fanxiaobao.xyz/Article/details/gmhsmeaiz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gnbzxbnud.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqzqwnodn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gayunkyaj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fanxiaobao.xyz/Article/details/ggdyggcsm.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fanxiaobao.xyz/Article/details/gigepfhcr.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.fanxiaobao.xyz/Article/details/gduwmwcif.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fanxiaobao.xyz/Article/details/geqbzledk.sHtML

[G07] 调用父类方法
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxasyskqs.sHtML

Py:   super().greet()
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrjtzhjh.sHtML

PHP:  parent::greet();
来源：http://blog.fanxiaobao.xyz/Article/details/gwyggjzwm.sHtML

JS:   super.greet();
来源：http://wap.fanxiaobao.xyz/Article/details/gkisoaczs.sHtML

TS:   super.greet();
来源：http://baike.fanxiaobao.xyz/Article/details/gevmtzopv.sHtML

Java: super.greet();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjoqgrehu.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fanxiaobao.xyz/Article/details/gnakcbqsf.sHtML

Ruby: super
来源：http://wap.fanxiaobao.xyz/Article/details/gjpqidpem.sHtML

C#:   base.Greet();
来源：http://read.share.fanxiaobao.xyz/Article/details/gizubtqai.sHtML

[G08] 静态方法与属性
来源：http://baike.fanxiaobao.xyz/Article/details/ghmkrovos.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfupaiqs.sHtML

PHP:  public static function f() {}
来源：http://baike.fanxiaobao.xyz/Article/details/gwuztwdsq.sHtML

JS:   static f() {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabxinmuh.sHtML

TS:   static f(): void {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gmeyqajrb.sHtML

Java: static void f() {}
来源：http://baike.fanxiaobao.xyz/Article/details/gtxukpbkv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.fanxiaobao.xyz/Article/details/gkkrtlkbc.sHtML

Ruby: def self.f; end
来源：http://3g.fanxiaobao.xyz/Article/details/ghodnwqpm.sHtML

C#:   public static void F() {}
来源：http://baike.fanxiaobao.xyz/Article/details/gslmtpvhd.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.fanxiaobao.xyz/Article/details/gyrdggypy.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.fanxiaobao.xyz/Article/details/gqwvuxkgh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdokdiey.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.fanxiaobao.xyz/Article/details/gcdvpontv.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.fanxiaobao.xyz/Article/details/gllebcaup.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzsvowqt.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcupkyvz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.fanxiaobao.xyz/Article/details/gpkhlanyf.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fanxiaobao.xyz/Article/details/gpmjbljmn.sHtML

[G10] 访问控制
来源：http://read.share.fanxiaobao.xyz/Article/details/grgrtvkiv.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkudecskm.sHtML

PHP:  public / protected / private
来源：http://3g.fanxiaobao.xyz/Article/details/guylnectu.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.fanxiaobao.xyz/Article/details/gbtvndiiz.sHtML

TS:   public / protected / private
来源：http://read.share.fanxiaobao.xyz/Article/details/gjywoqloc.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fanxiaobao.xyz/Article/details/gjsuwubho.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.fanxiaobao.xyz/Article/details/gbaddgzvq.sHtML

Ruby: public / protected / private
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxfpngbe.sHtML

C#:   public / protected / private / internal
来源：http://mobile.fanxiaobao.xyz/Article/details/gophtbexv.sHtML

[G11] getter / setter
来源：http://blog.fanxiaobao.xyz/Article/details/gevsxlegk.sHtML

Py:   @property 与 @x.setter
来源：http://baike.fanxiaobao.xyz/Article/details/glmozshzi.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjijycppv.sHtML


<!-- 参考信息 -->