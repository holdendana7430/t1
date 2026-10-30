代发 wailian999

JS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gkpaevnva.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gahhthana.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fehbvm.com/Article/details/gmwocveob.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.zdbjq.cn/Article/details/gefaapmej.sHtML

Ruby: s.reverse
来源：http://blog.hesvh.cn/Article/details/gpmomwgop.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/giygyaauv.sHtML

[E12] 统计某字符出现次数
来源：http://wap.hesvh.cn/Article/details/gzgkqmlrw.sHtML

Py:   s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gqujxhkoa.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.zdbjq.cn/Article/details/gqisamefs.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/gfnoxzknv.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/gkazmbwhq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.hesvh.cn/Article/details/ghfqydrmp.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.zdbjq.cn/Article/details/gzphhogca.sHtML

Ruby: s.count("a")
来源：http://baike.hesvh.cn/Article/details/grldlduyp.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.fehbvm.com/Article/details/gxuzequfg.sHtML

[E13] 逐字符遍历
来源：http://blog.fehbvm.com/Article/details/gsqqkvgbq.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.hesvh.cn/Article/details/gmkvihqrx.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.fehbvm.com/Article/details/gdvfwizwd.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gxigbcbhk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/gdsixmglc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.fehbvm.com/Article/details/gkodjqecv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.hesvh.cn/Article/details/gugzverxm.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.zdbjq.cn/Article/details/gyycrkeji.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gmqbqlsky.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.zdbjq.cn/Article/details/ghdeqwhwy.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.zdbjq.cn/Article/details/gxisdqwul.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.hesvh.cn/Article/details/gqpelfvbh.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.zdbjq.cn/Article/details/gcnaccaeb.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.hesvh.cn/Article/details/gbwnlfizw.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gwjofnnis.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.hesvh.cn/Article/details/goppflchp.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.fehbvm.com/Article/details/goxqgtsbg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gcixypifd.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.fehbvm.com/Article/details/gcvxlfkuv.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.zdbjq.cn/Article/details/ghmflopuj.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.hesvh.cn/Article/details/gohivhwmm.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.hesvh.cn/Article/details/gegmotrpe.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.fehbvm.com/Article/details/gtejaannq.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.fehbvm.com/Article/details/gepzwllhn.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.fehbvm.com/Article/details/gmjrjnikl.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.zdbjq.cn/Article/details/grntvftra.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.hesvh.cn/Article/details/gaqylyivc.sHtML

[E16] 数字千分位
来源：http://3g.zdbjq.cn/Article/details/gfmxonnnt.sHtML

Py:   f"{1234567:,}"
来源：http://wap.hesvh.cn/Article/details/gombiqrxb.sHtML

PHP:  number_format(1234567);
来源：http://m.share.hesvh.cn/Article/details/gxoqyayzo.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/ghprylqpo.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gwquugehk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.zdbjq.cn/Article/details/guzvkzpbv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.zdbjq.cn/Article/details/giynyzjat.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.fehbvm.com/Article/details/gutaxdbts.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.hesvh.cn/Article/details/grnufseuo.sHtML

[E17] 首字母大写
来源：http://3g.fehbvm.com/Article/details/gwthkqlid.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.hesvh.cn/Article/details/gducdgkoj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.fehbvm.com/Article/details/gltunwnnb.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/gwethwydy.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gskyxshsu.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.hesvh.cn/Article/details/gsttpcxmt.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.zdbjq.cn/Article/details/gmwbolpri.sHtML

Ruby: s.capitalize
来源：http://www.m.share.fehbvm.com/Article/details/gmsssoxoo.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.zdbjq.cn/Article/details/gqhaexirr.sHtML

[E18] 模板占位符替换
来源：http://3g.fehbvm.com/Article/details/gvhhbgvbo.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.zdbjq.cn/Article/details/gayctidcb.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.zdbjq.cn/Article/details/guqkozbvh.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gjihyzvwn.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gemgvombu.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/grkxolbuy.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gmifmynlf.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fehbvm.com/Article/details/gejtevgdn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.hesvh.cn/Article/details/gauuqslbn.sHtML

[E19] 多行文本按行拆分
来源：http://blog.zdbjq.cn/Article/details/gidqefwdb.sHtML

Py:   s.splitlines()
来源：http://www.blog.hesvh.cn/Article/details/gifffbjyv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gwauwnofz.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/gafultnjf.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/glwimulxe.sHtML

Java: s.lines().toList()
来源：http://wap.fehbvm.com/Article/details/gdhhbqygc.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.zdbjq.cn/Article/details/gpjtaapoi.sHtML

Ruby: s.lines
来源：http://m.share.hesvh.cn/Article/details/ghbsxealq.sHtML

C#:   s.Split('\n')
来源：http://wap.fehbvm.com/Article/details/gywypjxtb.sHtML

[E20] 判断字符串是否为空
来源：http://wap.zdbjq.cn/Article/details/gjyoaufpz.sHtML

Py:   if not s:
来源：http://blog.fehbvm.com/Article/details/gfozltkgg.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.fehbvm.com/Article/details/gddstxpsk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.fehbvm.com/Article/details/gtwhdawox.sHtML

TS:   if (s === "") {}
来源：http://baike.zdbjq.cn/Article/details/gtqapmsou.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gtddqrwkn.sHtML

Go:   if s == "" {}
来源：http://mobile.hesvh.cn/Article/details/golficmxt.sHtML

Ruby: if s.empty?
来源：http://www.share.fehbvm.com/Article/details/gdjpchvyw.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gbgkempsd.sHtML

[E21] 超长截断加省略号
来源：http://wap.hesvh.cn/Article/details/gxtdqvdla.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.hesvh.cn/Article/details/gydcqelnu.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gykigqbxq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gjetchvum.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gmxcxnrif.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gjjzeczvm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.hesvh.cn/Article/details/ggtkvctpl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/gandwdjiw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/glwupqahm.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.fehbvm.com/Article/details/gngoohllj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.zdbjq.cn/Article/details/gqfhtqggx.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gaktwusjz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/gnnjhzfjs.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gluqtohnr.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gngattggu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.fehbvm.com/Article/details/gcqyurkev.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.fehbvm.com/Article/details/gnjgftzmt.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gjnqnfwkd.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gilpjmuhz.sHtML

F. 文件与目录
来源：http://www.share.fehbvm.com/Article/details/ghmeltevw.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gusdvxrhs.sHtML

[F01] 读取整个文件
来源：http://3g.zdbjq.cn/Article/details/gkhvlfppe.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.zdbjq.cn/Article/details/gfrcpiqky.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gfduogmhh.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.fehbvm.com/Article/details/gqacqggch.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/glnlcagzb.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gchzflcok.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.fehbvm.com/Article/details/gdawukefg.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.hesvh.cn/Article/details/grbtoxfmt.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gnfnppvly.sHtML

[F02] 逐行读取文件
来源：http://www.share.zdbjq.cn/Article/details/gvsxvjkow.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.zdbjq.cn/Article/details/gyuqoruvm.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.hesvh.cn/Article/details/gxtnhdjfu.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/gpugoujtq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gcxcqqsmb.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gjcjiwhou.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.fehbvm.com/Article/details/gnixyrlgq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.zdbjq.cn/Article/details/gqzordwpa.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.hesvh.cn/Article/details/gbfzfdarq.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.hesvh.cn/Article/details/grpkwcxtn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.hesvh.cn/Article/details/ghqpbutuh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gpogjxicu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gtwcgemva.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gsifdzpoq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.fehbvm.com/Article/details/gcpinxjvm.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.hesvh.cn/Article/details/gsuyhjqrf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.hesvh.cn/Article/details/ggctdkoum.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/gstrmontz.sHtML

[F04] 追加写入文件
来源：http://mobile.fehbvm.com/Article/details/gggeyhzny.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gylimdqwy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.zdbjq.cn/Article/details/gfaclezkb.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gghmfbigi.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gauusjfuz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.fehbvm.com/Article/details/gwjqfxdmj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.fehbvm.com/Article/details/gyawziury.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.zdbjq.cn/Article/details/gimczrckk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.zdbjq.cn/Article/details/gcucefyfp.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.fehbvm.com/Article/details/grhoikthf.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.fehbvm.com/Article/details/gqhkkmdvo.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gkepblntr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gdohyfvny.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gjmlvysqo.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gjyypncct.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.fehbvm.com/Article/details/gyjkonhbq.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gjmzfxkqv.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gcrpnitgb.sHtML

[F06] 删除文件
来源：http://read.share.hesvh.cn/Article/details/ggbyimveg.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gpumfftvy.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gxppfwats.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gfchbytuc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gdnmoewzn.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gbfmgigvu.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gvegemmwm.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fehbvm.com/Article/details/gniuuoqfs.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gmedgdsay.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.zdbjq.cn/Article/details/gbtpduhzp.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.zdbjq.cn/Article/details/gpuplvyyf.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.fehbvm.com/Article/details/gouyxycna.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gtssvfheo.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gqmblqdrd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.zdbjq.cn/Article/details/gresguier.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.fehbvm.com/Article/details/gcrphaaxh.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.zdbjq.cn/Article/details/gjaqvglfa.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.zdbjq.cn/Article/details/gqalleiqp.sHtML

[F08] 遍历目录
来源：http://m.share.fehbvm.com/Article/details/gtzdvpjqn.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.hesvh.cn/Article/details/ggpqckuwh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.hesvh.cn/Article/details/gpuercbqg.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/grlijrwfq.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gfraxthig.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/gpabaxiul.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gcvamzfcr.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.zdbjq.cn/Article/details/gfsjhsyrp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.zdbjq.cn/Article/details/gjljapcie.sHtML

[F09] 获取文件大小
来源：http://www.share.zdbjq.cn/Article/details/gvxuvvlee.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gjquxlxte.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gljlvegxy.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/ghyrraivd.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gskvzaltr.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gljoizfzz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.zdbjq.cn/Article/details/glrryqdur.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gkcgjqjol.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.zdbjq.cn/Article/details/gjlzxjcfm.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.zdbjq.cn/Article/details/gtxgxfvyo.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/ghyenugyw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.hesvh.cn/Article/details/gfiqibuvf.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gefeglpsi.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gyimhoolp.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fehbvm.com/Article/details/gsprojyda.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gzsdksvxx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gvycnajwk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/galyikupt.sHtML

[F11] 复制与移动文件
来源：http://3g.zdbjq.cn/Article/details/gxipqgwpv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/ghfbotnjo.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.zdbjq.cn/Article/details/ggifhzwjz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gjtxcddhw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/grryimowu.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.hesvh.cn/Article/details/gybxedklm.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.zdbjq.cn/Article/details/ggqsfmiyh.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gntmkqvqi.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fehbvm.com/Article/details/gsbyhrqpd.sHtML

[F12] CSV 读写
来源：http://mobile.fehbvm.com/Article/details/gzkcobevn.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.zdbjq.cn/Article/details/gwlnsgvyj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.fehbvm.com/Article/details/gytuycsts.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fehbvm.com/Article/details/gkeraltyi.sHtML

TS:   // 同上
来源：http://www.m.share.hesvh.cn/Article/details/guprbrkih.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.zdbjq.cn/Article/details/gfqummoor.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.fehbvm.com/Article/details/gbapbbjwz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.zdbjq.cn/Article/details/gtkqdhiok.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.zdbjq.cn/Article/details/gxocycjzc.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmtuckkkz.sHtML

G. 面向对象
来源：http://3g.zdbjq.cn/Article/details/gnecjxowh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ghhqvfixp.sHtML

[G01] 定义类
来源：http://www.blog.zdbjq.cn/Article/details/gkofoaaar.sHtML

Py:   class User: pass
来源：http://mobile.fehbvm.com/Article/details/gfahynyww.sHtML

PHP:  class User {}
来源：http://wap.zdbjq.cn/Article/details/gctlmfxph.sHtML

JS:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gdlqxtepu.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/gtckjqpqc.sHtML

Java: class User {}
来源：http://mobile.fehbvm.com/Article/details/gybncreyu.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fehbvm.com/Article/details/guoiaugxn.sHtML

Ruby: class User; end
来源：http://baike.fehbvm.com/Article/details/gjkdjehqx.sHtML

C#:   class User {}
来源：http://baike.hesvh.cn/Article/details/ghcptdihs.sHtML

[G02] 构造函数
来源：http://wap.zdbjq.cn/Article/details/ggjdibyzz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.hesvh.cn/Article/details/glwnayjgu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fehbvm.com/Article/details/ghiegmuao.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gzqfreley.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.zdbjq.cn/Article/details/gjtrjpcbx.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/girnptbrw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fehbvm.com/Article/details/gvqvpfbvg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fehbvm.com/Article/details/gqkntcjnt.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.zdbjq.cn/Article/details/gagyeyzqd.sHtML

[G03] 实例属性
来源：http://baike.fehbvm.com/Article/details/gsiizkpoc.sHtML

Py:   self.name = "x"
来源：http://mobile.fehbvm.com/Article/details/gswtkukva.sHtML

PHP:  public string $name = "x";
来源：http://3g.zdbjq.cn/Article/details/gckintmhp.sHtML

JS:   this.name = "x";
来源：http://baike.fehbvm.com/Article/details/gjtbjklzr.sHtML

TS:   name: string = "x";
来源：http://blog.fehbvm.com/Article/details/gsjsxesua.sHtML

Java: private String name;
来源：http://mobile.zdbjq.cn/Article/details/gwejvivto.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.zdbjq.cn/Article/details/gskkrkfik.sHtML

Ruby: @name = "x"
来源：http://3g.hesvh.cn/Article/details/geeyozylf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.fehbvm.com/Article/details/gdcrzikko.sHtML

[G04] 定义方法
来源：http://www.share.fehbvm.com/Article/details/glbblybjm.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/ggyjggmhe.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gujwqaaly.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gzxdttkoa.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gasvzrlrc.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gutyzwyfs.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gfuyjelrf.sHtML

Ruby: def greet; @name; end
来源：http://3g.hesvh.cn/Article/details/gijmcjjxp.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.hesvh.cn/Article/details/gdfjqtoid.sHtML

[G05] 继承
来源：http://3g.hesvh.cn/Article/details/gyemtqpae.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.fehbvm.com/Article/details/gtrluzlui.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gscgboxfa.sHtML

JS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/ghmlwomyv.sHtML

TS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gdbzkzgai.sHtML

Java: class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/geolqpoos.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fehbvm.com/Article/details/gcwyspsfw.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.fehbvm.com/Article/details/gcwkrkbfv.sHtML

C#:   class Admin : User {}
来源：http://blog.hesvh.cn/Article/details/ghqjnyatx.sHtML

[G06] 重写方法
来源：http://blog.fehbvm.com/Article/details/gytssdrmd.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.hesvh.cn/Article/details/gxpafrxwp.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gbwzemvvx.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/govncbvhg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gzjxdvnzv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gblpxxpcn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.hesvh.cn/Article/details/gccseyjjl.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fehbvm.com/Article/details/glbdcsrqu.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.zdbjq.cn/Article/details/gkmsdkwwm.sHtML

[G07] 调用父类方法
来源：http://blog.zdbjq.cn/Article/details/goeaugbst.sHtML

Py:   super().greet()
来源：http://m.share.zdbjq.cn/Article/details/gezqjbnws.sHtML

PHP:  parent::greet();
来源：http://baike.zdbjq.cn/Article/details/gkcyfaprg.sHtML

JS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/guhyxicux.sHtML

TS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gdqvzwnuz.sHtML

Java: super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gkhjcpjgq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.zdbjq.cn/Article/details/gnndnjowf.sHtML

Ruby: super
来源：http://blog.fehbvm.com/Article/details/gmhqueani.sHtML

C#:   base.Greet();
来源：http://mobile.zdbjq.cn/Article/details/genakocej.sHtML

[G08] 静态方法与属性
来源：http://mobile.hesvh.cn/Article/details/gaorawzut.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.zdbjq.cn/Article/details/gruqvsbet.sHtML

PHP:  public static function f() {}
来源：http://www.blog.hesvh.cn/Article/details/gjuqojxhf.sHtML

JS:   static f() {}
来源：http://mobile.fehbvm.com/Article/details/gtponhsra.sHtML

TS:   static f(): void {}
来源：http://www.share.zdbjq.cn/Article/details/gamrdovuu.sHtML

Java: static void f() {}
来源：http://wap.hesvh.cn/Article/details/geflwywdl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.hesvh.cn/Article/details/gcrwnvlmr.sHtML

Ruby: def self.f; end
来源：http://www.blog.fehbvm.com/Article/details/gddtbrdir.sHtML

C#:   public static void F() {}
来源：http://www.blog.hesvh.cn/Article/details/gkvumjcmg.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.zdbjq.cn/Article/details/gqwsugfzq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fehbvm.com/Article/details/gjhrelpnt.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.zdbjq.cn/Article/details/gcnhvopgd.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.hesvh.cn/Article/details/granlqatj.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fehbvm.com/Article/details/grevknaqu.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.hesvh.cn/Article/details/gcporajcx.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.hesvh.cn/Article/details/ghhaoirzr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fehbvm.com/Article/details/gztzsgbvq.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.hesvh.cn/Article/details/gbimdpxih.sHtML


<!-- 参考信息 -->