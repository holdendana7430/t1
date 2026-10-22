代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2doqzbeop.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2qrwxywuy.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2dmesjvfc.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dvnrivya.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2vigowrrq.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2zzcoflwm.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2dwanfnrm.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2pcvygblp.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2tshvjmbz.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2sajrxewr.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2exdpxmqy.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2dberfzwd.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2epvzyghr.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2iafnhyle.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2lkkzrehf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2opvzbkhx.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2defcygiy.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2brcuwkdn.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2rnhpvvsc.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2nsjqcapa.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2omkzqbpd.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2wdoqjivl.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2phixtrik.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2gjssjgzn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2znzunjvd.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pzuvxyut.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2kskskgoq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2anvaedra.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2dmxobhzp.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2avfkrwjg.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2ehpgcjyr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2ywyzealz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2bynfirml.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2nupbjsvr.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2wusywigp.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2hpejngai.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2arztlxam.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2crctirkj.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2famnhxea.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2yfebrzou.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kfvcejby.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2kkjpzvbe.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2ypfznggt.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iusonirk.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uzwohbrv.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ypjbccft.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2xfcrtgvg.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2gzgunrln.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2mokjxgkq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2bjrfwhqw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2lydwetsw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2cmkhtsmj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2wqqrewpw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2pvvcqtaa.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2anckxyuo.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2icganjoi.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2dqmktdyw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2cdoqvdbn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2nfdezteo.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gbkrwxcc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2cdbnnxme.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2hwyuqpgy.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2dynbrfzp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2aweviljh.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2jlpqlazy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2fneowwad.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2spsmoroq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2dhnknbth.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2xrkzfnoq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2rgerhnfq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2melwqymn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2kfiiirya.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2avdahpui.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2ahjomlxo.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2ohsnkgqk.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2yfehiczf.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2bcnqjlis.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2eunlxtfp.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2aiviipod.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2kqmmgwrp.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2fhanzgpu.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2tqzkobkq.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2ylmlbvgi.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2txxzktbb.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2zpqvfoet.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2kvgpgstr.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2mxviheab.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2nydvzoae.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2peqjhsps.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2tsdfnlwu.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zclorjym.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2cbrxtjkk.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2hayejtpk.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2kedswyvi.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2xizzuzrw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2zsqhfkqj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2zfzxtyqc.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2mlessjmg.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vkmixgpc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2mpikurxy.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2hbfbpots.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2vcpxmhiu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2gpmcduzr.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2pcnjbsti.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ctefwsea.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2jpjzyriu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2lhhzgwkg.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2iqcylkut.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2bndegtax.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2benrwshu.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2mdfmgvoz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xxtkcuup.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2dgjfgsla.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2brvbtmho.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2djuotebi.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2cnsvgspl.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2aajbndcb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2govsvsmx.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2nyiuokjx.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gxdlvshy.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jdaocfsa.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2fswuinuf.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2nicvjblr.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2xbqmrvxy.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2twtqbjqv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vengolsm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2bgfilmri.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2rnbvzyii.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2juectfqi.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2fncwjyhb.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2meooizer.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2lhuaxblt.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2chkyuwxk.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2rtqdqwxb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2afliovjy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2xcdvuuth.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2cbocwcyx.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2uamftbop.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2vktkmksg.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2urpsazlh.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2daxzgxzn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2kbrxxvue.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2sowdzwck.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2axvjxqpa.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2ehcsmado.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2jlsgnuhz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2annyxbvy.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2ibkqyxfs.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2yqrjgrpr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2rlqmnzql.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2uufhhfim.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gxqmhbfz.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xeqcmutm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2estcaurg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2vkonhxhh.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2olswzzme.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ftncqgcr.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2mueybvaa.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xaehbkzo.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ctdndccx.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kgwypxqb.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vumhaffg.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2kzmirkcp.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xahbxlmc.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lnikxdae.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2odcujsni.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2iywyorbs.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2afcchehz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2bqzrhtgs.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2fexvqsrw.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2rdrpdjpm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2czzoccss.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2karysgno.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2dhhjakaw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2cmboawwf.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2uhjohrou.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2bqnouqdr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2joeyfviu.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hgawifwr.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2mvidcnej.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2wpefqvtp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2euutwomx.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2croknili.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2vmndohcd.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2gsltiqqp.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ikhartui.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hgiqrhff.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2fykwkurh.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2onxhoonu.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2wwyxjxxm.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2nkotimii.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2plijhyey.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2muejiond.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2fvfzrkcn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2thpyittd.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2otdjoqnv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ddzulslc.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dbcirbeg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2hekqmnik.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rclljzgx.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2irtoksey.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ljmfcksy.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2onahrjjc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nkoivmny.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2efwsbgxt.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jwcxzxcz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2lpgbnvcu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2aessmbgu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2mvspkgeb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ybreqcay.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2hmbwxmfm.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2afvfntng.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2dsjoqkcp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2owzzdvvx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2hfyzkqhe.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2jwqbghyo.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2kaqgtezc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2rsmgvcul.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2mwznycjb.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2cdqhvkak.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hvplxxft.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2iiaqawiw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jbuumdul.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2sezcqrzx.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2xycfnvco.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2daocxbnj.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2iyojhgaj.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2haxdnzfi.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2wlydsqhg.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2mjmkdqne.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ohzjskqs.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2dkufhmte.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2rwahjnjx.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2djschsft.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rziacuvm.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oklgqczp.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2crhjjsjf.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dffmxxiu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2actlnhmv.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2xchkqnjw.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2evydgjgu.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2lzcbbtuo.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2swjgnioc.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2pjnnqhlh.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2boztiwte.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2dzkuxnkv.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2vpoephbl.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2lcsfhamo.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2dwnixltb.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ixxjgpts.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2rldmkaoe.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2dalvlgaf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2offblrel.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gvtnvtpp.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2savsgtqg.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2rojaxzyr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ooumttjy.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2doaqixbj.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2udkjskvq.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2legkbusn.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2aeqhupaq.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xlikquow.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2wzojvhsn.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2mpchigxb.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2wwllbigy.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2vdmfyzgl.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2yxvbczcy.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2krqtivse.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2luvyqoqw.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2lxucscel.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nnoieaaq.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2iccainzc.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2efveetfc.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xvsbbqwa.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2memciqon.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2zsftohpg.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2nijrbtoi.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2jbczgkki.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2sxektcuw.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2itoezieb.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gbtyqewc.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vwnoztsd.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2noastzjp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2rbdqdyhi.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2hfyhmdlh.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rygvtulj.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2xsdgpskc.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2vsmcyena.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2cighspqn.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2hytifotg.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2hwhovote.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2lewdsxds.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2egusqzdy.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2mtjbrpmt.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2akkeiueu.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2hkpfsvlt.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2qjgwxysq.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2urbkmndj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2fjqjtnrz.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2ydlzvgjq.html


<!-- 参考信息 -->