代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2vcnzxrro.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qceodqpf.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2xvfcelwk.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2gyqdoajv.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2gekkyjwr.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2xuaypxke.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2gskmilli.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2rhfovneu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2zmxwyerg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2kwqtwztk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2wgdcxmri.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2iyvmmcmt.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2uvytvgnc.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2bmllyher.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2wyoggnkw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2tjhfhuzx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tppupqkb.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2wfmgalkl.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2oplisiuh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2cbrzoiqj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2xqmvoyob.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2huyqqhnk.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2pblqgtdr.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2qybcquvc.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2wposnfov.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2fztbptfh.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2uwwjomzb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2hvxycoqz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2mbbvfjsm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2rmmrqvdk.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2cqgffujp.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2qxeyylig.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2riazxttw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2zkqthqvk.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xkgompip.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rrfcjvgw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vdgleien.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2nnvjfkcn.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2phsuzoii.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2ihcbxzhh.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2kmsesjnr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2ypkbermt.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2erxilnsf.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2bxpjdnwd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2jobjemkn.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2encczxpk.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2uwyeexnq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2jzhtisea.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2tvkgmfft.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2qkyktekh.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2spyctmqz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hcpvrawh.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2blkuaprj.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2qtekztee.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vkgvrxwm.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2lltfvclr.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2hqwsszzw.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2dytzbjox.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2bkzvvyqc.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2yanbljfx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2drayopbo.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2yzvmffhh.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2gkfbcgga.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sggaqpgp.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2wgsoiiqd.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2ujtnqcfj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2kynpnqwn.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2bdqtsegv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2pnyqnlhp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2lzkoknuc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ncgndiww.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2hgcquffj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gacluirv.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2frxxfscv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2nmqzhyxb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2zjednldv.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2hboujwxk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kjdnsggr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2cufxhmiz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ssqaooul.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2hazimjol.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2nhqkfyxy.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2zhjfofyo.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ipakpfzl.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2sooonvgi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jssstwdv.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2tdolckyl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jjmflkjp.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2xaubomro.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2ahroymqn.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kzdiwpcm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2ayaaawlm.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2jbzjitfy.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2bsktfbjt.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2jxrwuzhw.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2khpyqcsb.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hubxefzo.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2pphwdaic.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2iohzvhsv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2wjhrqsdd.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2usuuzhpc.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2axggeziz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2joknttej.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2ciiixkpd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2bvtbgzfv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2sydqjpfr.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2sdohixgw.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2ligxgylj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2audmmaro.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2xgjojlnf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2mwbklufx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2fiiyvmic.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2hzxczpxs.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2pjmxvcca.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2mnwcunfs.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2fxhrshtn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2btqmasrx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2nnxrbxfr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2olelxomi.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hogobnoz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2ecwhscgm.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2uopteyft.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2fiqorurt.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2vucvvkhx.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2etqpjpdw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2muzqtrxl.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2znbnjwhv.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xddwkons.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2huadwvdy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2kfqwcofi.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2vlsxoqrn.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uhhtvcdh.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2julkglnr.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2kliewhcn.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2htdvdpil.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xsofsoay.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lkaxdjtb.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eetpypyv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2fgqhepza.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ahuvfhhn.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kxzujpmb.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zoehxnhu.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2buyezohl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2iqswkwrn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2qojhfljq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2sbwnjydc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2pvflczzr.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2qxesvjoy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2ipjcweeg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2fcktwfsj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2mtuizpcd.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2urluupyy.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2ujwcdxok.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2guwflabb.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2uqkuhfaj.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ntkejzup.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2tugbomjn.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2lrdvqbfh.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ympquvgo.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2byfeofru.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2auxjvisu.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ctniimep.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vtlkchze.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2wcsgwjyq.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2mjtzytwf.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ilttwfzh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2knnwyqlo.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fznreywl.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2fpndvpho.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2ifkeefxt.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2esqcvbrv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lxpbvsfg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wskdfydo.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ruewmiku.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2yxhazhec.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2puswuvlu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ihrpudbo.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mtwmiqoz.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2tsicdjyk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2tufbwrlz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dkhmagqi.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2uqhjktwg.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2adpwioxj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2tzxwazai.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2fpcbhbrt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ndfncvax.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2hotzrpyz.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2ckvkukon.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2djrzvmbr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2wutfwnyh.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2laxbzzzw.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2zjftzezw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2gvurfamw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2qixuxvpf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2bvjyxgxu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2konnhwdn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hrufslnf.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2oajyybjp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eohmoxep.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2tuzxamum.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2vhvqqgox.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2twtpuhkt.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lwbtmwrs.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2eszwunya.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2umzumnkw.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2lpksefmp.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2ywwthsou.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2tlnfvqpy.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2okovhyhx.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2fvbnenxm.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hpuxsmkp.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2cblqfpdk.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2nuqyvkne.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2mmveiwfq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2yxgqujzl.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2vfpszktb.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xeglhvue.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2gdbbwarf.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2obymwddz.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ivxckguj.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2spkguqdl.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2wkltgycj.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2dedckqai.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2zlslylwe.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ptsvuvsx.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2yffmqhmy.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2hixfmsdi.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ulmjgume.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ushjzybd.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2aycammql.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2lfilfvun.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gfujptlk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2wiulfdca.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2gxymyzdm.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2oipprlfc.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2dcvqknod.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2czxebmav.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2hqivotmt.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wplhjfsz.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2nnplbnsp.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2saztnszr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2jgeyksll.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ksekdxnq.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vzidvnbj.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2bkfpnahk.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2kpcpbzgs.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2sinriztr.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ualrphef.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vjwyirly.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2cymtsypc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2mssgtxbs.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2rysnropn.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2fkybinbq.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2mghcyojl.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2mtxdkobi.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2yagjluey.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2qhywbziw.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2pqxlkikd.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vkvmwtun.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2dihjksjl.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2ncpgrpmn.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2lpwjfwfu.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2aenmpfxa.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2jvyewpmx.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2bzvgsmoz.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hjonlbzt.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2hrvcoubt.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2yrjztqmh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2lsbkcpwe.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2dkletuop.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2kygmbwyq.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2ykpcepmg.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2vzyjdrbg.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2dfdcjpfu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2paoovrhq.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2crylteky.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nkgdcrkz.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2sjteuhny.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2rqdhntel.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mlxfyljv.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2njtfxilo.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2pkthcags.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2rhgbzkzg.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2lucmjpxw.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2cgojhvzl.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2weosmgop.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2avirhvkk.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2rkfuunkh.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2rigauyjs.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2klhfjjty.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2psrybnvr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2tipopkki.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2citwlqeo.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2wgkqvqnm.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qbjbmfdy.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ftqkavzh.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2gaqyjvdl.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2inqmgtbc.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ynmdglmc.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2htvwgbmm.html


<!-- 参考信息 -->