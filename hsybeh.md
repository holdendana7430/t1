代发 wailian999

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2liapfhdo.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2tinzfger.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2qbcttxlk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2qffkfucc.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2uildklcq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2ktffcuvj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2cdqydbgn.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2wylsuixl.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2nchivjax.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2tgrtfwqu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2oektwyzb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2ejbgynrp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uqwqfktm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2cptwwdta.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2atnnijxo.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2rbpfbvdp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2gkriestt.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2cuznywqd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2pzjpwblv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2gmjgkqtx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qunglwda.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2nwdekvzw.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2buhjlovc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2slxewgfa.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2vnicrmcp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ncrhxlqj.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2lcbdcrcl.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2oyzhrecx.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2hmydhhca.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ijahufjk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2xysebbgy.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2eefekidi.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2awayjvmw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2mmoucxqg.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2pmlgdrtv.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2sgxldgre.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2yjflyacv.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2baephbmk.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2eevjzgvm.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rragbbcg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2hqjzqbun.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2vbucvfbk.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2oubwzlay.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2zxcgybcb.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2zzdzpxba.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2auktoirt.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2spostagu.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2cimzkaov.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2gvsdakun.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2dmmrrash.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2mtjjpvle.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2jrjtqenj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2dfselxhd.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2irottryy.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2dgasakuz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2wcxypdhi.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2kkzuypux.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2gecswurp.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2yjkljwvk.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qnzkefqb.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2yhrrdgnk.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2yhssqtpa.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2qlrzwtby.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2akfwhefz.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2qorhoaik.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dwpxkicu.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2nmuigtaa.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wutcjill.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2yeydrgvr.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2avyftpvt.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xjaublbd.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2qqedgrob.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2dgqbhhoi.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2euaslynq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2wvkyuujy.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2malwxqbx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xueacrgp.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2jbitvvqz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2werakzrz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2iacixvwg.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2wceztgsa.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2zxwzfzau.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2xoragpqz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2nxephqoa.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ryqctffk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2dpvklwkx.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2amzrinhd.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2habtafsi.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2lcqmekgv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ivxyjmfe.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2kmxscewf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2malheuri.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2yexyxwph.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2sajpvrwb.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2keccweje.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2nwgrhkyx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2njihcpod.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2gbmsiweq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2euvqxqao.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mbovpfgt.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ozblvrmz.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2jbcgebop.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2mmojcabs.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2daswqaqm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nwjgrsqg.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2sbhzrvkb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2caiqfqax.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2ozafzddo.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2joygjdsw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2tunzdtpc.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2opsfwobj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2wrcuptfr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2lrbtkgnw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2wlpygftj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2jgbnqkaq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2zxjvvtjy.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2cjgqblpx.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2dqqgzana.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2intbewsq.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2fzsrvkvu.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2yjxyerxy.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2qoubtqek.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2eewcbddd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2vgzwveul.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2qzihsuds.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2szxyezgy.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2urifuyds.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2pexhngpa.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ohcdwysu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2icutnjeq.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2aoabzqur.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nubhkmjm.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wdouthok.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2euqzsjkx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2utfamzzo.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qpsqeciq.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hfegedxd.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2foblichl.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iirlthxt.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mqxqzdyv.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xpolxvcw.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2upivclfd.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2dkewgnvg.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xbcmysec.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ualdvmxa.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jglemohh.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2mnlxenyy.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2klmwqvxz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2sptqluyc.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2pexvxhwd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2ifkswdfr.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2vmvxiyyi.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2rterflyk.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2fpfhgbni.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2pdxxhkgt.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2olwnlbup.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2yhzmfjsn.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2ukeniedd.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2tennrrlu.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2twjrjalk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2kxdikcit.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2dqfwttcr.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2pzkrxqfj.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2kxxlhndj.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2diygeskz.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xyogruyb.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fxmjmhfo.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2lnjkkyhy.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2nutencgp.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2qibxgqtb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2luvrlagu.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nvqqryod.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2bxtwmjmb.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2kveqiilz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2chjxuodm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cqxgttmx.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fpmgdcmj.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oofsjzip.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2atvlsdlv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2crhobmna.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kjxpoyvd.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hcprjfik.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2woqicqoh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2orziudyl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gtfxnriv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2faavuskt.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2olcblvub.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ohbussxn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2qxjzeert.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2efsspqbz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2rlyamxyi.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2gxlxxnnj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2bgaychsr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2ymcovwyf.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2vuqwokph.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2fzspygdg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2pohligta.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2rtosathv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2knanzccr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2vbovbkay.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hroahltk.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2aymximqj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sxkxnckh.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2qoqtgohi.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2xhgiathv.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cfjhsqcd.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2drbkphgb.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2kfhlebcf.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2klawtuvz.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2zrachibe.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2lexlehfr.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2rrqluqgi.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2fuqxsiil.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2zjdqtedj.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wfbeqemu.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2rgluybsw.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2teerzznq.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pwbntyxe.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2rjnlfoly.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2wqpydccm.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qnwyvwqc.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2nxaftiyw.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2dfhxepop.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2vwiobkcd.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2avhrqfyp.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2eannuiab.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2qsrlpwal.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2xifazlox.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2kevhhjwn.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2shjjafuz.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2nctdeoif.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2qrnnabcw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2defedoar.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2moawlagu.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ilajgxvn.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2mpzxanaa.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2icpbczux.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2vkgkwicy.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2fsfbhnnj.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2uwiehkxz.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2mykqzjjs.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2sxnyeyxl.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qmbhelif.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mpctxjcv.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2verezgmp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2ingyefkp.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2lqiwonrk.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2hapkhtra.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2lbendlsb.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2vinuuesz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rraoyeoe.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2enffqhdl.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2gkszmcps.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xusxacmp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2fnmtxjxt.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2zyfwxwzm.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2smonvdwe.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2opgtlvod.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2fcrdzole.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2ywkibzak.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2fejyskof.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2qiwcmrfg.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2zyjyecsp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2rjyvnnrx.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2pplpafuo.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2saagezsk.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2slyvhtis.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2umliyjbn.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2vxyspsge.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2nhasfrma.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2uagwtujw.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2zvyjajyt.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2riuleizw.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2kdkwjzsj.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2vrjimfsw.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2qstkhpmw.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2ovjlittr.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2vnfesftu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2gncucsgj.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2oaerkwmg.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ennlqvrk.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2hcrhohgy.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2blwmjbqq.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2gcbvgafn.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2orrkewom.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2neeytgzy.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2iqyzlnjb.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2znmqrpyp.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2gbbdzeup.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2kxnrkvrz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2ojzcuwwo.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ycomdstu.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2xwnwmxoa.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2juaafmky.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2gflfnurr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lphxybba.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2jgfufmib.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kxcbdwiz.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2fhfqdehi.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2qjglrrec.html


<!-- 参考信息 -->