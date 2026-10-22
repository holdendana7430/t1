代发 wailian999

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2wlzttqnp.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2tnilvwyv.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2zuovpeve.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2rvzooydl.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2bhxlbqky.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2xvhheiac.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2pqjpjagf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2gepfzzsz.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2semqstgo.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2izeqgwyo.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2gxpxcuid.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gbagpsgr.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2inllmlnk.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2bwgpssfm.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2zhdqxpxn.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2gsjdblja.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ijgtgtds.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2hhgonmeg.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2yeelkhwj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2zbdqnbmw.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2cbqnjrla.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2lhckcwza.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ncdoopdv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2blsbhfxz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2fquokcid.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2koezglzi.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2srvtrtev.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2vkobgenm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2lvgrahbh.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2jcjcuwqo.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2jkeeggbh.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vsdsfezt.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ikynsnll.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vhxepijk.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2iuiyocgz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ccpxqmpm.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2dkodzxol.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2qucnehlf.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2nzqaqnbv.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2rstpyxbi.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2prjpqvmt.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2vebalujq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2gewjgluz.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2hpexhkfi.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2qfevjjmg.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2pscqxdqw.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2cfjbryuz.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2ilknbjwq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2bhwcoedq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xuyfkvky.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vjfwqcpz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2erjifenk.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tccvnlcs.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2euyzocyy.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2yfjlhuxn.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2ctrpidpt.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2eoxmmrmr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2vpfsinsd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2auvaitig.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ukacljqq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2njixxoyt.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2moxcufhk.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2sfmsiptw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2glzidrkk.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2hyydoevh.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2avzxuhwe.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2sgewuufu.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2iolsnfus.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2yjdldupo.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2fxgiwtfq.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nhdsivdh.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2yznxjnsv.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2kcoipzgh.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2agtsjzfy.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2wyragpfr.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2dwukxqpu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2iniwggpv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2uodbpgrj.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2lyxonvgs.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2xsiwhwgr.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2zjeljprv.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2rzsuqqgo.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mosyvqyc.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2ttsnwkmb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2zrkofsrg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ptmkoddl.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gjvojbne.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2itoecrde.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qnehkyps.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2qlmetpso.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2rvtlqcfu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2cmihbgqy.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2qfdcelks.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2pyukdldy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2iqrdqgoa.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2zblrfccn.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2zbcieipm.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ruksfwpu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2qiiwmznr.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ejajcjel.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2levwjwwn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pqnpmzxk.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2szirvdtz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vcyyuhyk.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2azspnzqf.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2nzanthba.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tdypvhqr.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2ohhcppru.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2qpprtsqi.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2rdzqmyuz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2vqvyaqhv.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xfgjjbwo.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rldudcqi.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2xzcggdlo.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2pvfvpeld.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2xwrhzlvj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2smzxrndf.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2rsaflxpw.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2vurddzsb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2kpzcottd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2eqnbstke.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2jsxsizpo.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2onmigmqq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2plkqnymz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2fiwibkse.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2eiguqdhh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2utazcdec.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2gbkiktla.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2igngtkps.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2ezcivwdi.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2cuyiazhz.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2gmukrqmm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2bghvaxil.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2ilewyrvr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ifbbmczn.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vpfeopyf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2agbppxsf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2hqjjcskd.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2srkugyut.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2icmkfwnf.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2qmyemhnk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2nasdmukc.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ghfmuipf.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ojelcheb.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uuccsfqp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2zgcdaajp.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2xcmhlxud.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xfftgflf.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sukvtkok.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2hfghmlqt.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2carzjuvr.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2peujwunk.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ushthbys.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cvjrrdwt.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2vevxqnlq.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2stffhsio.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ysekkuix.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ybsklovf.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2gzhbazlt.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2lhdyltjh.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2axvzvhpq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2kqgjiqsa.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2bziyruug.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2uzbfudgo.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2mxhtlfee.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2cxcwxtxx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2klxkchgb.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2pfxdoxdb.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2gxspncfk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2knutrlak.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2hfjtyeek.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2ozxpeakz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2lekfaitu.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2dbspgwxb.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2gdflexko.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ghhxyjtr.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2xbxcehbq.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gpmnxvqb.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gvfmevvx.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2skpfgaxa.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2tofprtde.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2mpbtzhkx.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2duyvzxor.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mulerkgr.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2zqsrkqjv.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2olaxjsps.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2imlskjcs.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wpdcuxnt.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2epqnaxij.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wreufuuz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2ihtfttbp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pkpituqt.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2azwddsax.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lbtwbqol.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2nnakmxwu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2mjcbxymd.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2wwzrgijt.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qkhhzcou.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ulyhljjo.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2cmdmjkeg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2qmoluhej.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2urvbyfhe.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2siefjhhm.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2gicfospp.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2iezuhify.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2iutellcl.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2jpzvrpbt.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2lsvahecl.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2gfqhibps.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2ivhrlufv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2ycpxlwcd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2lsoabbia.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ftkybbhr.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2phgfxtqh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zrbmromg.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2okrqvogy.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2renuboms.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2eortjzmv.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2cueqzyuu.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2qpzsnquc.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2fxxwipjn.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2aakbwhvg.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2eufqjujn.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2zyfqtzxo.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2upbnuoer.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2wqtbxgxj.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2oawdiquo.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2abelfyam.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kpdpyavq.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2xtmgdjmu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2fosrgouk.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2tpbswpgm.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2blbaqnti.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2wnlcrttz.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2sipyjbcb.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2virdurmk.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2slzyaxls.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2nfdlzior.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2hfevqjfk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2rdstznww.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2oyiyxxfb.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2brycnlid.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2nvstjsdn.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2dzjqkxil.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2skgadetf.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2lieuoddv.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2uhplvdxl.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2tidfaibs.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2yyksnitk.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2epozhygu.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2touiduyd.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2vxmddhpe.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2fvmnongv.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ghjrpaqi.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2prvszyxu.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2iaopzrgk.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nuxeeyxj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2xwfhqdol.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2xxudqlbw.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2kgufjgrs.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2tydxaami.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2lfhktqde.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2nvpprflm.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2kqdynfct.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zlhimvpz.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gupyxjbz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2zzgvncif.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2uqaeavvl.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2hogsmfhj.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2kofmckty.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2xvpxqdvf.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2omzivagt.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2sopchogm.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2drthetgu.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2dbofuxdv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2fthuycnf.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2hxrnmnuw.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2iotnifjp.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2kcictolk.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2jbkrstva.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2utihypsq.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2urabslmg.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2eiwvejqf.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2yzndhdwq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2abhsqbws.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2crgsswxr.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2rutbifrc.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2zfkjuzbz.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2ejhewwxf.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2uevprcvt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2usbnjbxl.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2uqkjlbem.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2wxskccvw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2fejrfebq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2fiwaddko.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hzweffad.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2cglshqtd.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2ajtrvvkq.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2cuoauqoo.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2yywvswls.html


<!-- 参考信息 -->