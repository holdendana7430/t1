代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3epscdoxn.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3cwojbqwg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3leoagwnz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ljyahffj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3snbdwqlk.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3pqgcmztt.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3feboxxkx.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rwtqqhix.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3rntgnqxk.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3eundzpgz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3cgmxsdzt.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3hjrenfwv.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ulvirqdo.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3wrbpvamj.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3xphjirna.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3nszxyukm.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3jiispakj.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3paditxtd.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3agmrqzcb.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3jiwemrda.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3chrsazls.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ioespzig.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3osubbkzz.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3udeppmdy.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3pgkvqpap.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3kuytuzfs.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3mblhqfoy.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3xyucsghw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3wlafimxt.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3emkkjdaw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3xiohewis.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3rudaaswy.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3hqkkfxef.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3htudzhuj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mruzshhr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3tiepbsel.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mkilkkem.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3jwmonqla.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3ajwejapj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3lggckuwm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3wshbnxun.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3pqbbvueb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qlhelfyk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wjapfirf.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qzmzijno.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3skecajch.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3hqwlnxlx.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3eowpthfq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3rikhoxrj.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3vigxjgjl.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3fdslrvwd.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3krdftewe.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3uxmxgqkw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3zywfbbpu.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3okclkyzr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3icocssyv.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3bbxgbmvp.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3bvxmsttk.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3jkxqeulx.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3rmwiekga.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3uivpvmps.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3uawndazn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rasnxvel.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dxkzetxr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3strwvmky.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3oygdzgtm.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3xftssjqn.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3goblbvaz.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3atpryqaw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3lqfzvnpl.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3jmvnypbj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ottjigyq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3vvnvxgoi.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3qtiavotn.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3moqpvisd.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3reordles.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3kaxxdoda.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3nznfajqw.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3uwxkrkxe.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3nhecaczt.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3iclchmoi.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3npzqhwqv.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3nheafqdz.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3khxchexu.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3fwdjzfgu.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3omilhydg.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3jehowajn.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3whjqxeoc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3hblyylse.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3moqsbzix.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3jhxcwdmi.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ozwllnhs.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3uxgzlsmh.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3rwflvncf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cxkihwys.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3pppchkcy.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3sntxgjmd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3qqpbpibv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3vxhkgffy.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3orlmovee.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3fypqstbo.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3zsxjcbmz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3feydyahv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3bchbkiev.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3fhjokztc.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3arkhpiov.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3afczqrmt.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3znefidmp.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3dtpupqxm.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3qnkwwvip.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3asgpggbx.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3unxlnegi.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3zywrginz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oszwuevh.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3xoqsuzby.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kukcrntx.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3hotkmxch.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3xljaqiix.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ttohkesy.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3rkaxkuvy.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3icljnjsm.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3jiwbfiap.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3analllax.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cydonynx.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hgxefmzy.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3kfdensno.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3ziccmqxx.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ehowvwhm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3zziebawa.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3teaytalx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3hbclkjkb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3syuuplvc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3zlapkwpz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3xflkdxqq.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3ccbgdpqn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3tstyyvej.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3lkehptvd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3jdgksmrx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3mscfnzya.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3mlvodfaw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3zjmetfmw.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3vwjdvtls.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3xdggxdij.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3mxkuhhgi.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3mdhipcdj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3nljsolgk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3znqkayho.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3eotwbyhy.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3sbymsqsz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3sfqgoylj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3ldtqbtcx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3farwiwsg.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3ciydhqpw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3kuwlwuew.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ygqwmbqj.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zudbfqsh.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ejywqtds.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3fvolzaxn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3upxnowuo.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iklcvnyz.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uwsvrgeu.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3hhwsbdej.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rzcdxmyd.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zdepwtdl.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hyyhcgrv.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nkkoiveh.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3nxampfek.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3riyjlozu.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jjkjbxlb.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dzapvxfx.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3rhmjyqhy.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3gtmdydwr.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3xqurptsn.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3sqowksrk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3wtwmzpxh.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3ngftvuit.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3rhusowrc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3wkmyruru.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3hjbralej.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3lribgogd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3eityqsiz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3vptmiyos.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3pfywdycw.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ffgmdoyv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3gskrfqgz.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vdvfwvrz.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3kgpowpfz.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3bspzbqxb.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3kdnaanxo.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jeoufhtr.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lwninlfj.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3tshojexv.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3gunebhfh.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3nimiqkjp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3wgvyvzvc.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vzeevbbw.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3sxzuzioe.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3nwbzasix.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3todmhnqp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jtqfzwcj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ubypqggj.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lqntmiwh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3eqjgghhf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3etclglxl.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3otmvchdg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xgpootip.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3gpwsceax.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lxrrfesm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ynuwpyuv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yiifeyqn.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zvzsylyf.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3sofrqslv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3vbnouzrd.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wvewtfwr.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3xtvydrwn.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3eetsmluj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3otlgdufh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3dwtobtpb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3dtqxmhhw.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3cnefnzcv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3aaovcrho.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3nmctmafk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3ttsjnuje.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3fayjuugg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vynrgopy.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3efggvsgj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kywdnjoh.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3idkzunik.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3xkkndqmw.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3cbgbxkxp.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kvvnfhwu.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3lzsnxoys.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3erccicdd.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3kiwlgyjf.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3pgfoegtb.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3zfvxejlx.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3eevxyjnk.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3hdbybous.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dduzyich.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3nwnpmsqa.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ovhxeonh.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3umymfwza.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3fgulxiag.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3llihisvs.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qkzhqgjr.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3fhoyvzia.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3lpsgvjlk.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3fnwodhqf.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ikfmvamf.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3krnauqgl.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3imflnjuu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3uuevheks.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3vcsdsxbt.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3voynrkzl.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3ehyimpwr.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3yhlhizeh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aapgghml.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dtzlaglq.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mpuzdfsr.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bzrtmbev.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3rpqrgqdy.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3xxquxutd.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3lehtajni.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3kaxkqfia.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3bsmfwuia.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3evhqpype.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3jsjnopel.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3doaefzzb.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cfhixzgp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3yujkppfz.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3qwcfdvwr.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3ctatdtat.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3djuksdak.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3fcubgeul.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iyjtiifz.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xxznrylf.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qzdxusgv.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lhwbsdwh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3obvcydyo.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3rdjtdvcw.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3okgmzgxv.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3bmlrzkbx.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3pbidxnnx.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3odhmxihk.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zhdrwnce.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3kkfrssbk.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3urncsbsa.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3ymgwjsnt.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3jkhenzvn.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3njpnrieq.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3oqdzbiot.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3efvzfdqz.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3cydmavdn.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3tqcchxcc.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3hlzklypd.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3vqiqlktk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3kafrzcpa.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3idrfyqek.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3pkhfkasg.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3qmnavuzo.html


<!-- 参考信息 -->