代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2nhvpjkrf.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2jtwapvwt.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2hctjjpzf.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2knntymfj.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2aexstcsj.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2iookvqzl.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2gjrpjqfr.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2quinjwaj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2ikdbmeax.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2orgnikla.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2zdgqzggz.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2orsobgnb.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2opmtwlew.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2wvbxatlk.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2amgrrcel.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2jfkiykyv.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2hmsswjpx.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2yxzkyfcc.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2svubgkmx.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2fvjxwguh.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2mdrhcrxy.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2hvfkpzjd.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2ikzmzdug.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2sgjtzmrl.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2pytmgaev.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2wtppatja.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2opogaepc.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mzciveds.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2cudxtoik.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2hvcamzar.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2jdvogncc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2vkmbzobr.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2xidlpffj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vwfxclpo.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2oeshwezu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ikdgyhbi.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2mrcxnnxy.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2pvbtmfkr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2htewgiij.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2rgfpqewa.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2lsfmrqor.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2hayurugo.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2cretdsbx.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2slzavlnq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2mlbhvtbe.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2szemoltf.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2twyynwwa.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2nwbkmebt.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fiprvkuv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2hkhdokzz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2myzqpjhq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2mdttpjvt.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pxiijamc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2kldklygr.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2mbnkenzw.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2nmbwcvus.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2bmzqculq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2rnoziphm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2hajfkuoh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2cnbatxhn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2knxwjpzg.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2eezlxnyy.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2zrqzjuxr.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2ardcmxtv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2figsvlzt.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2sdgavkxe.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wqzspmeg.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lmcxtfwv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2dwsowdde.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2ydwaluxu.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2ghjjpakn.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2ajhflkjm.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2tyaoumvh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2hhmfgaey.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2iahhflma.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2slqtpfrw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2mchdhxet.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2pztaskuc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2nxcvejrk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2nusydtay.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2nnqugsta.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2aapeotsl.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2afpwoxef.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mxbkurlf.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2yszwkntu.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2ubuxbbbo.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rppraqzg.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2fbreodwg.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2fmziykoa.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2vonqrwlp.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2delhxjoi.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2risgdkgj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2xfbqlewm.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hlgkkgin.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2qsebfqfq.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2skqrhnfz.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2efasojvt.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2caxqifgz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2bjpoodfe.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2tgwcuycf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2unhtacfj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2qiczewie.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2uksbhjjg.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nymyonvr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2qdwhqqky.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2rrhofuap.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2nfscugyv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2eykhniiv.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2yfezrluj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bqedgclx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2jcjwtkkx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2tumqdgjl.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2uxfikkvf.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2bwgoefdd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2xmnvrwbz.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2lqkpspiv.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2hsmmjini.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mjuttfjy.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2btofutnx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2chunruyr.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2hxyyizkn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2dckcuezn.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xcqmjoxh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2cufsmgrs.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2fnhwmotk.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2vvvqrqyf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2lnipvzkv.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uqkxhfxw.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mteiawql.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2jiaminnx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2rnjwifsk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2bfihaxxq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ddunyxcj.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uyrwgsps.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2bjvdiyxk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2sbptnyvq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2rtqzcycn.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2gxecjdyc.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2obatednx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ghlclnrk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2zjnbzrxe.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2itvfrhjj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ommsazbi.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2bglvsbao.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2nzuueegq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ohywmpnq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2wstyjxyf.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2kxpvfrmr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zadzduxh.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2wmaygnyr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2mvezuxzf.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2eynonxly.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2nyyighfe.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2gyhkgepy.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2xktqnrlm.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2xsuuoocb.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2bjkbnzyc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2fzplbutt.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hjvehjce.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vtaipbkh.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ugwhzpyq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2fsgczeqj.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2oqufqsby.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oqutjohf.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wctaajcm.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2fkyajoaa.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uzabhphi.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2moaxwoez.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qeyxuvyq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ehsfjlxe.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2rljbtsdt.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dnbqznbr.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pcxvinau.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vphpznfx.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2jsgslyla.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2yidedfua.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ugocijgw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2jrebmizd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2uzxkwlyt.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2uktfkygh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2jhpxfiev.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2ueyrogue.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2zujhfawu.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2oknwocuj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2zeyzxiqp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2ktvxdjjd.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2zdphpyyn.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2tojbsain.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2qqhkzqno.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2mimiidza.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2pfjdskkj.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2nvlxbofo.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2upuvveax.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zlbglsnd.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2efsrqabr.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2nduczfwv.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2rycswmlw.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2vqpjbhcw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2akjoipkn.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rvrqrwpj.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2bcctuvtd.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2lkfjrbyq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hojylzqi.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2amyshyoi.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fmteljpx.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xtwnfymz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2cmqpylsf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2adqhtmkc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nbtoodsa.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tjtljhxi.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2dcheaoih.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2epbfyzoe.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2mqhpejso.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2dddtahhv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fzqjkrwt.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2dddbcdxn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2ajrbjald.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cvdfxyml.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2ghswyhgo.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2tagfbeqq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2pxqfzjqe.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2jbcsahfp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2omtoxxvz.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2mapkuwsh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2hutbpagp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2xdhybmde.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2lrraaioj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2oozbvuks.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zkfffosv.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2hyublzby.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kamxgnhe.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2yqllnfiy.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2vdeexqnc.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2atzrnrqh.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2tcnhgflx.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2igulfoft.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2kmdusoki.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2ulavlakt.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2ygeuejnn.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dlnoiixk.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2wxowoqvh.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2fzonpnbo.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2xkgrbwyc.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2tuecbodi.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2monvepxa.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2zfkeqmhr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2eqhfirva.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2diezmdsl.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2muzvlbjt.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2vavwhbrs.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2omxdfucl.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2zqybhdgj.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2lashthsy.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2heyqtvil.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2dqdcwqrd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2qtftbmvw.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ltcruvez.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2dbhvfcwq.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2sdoyyevf.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2fanjpbuj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qxwmazty.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xnucreyr.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2juczzimj.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dwmcpbiy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2agknsldp.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2vbbiaxgy.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2rjugqekm.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2hkawxrov.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2euhcfnrq.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2plrkojrm.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ceeorqch.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2xbyibowg.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2uafgcpxp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2jdvfeppu.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2uprdedlt.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fnctzawz.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2xnlnvkib.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2uftxtizt.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2fvaxitam.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wqayvhmo.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ajwxgpqj.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yntznmxc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2vaqkrpmd.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2hrzepsuv.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2wquqivyw.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2vbnhwvif.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2xrilnwwg.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2bcdfdhst.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2muvrpnmf.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2nppxdpdv.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2hlzmghqy.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2lgdncuuf.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2vfjfpcrf.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ksskypsp.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2yvgeigrm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2vrjsmpaj.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2mvweuajg.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xqwtytop.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2gspgybqq.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2kuiutdve.html


<!-- 参考信息 -->