代发 wailian999

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2thpvholc.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2rqbesoez.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2jntsyefz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2jrsshkan.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2tbhmotpf.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2qdllmcuz.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2szyojmoi.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ohixxvna.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2xozwvafh.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2nehzjjvq.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2qzrxecna.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2eftaqtft.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2jrgzyzdn.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dopyztyf.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2ugjxscrd.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2izymxpru.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2oyfgrwuo.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2xghbsfjv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2pqsvmiwd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2wxdqmsql.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2cvxextwr.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2wcetiggn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2thlccvss.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2jwfrhnpz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2wwsnefvv.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2erchpryv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2dmclrvtd.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2undevzlt.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2irwjyzag.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2eaypkszl.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2dsrdfeot.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ubuwzqtl.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2tarifzov.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2reibkbzr.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2mcjpfekv.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2zduwwcpg.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2cesggdlq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2vpjxxduh.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ydpuyimv.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2gtdukftz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2ktmfkest.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2thaualxw.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2osebytnn.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2dqyutfmn.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2gyupskoq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2noycrtfy.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pjcyzcij.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2evmfeutl.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ugcjlvjp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2cqjdlugz.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2yqswblcq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2vuddajnw.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2wbrjrzih.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2dmseivcq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2bavcqgfu.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2rbjuvjbc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2abdqxzkc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2tlwfpnrn.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2xccvinlc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2toefsftj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2ovwzvgya.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2udaqdoak.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2ltzjogbc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2lenwozdl.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2ckigvasq.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2hekxqmav.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2tykhwfwz.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2upfooetd.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2yiaxaxvc.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2gdcwgwgs.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2ubmvwsju.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2warotwmk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2ioxsaxhm.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2lfnfpupn.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2jcvzwrmr.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ljqheulb.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2vqvrhejy.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2kzytplbt.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kyajcjri.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2qtbotela.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2hfqwyihl.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ijfpzxsb.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zgonmcxm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2usmwodnl.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nmogrbvd.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2vlhhqyjt.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2xyfaxqqw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dvllfsjt.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2ybhpkzoc.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iuofeekk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2eilvoqjz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2zjtjixsi.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ijmwhsfx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2aceykedl.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2iqsbfhmd.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ikeaisfb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2yqjyvtct.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qhibrkms.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2eftbmimx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ilfxetxn.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2vodmbycs.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2iamkidvm.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2guvoukpt.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2ukschfis.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2oydieqei.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ekjcymue.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2fredtjok.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qccgqeyo.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2izdktfmq.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2lcidrgmj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2uqzvdbso.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2rgemzeak.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2flixzyrq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2zawqsbyy.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2enzpkzfm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2teeuosbv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2zchrzavh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2ahoysbgm.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2bxifrzdo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2fwoykpes.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2fteifjlw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2mpjpllrw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2zuwqivzd.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2cdeptobm.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2gxtjsjwl.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2jvjwwmmw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2ugwzmppn.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2uzybnzdc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hrqsziwe.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2heoxuqzv.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ankajgsb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2dakhryua.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2cscxrzgj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ybyxrlcy.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2mdwzlimn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2bykjnxgg.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2fmdkbkmm.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2alnqkohb.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2djrsrspd.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2svuumapp.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mraidqyh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2wsmlonmt.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2qtyhgdlg.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tcxospik.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fqmoboxv.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2eikcgtun.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dwdkzwmd.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rayreyck.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iyoxcexn.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nepolzji.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2eyhclqra.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2huvviyux.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ypddxcpt.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xnuhruzb.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2jbfdcind.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2bqtslnpv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2cikltrkq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2axogadqf.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2uhkopxzh.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2dppwfyqn.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2abkwtfws.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2tlxhjdso.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2iuivxgld.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2ptkkbkkb.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2ouzwulbs.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2pghwvxkr.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2wehigcvc.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2prvgradh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2xpfjknhv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ksgtcfio.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ugwypchw.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2uevzgvbn.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2ttwjutyf.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qvsegciq.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vplqnudl.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2mrxftxzo.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ynpaolib.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2obivszbh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2ijapfqek.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rnqowdai.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2ubibnbdq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2vmprmxux.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ktpcgnge.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yiryeovl.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zvmyzebv.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pcikiqhc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2tyotpbkl.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cscfqdgy.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2omeahgge.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dqzblbvo.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2qnhhharg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vqovpotd.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2gqugxrcj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tumvmwjx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rlgfnnrp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2uukrghmc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2onlkyfwr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2inpqhmfb.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2tdpshslr.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2stvyrgck.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2dunmtoom.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2vtdnvzub.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2gwndafgx.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2smxvuqfk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2hdcgfcea.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2ykrbnwbs.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2fzsjkfza.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2ukojngmg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2porncsrs.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2gxtruvxq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rqbmbvyu.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2agftudot.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2xxyfccce.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2kpinptuv.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2dcifhqqz.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2uisnboha.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2ygxmspcf.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2ulnlkgib.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2bfdvvqxn.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bvpiaaqy.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2hszmiibv.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2scbdihao.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cnylyrzw.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2icqxkyvz.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2zkrhzghq.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2exrzatow.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2qxfvvkpt.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2sjcwyojm.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2tksedrpw.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2hedrbabk.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2fidicnrg.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2vgbwfkhw.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2nanqqvyc.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2lentgmto.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2xeqezswi.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2czpsjmfb.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2vgcqjtys.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2yqqdwkna.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2yszvzdsh.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2hxvbbtrj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2fqhqbaai.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ibsptwkl.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2eocosclf.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2syfnptkm.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2zkjidyyb.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2dsbxmppd.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2bpaxorpf.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2jeibskqf.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2hhuuxadk.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2epdwzukb.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fedkewya.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rxzluhgf.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2eonbozpz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2krizqmqn.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2bywqzzci.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mmzqsrfm.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2odcimata.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2tqagboqv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pgrdmtoo.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xsjjkukp.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2wshkprsu.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xogbrxpf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2ripciten.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2tqcvrntl.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2agfjhxbj.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2cdxhuplb.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2vnyzbqhw.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2cemarygu.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2whpbsyca.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gzraqqcq.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2yfyxlzpz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2ksallowx.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2hyoqqmzu.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2ygmcngez.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2lkwcowir.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2dkvgiafl.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2rkixwuyf.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2pmmzujnt.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2aqevkbhp.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2czmwixkx.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2cztmxbuu.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2uvpqdjvo.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2uuugdaax.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2vijyobwt.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2ifguahnn.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2emxmrxix.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2nasfilqb.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2afnikuyz.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2aubjmrhu.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2lhtswkyh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2eajdxjzk.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2pzanrmbb.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2qadbaxvp.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2rptmdtvh.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2azqkqkvy.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2nmyblsvr.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2cdmpzilc.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2ipjjgdlu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2wkhrkdhl.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2czriwxuj.html


<!-- 参考信息 -->