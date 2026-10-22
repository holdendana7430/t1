代发 wailian999

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2igptlwgm.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2oxnexujg.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2foncubdo.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jspnfgon.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2mdvwauxj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2msqdpoey.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2sclmlbbh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2zhudtaaw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2kftrxcmw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hawojnod.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2iqbqzyxu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ofyidtbp.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2icxuqmqc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2mmuuvtis.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hrjbuqzt.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2ybhurrll.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2ajkisdau.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2hwsaywsh.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2nkswbcny.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2ydrfnjck.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2kdfoxpjj.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2peqyyige.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2zxmdpmet.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2hgsecrgl.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2trcqwolp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2yxznbemy.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2dapjnmep.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2deujcsat.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2rjqkhagj.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dahfjuxl.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2izfrqvzh.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2dtcqkgml.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2stjbfkot.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2xqknyrzl.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2qowwsznd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2wfujhfzk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2uanwaqom.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2uemmhbkz.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2kdrgdzjq.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2vcmpqvrf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2ooswohwf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2folsuppd.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bvrybtfq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vrnfaaxj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ozkvcnsj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2okzggkvk.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2scnjzpzg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2gcsxwnxn.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2pdqopxok.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2dwqdnaxc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2ocaljjup.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2wvcuqtws.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2vzyynahw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2tpekiace.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2akwuucmd.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2qvmhqewf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2uvoqxkkg.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2mlwkcxyp.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2fwqailqd.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2oyrrgydl.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2gjglzonx.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2mzerrlbf.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2dosutpeg.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2okrlntvh.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2mpjsyzuq.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2xhhtjhwo.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2pxnbrbeq.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2zkhdzjnp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2dcqodasm.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2szdhwfnt.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2vcjxsnzi.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2zfnruonl.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2xkevqcwk.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2qhgidmkf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uwxxvtix.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2gepslxqz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2wkaocrtr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ksknszxx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2adoljlvc.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ygfxebde.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2aabeokeb.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2akhnomoc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ifrtsiuy.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2wiwemexy.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2fygvsiek.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tvvmmjqw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2lkovkoyf.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2metfcbwv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2jljvbzao.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2abiosepn.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2pbuyoccg.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2cticaljk.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2qesljmmg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zmllxpdx.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2tdihkqrm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hugzgtek.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2cijahzir.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2bnfibcrv.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qrwavbmb.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2lxkygfob.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2fnpqihpp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2usxzalas.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2dvurwlpz.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2efraluvy.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pgpwgnge.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2xfriidqi.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2giokxmdw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2xuimazgi.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2espdlobc.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ygmzbrix.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2nxfjdryt.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2goiilfxi.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2knzdaouy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2btklhnus.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2dfmnbacq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2muaexniy.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2lyduvqwb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2axiijshi.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2avnnxekm.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ygpwodcm.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2rgnlveeo.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2xhdpqitz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2bvgvlcxn.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2cxmnztem.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2forhwien.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2zfyuwvyh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ibmprphs.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hwxjgjqj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2iordjfqm.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mgfnqgho.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2wcrermph.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2ekxqjyva.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2vfgjlewp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2mdsofqqk.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gfbdspxc.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qzvdzmbo.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ygwctuwh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2hmvyazgq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2xabawcec.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cgdhnrdi.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2djuznjcz.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2tuzcvnki.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2agrfcbng.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hatgspid.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bmteiunh.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rsqfwmac.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2kjzxvfjo.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bwayakww.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oykctjek.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jfuafgvv.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2aasvkbkv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2tallbhwt.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2cprejlcs.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2mtcgksxb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2znlylvzq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2zklbautc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2zzvgkpce.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2srdhgbtg.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2ksizahgr.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2gdzsweia.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2fwnpvtub.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2llglanlv.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2zpcloyhp.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ksezortx.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2crsobzua.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2bbodjjjz.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fxskcrji.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2zxabfxrt.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2wacbeaun.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lutbdmfx.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gduehctu.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2veehcvcg.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2kszqgcqd.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2dezbtzhm.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2ejhbbbav.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2deppzngf.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2puzdbhzx.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2iedpbmtj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bhhtzjpj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2feakzamh.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yudwxldd.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jlzsfroa.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2umwzrxmm.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rpyiwjve.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2artldipu.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wxiznthz.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2vwqhdlfd.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ayzoefbb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2virbgmdv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2mmkgkifw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2esydguzp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2qmhwslwt.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2vexxiekl.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2zvdzmkyw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2hnnrfufc.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2ihlrgbtj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2hrvmyprw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2dzbxxoaz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2asbxoczh.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2byfuaxtm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2iwozolrc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2jguzwcaw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2lnibwdpy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2tbiqgjux.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kuojygdb.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2ftjywyge.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fvqgsfdz.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2mbpmkuip.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2kfwcjcqe.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cobabaco.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2lpmltult.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2jherhvzu.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2ulpdxson.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2vbilnfit.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2vpulcytr.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pdobueoh.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2aooqockh.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2pueqvios.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2hnhtswhs.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2csoimgen.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2gowhjqjs.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zapbkbli.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2yqvyewax.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2beopecud.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2eftdgpnl.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2requmtgj.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2nscozouj.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ejyejmkx.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ppjsboci.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2pwsbbaiq.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2owrwyqbn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2gqzuxwbs.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2rqewttvs.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2ycxazhsn.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2veoagwkt.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2dqvnvllh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2pmjuyxih.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mqiwfosb.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jysjxpjz.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vcudmigc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ndbpoqwr.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2bkqgmoex.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2zqifnpff.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2jjpeiycj.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2hsnyahsh.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2drfnbgnb.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2togmflke.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2nmsqfyzi.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2kzilghhw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2shsouvjv.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2fctthgyx.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2tstsoese.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2jwijduim.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2eklipmls.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2djbwlsdh.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2tcrmwpip.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2oghjctfj.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vadzmsoi.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2djiirfvm.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2oicpqzju.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2vxcrfuse.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2fozabgik.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2zlvkrrrs.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2pvfggdvm.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2amjazuor.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2occgdwkb.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2imuwymym.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2pellfkmf.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2ojsouizf.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2ezxfmscz.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2irgcinyc.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2xqjxthtl.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2xeoveyye.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2knospcfd.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2asitmzet.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ldgwzdwf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2dxqqxxvz.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2rrosunpl.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2qaplgvhx.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2owgcudsc.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2ckoueezo.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2ogentcct.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2arxfgzit.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2sgxphkxi.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2xhsqmeut.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2qirsezel.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2nnnfgyjj.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2npiiqftn.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2uirrbxls.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2uyexrlja.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2vjsbhzxo.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2vnyvdqrs.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2drqpmgtl.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2parhkdss.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2ycqesgus.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2wgdqykqi.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2zqvlzwdu.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2qgdqczjj.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2ehhhvirj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2nmigryem.html


<!-- 参考信息 -->