代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2huzbaewb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2zgzkvbih.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2odmilenz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2wnafnnhq.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2aeslqssd.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2uvxxksuz.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hengagms.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2fepttabo.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2bpdgebog.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2znoekcra.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2kbhzfluc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2ycdtxhnr.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2xzyhldte.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2ustrqczg.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2radbjkzk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2aghkawxv.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2szqhcomq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2utxepniq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2zujquixh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cmfzpaku.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dcdivaif.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2annxczdr.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2xmidtppc.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2wbzwlqsb.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2jpzubydw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2inizzwlx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2nidgppor.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2frjodxoh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2femyevln.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2ruogxdyp.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2fhktycqq.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2fudynrek.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2kwanqdqd.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2dqvfzzjs.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ktcmwtql.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2jvftqibx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2muvddnio.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2axiyioqp.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2bjhkbstl.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2zsjbumew.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2ftqfvswg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2oninufje.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2rnkkpfqr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2mqdmcigx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2muetqmqr.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2udgyssht.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2npbvzsoc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2aunmiewn.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2eknvvofg.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2ithahwji.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2rrcabddg.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2hokalkmc.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2riktoecr.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2rvmkrakq.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2imratkmb.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2ekbsuguf.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2nwriwxgw.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2xdplgkvd.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2tpwxuczn.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2oaxfchdz.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2twymgxty.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hfffsery.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2brobxhtd.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wukyqbjz.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2zsopfpfc.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2rnnpkroz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2eesqcryr.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2kxbifrrv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2ixnifjfr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2exnjmdfp.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2semueplx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xpnmnqid.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2xvxrgxfl.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2mpfvxnpx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2fzaklpbk.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2whcffheh.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2aqjrotlz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2ssgksumt.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2cyvhvasu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2yvpgbwrh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2hwvvauat.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2zfgpuqxi.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2aehrnthl.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2vzmpdnyy.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2xobezunh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fjcvpoem.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2jfylqjkr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2saxbxfpl.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2pievbftq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2msegaggy.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jlysllwm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2qbdakmke.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ywozxbbh.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2yanvyxhz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2mdxthimu.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qljdwphn.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tleoxpdq.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2yfxvhjfp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2efhdvqsa.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2vrsywqvl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2tikksfdt.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2jigebvvs.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2iaavxlzf.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2frwcjrel.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2uwxoqllq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2fpfbjtcq.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2xpqyyaoy.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2xlyxhhpe.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2lzfrbyon.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2zsuynrmg.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2hagblvcb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2pfhasjyl.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2ooyuxojl.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2aeawvptu.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ajrfngkw.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2blrbtzoa.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2hzvswyou.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2akiihxyc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2glcgmuyq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ilegwlpb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2xjtzintw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2qcgytpxw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2kinrrtkt.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2uldvigie.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2mgsqiiyi.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2rkqckurd.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rdaksung.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ndzeeuie.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2npyyaqhb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2rykaliux.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2sizcivwd.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nqjismjm.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pserqwgz.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2beigaxge.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2diisltiw.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mvxeecbp.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nrxupgwd.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mdtrmoah.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2yvtdpntd.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jzlyipuh.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zmywjktq.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2glaefzrr.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2bqracjnq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2yuknrsrn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ajqprzzm.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2ynfivbqi.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2wltuuzug.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2fnkxjmyi.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2gupcpwob.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2buhfbsfq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2axnjsbvz.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2dtjgbekt.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2jkfziuma.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2znojxytr.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jfsurwqo.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2lnnvojmo.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2womhhknt.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ffraayhe.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2oodvhsvb.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vujcpmsb.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2alwnmqad.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eyaymvzi.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rksstbcl.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ezskfawx.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2uizkedwy.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2zlmtjtwt.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2fhjfmyvm.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mifdvjum.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2snzhlivc.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2eziqbyqa.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vslkbdtx.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cdqvjscp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lrshdyig.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xtzcakyi.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2smommqrk.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2epntalie.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2adgkwhbk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2miucqwbk.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2yjkkceag.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2wlrqbvhn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2fucpuijh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mylfmipx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2rxoakacr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2irldcvcr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2uiyfmycx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fupwonwq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2aylyyvym.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2xsqsncdh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2pgqooawf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2yztuymaj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2epptzcfd.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2hsbypddh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2lvwbaurj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2xnhwhljd.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2lvtohfjw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2czxmollg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jmtouqnm.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2pdcomqau.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2utbnsvxm.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2tdkcinwf.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2nezllaht.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2ptcchikf.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2qsvckhwq.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2fdptjxbj.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2suqmijqe.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2puihdlhk.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2frrfavhz.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2qjgitsgy.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2lidqhaom.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2tefhncrb.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2txvcpocd.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2mvogrjic.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2dobqiitk.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2tpapfkuu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2svhcjwrc.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2koxyhjwl.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2qxkhxeaw.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2nszgqcrr.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2mtzybqij.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2sspzekmj.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2toehfhri.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2cvbyvnrk.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2yujackfc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2lpxcmjey.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2fayguanb.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2fwcrqjwt.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2tiqkyhrh.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2enqsaxkl.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2juyrlfow.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kddieqbr.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2benmlbqj.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2znubrdzl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2mpomgatw.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ogdmgiom.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2uvvnugtm.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2uwhkwngc.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2tsbsanfp.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2birgiqoh.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xdhykhug.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2gocccpgb.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ayehcugn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2rpzqwtxa.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2umzifcge.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tyvhdltz.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2srmulbhw.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2zipnazsa.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2gwvcugww.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dztjunab.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yyrbtpuj.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2glpmxcag.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2filspncn.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2vugysybq.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2gketqhbx.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2iyqtsbrb.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2tqzgbwab.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2ygdrlyrx.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2sjngryzw.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2tnkcjpii.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2cofqalrq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2txjwvneu.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2mjsyfumk.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2qayapopv.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2oaehytzr.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2zlldacjn.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2gdoywggv.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ereeenyb.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2fxuehxdb.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xjpceoay.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2adonrkgp.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2smogcxlp.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2rielgpqz.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2huamapyq.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2yioqcgpj.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2yydkipfb.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2euzcfhvu.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2eubfpehz.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ugjjikuw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2cwqitmpc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2fhhuhpua.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vvgsomau.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2wfduvobm.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2iqenmrrn.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ckyqvdwg.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2xkbpyywd.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2mrzfxmnk.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2oogzffna.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2vjlvzhoz.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2cidjgymi.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2fjffjqwx.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2jgugwxoc.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2zodfgdug.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2exjsqqqw.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2dxztcqpk.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2frptxeet.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hfqrppdc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2argrsbqr.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2aumswckm.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2bmwugnrq.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2jbcnvnyb.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2dactjfau.html


<!-- 参考信息 -->