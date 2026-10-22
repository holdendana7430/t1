代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2fuflsjwz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2zqzhfwrw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2wmygicvw.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2wckbtpga.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2zmjajyol.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2papkveqq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ohstbqat.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2svngzpyo.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2lpcbpqqt.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2brahxdkm.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2sjakyyin.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2fgqfpomy.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2rlhikayf.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2frmmguxw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2aukemeha.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2fzthypjn.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2rcgqdoft.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2vlqnawql.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2tawiydvw.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2mlguxgba.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2rutyfpzb.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2marjzxfj.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2yywnpoxv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2txqylojf.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2usdiemth.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2aarfymfu.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2iayxmebq.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bzniwtmu.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2aoamfehy.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2gepcwfrd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2wpqazagu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2qtbqgdcg.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2yznqigce.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2bpixxios.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2iqpzicqp.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2oinwmuvx.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2pcttiqhx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2fmuejzom.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2uvbdsusz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2bfhysaho.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2wweplzvh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2inrosjyh.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2rdicfdez.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2wlgyrsou.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2hzxhxjck.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2ngpbtoxx.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2clgafkfq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2hsodcffp.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2dlkmkrvl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2cxwjzxwg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2mzenaitz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lspzwavr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2tqebqink.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2txpauesi.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2aoeqehmo.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2qvgufaau.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2scntldtp.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2yyoxgswx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2dfaxjrro.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2tiouesrg.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2zcwwmlfl.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2cuhewdob.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2ivbquuju.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2wrpuzabs.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2kufpqayy.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2xgnxxbjx.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uhecqhlf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2mdcwsjzl.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vrxchkmz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2uaxrcmao.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ojhifxbp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2dkkkbfod.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2dlnokkgj.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2fembnzce.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2jczkgwup.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ypcqwsoo.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2hypaapep.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2foqzapto.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2jycucccn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2kuknkkam.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2srezdwrl.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2clmmxzeg.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2rrefdixp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ysuypjwt.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2sifficst.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2fvsblrhr.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ivhvjlkj.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2vvzrtwhs.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2cyzxsjbx.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2fifddjnl.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2oqgxtboz.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2fzowmqtm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2ainhwpey.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2jhwvkizl.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2vixdgdfo.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ybskkqzj.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2zzmmegyy.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2bepoqseq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ilhlnsvw.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2dmemqfqy.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2hgiumywa.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2bvbsqnkc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2eqeoxjvf.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ntjunkto.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2hdmpyhvh.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2wwommnih.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2uhtfnery.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2hgwhljor.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2xngrejiw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ciirlbgv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2mvnbnnyw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2vicequyp.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2lyvbpcvj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ltwajwox.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2hveuabnl.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2omfhslrc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2hqfekzgw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wvecware.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2cbhbudza.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jufxbise.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2vsrshgop.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2exoaifzg.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2odwkhnvd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2rhqkkcoa.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2uksnefpt.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2vophmkcm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2ormkcpye.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2trnvmfqw.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2uturmcna.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2pstnkooi.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2fytdrxzw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2hfljoeao.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tkomlkcp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2miylysge.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2uvsywcal.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2nicqjgnk.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2tolngjll.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2wjkmojnn.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2drtwgzjv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2cvrzzzux.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2ujhzyyuu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ejxxtiqi.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2jkqsweyf.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2tdfgfumd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2ozovfskm.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2hpixgrql.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2gfrdmcmu.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2vcneygtq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2praqqtxk.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2tfsjykqv.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2yheplwsk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2dgldgdtz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2knzctpoi.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zqkngxyg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2hehkuwbm.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2kmadgsgl.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2mizpfxfq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2tmkvvvrl.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cfnskqqy.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wohihvxv.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ulzsyuqn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2yjubyfdz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2jkvzbtno.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pqsvcizi.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dijauhrk.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2swscafwu.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wtqqqzdv.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2drsfdrfj.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2umjyfcdt.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mwwczwqj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2cvdvajcc.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2guhhtscu.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xrzvdkaa.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dhujtdqw.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2krtfpsqy.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2kfkrqumi.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2washaucd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2airhtsyv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2carvglee.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2vvprtovm.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2fwonfezj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2bxtmdtsv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2eaqwmcid.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2mqeogmwn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2xkuonpgy.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2ghrcubwz.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2iddrncrw.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2urrqjnjc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2areshhxv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2gvsbvhsw.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2bntqbmle.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2pyhhfilc.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2wpwanolk.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2alkrtwlm.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vgffxqmz.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2kceggipu.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2dfnwynhl.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2uszqebki.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2jojrkrte.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zmqfevbd.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2yuivrgdy.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2bnsnlfol.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pcekancm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rvbfvvii.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qkhpwyff.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ufpxifny.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2dewnsbbs.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qqlyrsnf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mavwyfrz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xpklqewx.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2fzyggvkp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2chzezrmj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2owfbmgdv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2jkyhktoe.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2prqedeay.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2fgrtrlvn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2pzgticwk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iicrfrbl.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2mcfimxan.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2nkidpwuw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2ifidfpbk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2ncrzmjof.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2xzdtheta.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2huhxmvwx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2nduynjjz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2trpsjrba.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2unqpvxkd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2bqiiiqyz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zehdpydo.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2ahfnglav.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lqlqzjmz.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2wyoozzrj.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2scnyydah.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xfnxcnii.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lzfkjhfh.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2ghqwhigl.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2gxitlloi.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2wpdpisrn.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2bbkldlgs.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qopaaqrs.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2dlieqnut.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2nrnnswxz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2loermebe.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2qrdragki.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ssjttepp.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2llswcvlx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2beccvddb.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2eibjfzhs.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ydlxdcjh.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2jqmrpkdx.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2snsmokqu.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2fkxxnaag.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2oubapcex.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2dupriarn.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2ygmojfyj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2dqnvvwat.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2vtwnkhfq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2rlidtyul.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2eppnrqbb.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2xpczgxhf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2kkhaxpns.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qtbambyv.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ohnzqxwn.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2somirewa.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2eqwjzrxy.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2awntysiw.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2xxgdzbzl.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2wlcmlabm.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ccvaqkga.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2wkrpemot.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2wknjhwcc.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mfqxbzqu.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2rjxzkkch.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2ebjzrxxq.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2uzzjdtva.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2gimxsesg.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2qazkfutt.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2lruzlhlc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qrjkdnpf.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oifkkfuw.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nvpamhic.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2azuoffij.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2nnzndaou.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2swemtswz.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2dsczcwla.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2fjjgcqcn.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2ametfjmy.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2cbwljrer.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2zvgrqtgk.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2mswdmmss.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ucqshgyf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2femohctn.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2jwxmktvd.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2bzkuhtdy.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2nncbizas.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2zmfpjzyy.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2jzmikksb.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2zkuozufl.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2nmbxdjzp.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2xjmewmej.html


<!-- 参考信息 -->