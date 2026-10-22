代发 wailian999

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2qqluubmv.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2vmgvwbbu.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2awwckwgm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2mrqxlvqr.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2skiodkao.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2klajawqi.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2zviywklk.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2rjpxhlnq.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2crlooyih.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2vipldxvb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2kmpyptvu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ikfkafhi.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ukctibpp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2krjvahyl.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2tyeolysa.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2yfjbxsmj.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2vjtclvnm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2oatnfrjj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2skvobwge.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2xbxeomxi.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bxphmlfh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2xfsfbior.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2uhksmzfh.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2brzpzxtc.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ngnzljgi.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2hfgkxitj.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2zhmorusl.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2thwhtgau.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2admddctu.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2hjxliuay.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2bzxzkvys.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2jpblzeau.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2qnyeutmx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hkzbvrfp.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2zozptlpt.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2pxpoyady.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2kwjvblqv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2zofotauo.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2mctkoquy.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2hrokkldw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2ihawhlxk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ucrjtqnk.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2xrrajrmc.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2yfjpztri.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2hcsrnijg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2wufdkkwq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2xwqqxjdt.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2aglvjbes.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pacjoihf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2suauayim.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2liswqnun.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2lmwjwtua.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2ofiybvfl.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2pbpinawc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2xsajqqhb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2phsbocxv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2uxrkdeme.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2mmndaqjh.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2spxylyhd.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2ntxgchyg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2nkkhdons.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2mrvqebbx.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2meuteade.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ochypawz.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2tzbbitvr.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2jvdmuxtx.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2lgmbabuh.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2fhtngdpn.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2ybtwvzgs.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2eafjzkap.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2wbucerxk.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2lelpxfqy.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2wrjddhqk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2pkyjxzuv.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2lsnyofqu.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xxbyxnpd.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2pzycnqgo.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2lhicjaha.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2fbditktt.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2wskbvetf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2pnjffmbi.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2citfqzad.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2wubxgvhq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2lcfcckpb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2fdugbjcn.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2hhbkdrus.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2bfjrmfjd.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2hiufyyxv.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2gpxrjzmb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lycttkjp.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2hwbiaapt.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2grzffeld.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xdoqcjex.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ogqqdtkk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2wnmijvzu.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ipbwhxwz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2mulflvqo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wljeyavq.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2bsdhpikm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zywxhhhz.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2qzdtbzbp.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2ineararu.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2owyxbcja.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2ugkhyjbf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2glaxikcg.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2floyeyve.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2dinyxibz.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aqhehkre.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nkxicocr.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2xecylizi.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2iodkfgmr.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2bzmwusjh.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2vytrvnhs.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ulzruuwx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2bhtgkwsm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2pliecrim.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2ycprakmz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2ghlcysah.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2aogxipgt.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2vrfsrsrr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2nponzeuj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2vkpdfdse.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2fdpvdgds.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2nvtuqqon.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2xlirswum.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2irsoijnq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2nnmlkbtw.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2kgoeowgj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2pmvwuwsb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2idaqlltq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wtfibmbh.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mnflfecd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2ltniehil.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2cycfvyqa.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2xcsvkiqi.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2ijnyyhwa.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2uyubecvf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2pgrdawai.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kwwmipjy.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yqystrzp.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xnkzmoqw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2etfyfqpd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2sxwukdhe.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lebaucoo.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qkcuuqhi.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2hjjacprj.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uuunkfyy.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2eqzwxrnn.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qzdqzdaj.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gbprvath.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2izgiwszc.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2muqsobfo.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2udpdzllw.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rdsxupka.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2mghlfdaf.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2yviewnlx.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2hzjqybwp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2wjdaozmu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2kvohnoeo.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2ecivjdbg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2aglaxoxw.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2otzbgrlx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2epiaeflx.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2ougqbglu.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2ljlrfzgo.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2lhbdolxj.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2chroslmh.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2bwyqwode.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2asyxszfx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2zvvphidj.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ydhhkomc.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vdpylyxb.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2lggsygco.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vdmnqclw.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uhtdxgdo.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2gmiddzxi.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2rwvgfepm.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2akcucqmo.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2quxgyvvy.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mgbhmjrn.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2gotvjnrp.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2crfyeaxy.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zqsqtbyl.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yjqadahg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yqgeujbz.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bepytrlx.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2verbvmal.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vtuduowg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gckdnszq.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ewctaqat.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2elyrevcp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2taszucys.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2ixpzvoev.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lzxhxvcw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ugecgdrp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2henwmrvq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2hpinhyey.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2odheesax.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2fwwccasv.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2rskzknbg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2hefcyqqd.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2lmqlbswn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2vaxgqkat.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2twqotptr.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2fozqcuxu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2ktecobpx.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2euqhnyjw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2eqmzeflf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2njzdcvur.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2kmicvkxn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iaopoisp.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2sfhaevid.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2xbvztncc.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gpnkozxx.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ixovoguv.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2aeqomldy.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2okoqvent.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2iombkboj.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2cexkofoc.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bgnzszmc.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2nuuvqwgj.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2utgusgaz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wpzyjsez.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2lrohcqrs.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2ehetwzms.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hfkpxecn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2xlwwybka.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2rrizsttq.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tylkdwos.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2eviehsqs.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2tojbwubx.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2oipmglvc.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2grxcddob.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ucjveqhm.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2ktimdfij.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2gsoerxoz.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2omhywqlq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2onjdnblp.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2fzwlsdws.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2yruhrgda.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2fdsabfsy.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qpqikdck.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ljpsqkxq.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zifkztdx.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ykevfahx.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2nagvapsl.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2inkakswk.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2smdnxkzb.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2nnposuro.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ltgyqfki.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vppufcwg.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2fgxlyyir.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wevrysmp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2cfpmrpjh.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2dhdffaws.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2dsjvcesn.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2khaogtke.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2cluqmukg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2cmwkkyle.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2esdgjepg.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zgreiflo.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2iswyeypw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2mxjshvaj.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2ztaltgdy.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2uibiuogd.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2gvdmlgns.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2sjlnkfbn.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2bxdqopkt.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ytiqwakw.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2bhbicolg.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2figaxgyf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2abjmevzh.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2zlfxizyf.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2uhwentbj.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2pfisoccc.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2dzsnchrs.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2afutukwo.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2rrzxvdgf.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2cdbbfwaa.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2aqqrryaa.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2wporasec.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2hufypaal.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2flbywshx.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2iqvcyfcb.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2vmeskcou.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2zplalqsl.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2oxyqeggs.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2glswjhdb.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kvtnxfwg.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2iffpvsrv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2neshdboe.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uwptydnr.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2xscfksku.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2rarqddzj.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2kuvgwkyv.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2fthqoumt.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2szxhupsp.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2yqhzmjms.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2ttwsrwvz.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2jcfdhbyp.html


<!-- 参考信息 -->