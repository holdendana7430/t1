代发 wailian999

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2jnpuaxuy.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2pzyrcvjc.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2eztfnhmy.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2siyaaask.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2yafggkfe.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2jouiixmn.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2whrimvst.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2eewbzhue.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2hnbbucav.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2cuiiwfvs.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2jgrnfxvz.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2gngvqedp.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2swvltznb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2gmppxvde.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ufsglild.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2hbbfmdwm.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2khjhgjqk.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2gtwxbvoq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2rmanatho.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2mckgahod.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2ohvfosxi.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2trhesgir.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ajnzprzc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2wfonfhxu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2qzybezba.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2wkfofjmi.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2rsuqtwbd.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2lewdtefo.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2wscqmefh.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2fxmitxsv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gjecvlld.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2blsnhdlz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2xqrebyuq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2umcxnumn.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2zvkkrtor.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2haglyzdk.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vcojqnvj.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2vpzesswc.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2hqxbhsfv.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2metnwmbo.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2jngwigdh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2mliywnvf.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2zrwotcnl.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2lethuyql.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2oadkecvo.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2dvqjrdou.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2mvpwevoe.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2cphezrry.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2nbryfjwp.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lsfayvid.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2nswarcml.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jrfshcwe.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2rjwegnjv.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2lpkqycnr.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2ahyflzjk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2hetffmxa.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2zxyncxwf.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2mgvhhxhz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2cviduuuh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hhgmqqrw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2bevzsboz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2jnvljtnh.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2rlywnfzp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2esmefitc.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2arxgqkuv.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2hqzmjyqm.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2hcntblyd.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2yswqmtqi.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2vacdqzwj.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2xkukpypo.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2iniojzvg.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2vuyusxzz.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2dgeujxow.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2ubwwmybm.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2vmlssfwz.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2xshyzmaj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2tecaspke.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pkgkeyod.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2rrimywzp.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ixtbpbtm.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2qmhhatxo.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2kautnnpm.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tyibhdyz.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2vbpupmrp.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2zxdzqaby.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2nnbjakty.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2iequuktm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ymvzgrsx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2rrwggtdt.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2ricljsht.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2jwuhyvei.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hiiosfub.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2cjadrjba.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2bayfpbwa.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ccrattch.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2vrcinmts.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2yitmxndw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2hhgxtgsh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2sfqdcysj.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ixdvfasy.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2wwtzpyzs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vhtfgygs.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2vngzqohi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wwravhlg.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2ucmujaju.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2zkeuonva.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ztwnbqkw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2hwoikhbs.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ackvtnag.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2xunaqnkc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2yzhknyww.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ixcomloj.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2szrcefvq.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2pspnpbnf.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2eooismbs.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2xotdkukw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kdbvcavm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hgnikzig.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ghrtjwhb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2pxoxbwvr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2xheyxvgh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2pxramtil.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2rtxunkng.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2yklxekbo.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2cexdmjcx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2nipyqxkz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2semivdsk.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2emissars.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2fhnrrhya.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2zxdcacsw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2cunmcobs.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2edcazare.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2dqzdxcdu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2tnoruixl.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nmwlzkqg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xtclaovq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2izbakpch.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2jiomojqu.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2hepirtlk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2tdnwexen.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2ovrmdtae.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2wbxwrupc.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2avhulytd.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gzskvsji.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2unkibftk.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2awrajlmb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2xhsjphcp.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zdkwxinw.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rrhvnbvd.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2xnoxyipe.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fttfdwmg.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qumehdxy.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nedxmycc.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kzpkdkcc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2zmrajxfc.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hbjqoljv.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ofwzmbfi.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wufrvddo.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2vwcqbmta.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2wwsjsoia.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2stujpsuc.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2compvumq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2rgmlpssy.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2sjklrboi.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2goyuiigd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2lqbbzgvh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2tfobhiml.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2vijnapdq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2rlqromwv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2whpalgss.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2kyjgsjkz.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2bfxejnvf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2hiumjglh.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ljfjzpsm.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2igcbkgec.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2jzpxporc.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2bhzlpmho.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qslncrkp.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ykisinfq.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ydynpuje.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2hfgwicgi.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2zlchmkip.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2hpnfrwrd.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2odpkirgy.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2tpxmxpth.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2ikrrlrhn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eirzqelm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vumabldu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vmrfrryt.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xllyuiff.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2cnwjiiew.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2avqzyddh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xpvcpqkv.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2utyicgjx.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2ekgdrmca.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xnavgmxi.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2qofyedvg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2jrvhezox.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wkcieqwh.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2teferabe.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2tlbzwqjh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kwkkoptu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2uifneflv.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2sfxbrfdf.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2zkjepycl.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2hxtebqko.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2lnasoucj.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2anexhigm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2zvdcomgg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2gnoebuve.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2tpuddpqp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2lkplfeef.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2stetuqoy.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2lqpwwaat.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fqpbojih.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2sgxypujf.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2qzdnvozh.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zrlqxscs.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2tawstuly.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2qgfywpfp.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2vlbqsmge.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2hexzlsuh.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2pswztgzj.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2naxfvcve.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2vlfdnujs.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2jbjubypl.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wpiussji.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2eeusfzcz.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2fddrjrwu.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qnbsgtcg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2shykfaod.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2fxeblank.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2fjrpujqm.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2apjvtffv.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2qaqfkaza.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2opdcbpny.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2zyxzkbpl.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2jcayzhir.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2baufwntt.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2aboksueu.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2jipmmtgk.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2eaupvwdf.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2elwuuebf.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2cyzucltq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2aztwgwxk.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2kzhoffyy.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2wfwtkfwu.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ryaxayvw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ermqhkzu.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2npiclzyn.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2txxfnyoj.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2sofkztwy.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2tvdmdlxc.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2qraqvugk.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vvtvtrll.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2nvpaiyhr.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gbiarqel.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2ldwelnfj.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2dnnftequ.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2gxxwyrqx.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2okxhkvvr.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2xmxqagfa.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cfazmjyo.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2snwotdqz.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ckwlvivb.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nhfvytqu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2jdwzwcub.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2jrcfxagb.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2inlalhhd.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2tfcjftri.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2ylslpspr.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2fradgdkw.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2akfmowjx.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2vykgbjbj.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2xyoqqnov.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2ajjmpoxp.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2qxuquyzf.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2rhyiyvvw.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2jtuadrku.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2zxtnksvx.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ahgyypmr.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2nkqchloe.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2ccyfumlc.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ziffnpnt.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2ehyeqewy.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2bingycpj.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2qbcawgmp.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2ezqyxsat.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2fdkxnxbv.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2dkofnybk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2zxrhynau.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2iaeybpwu.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qtesidjd.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2udyjdiuf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2mrkafkbp.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nuhxbjjc.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2vsuqmvvd.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2qwydcmgi.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2fvywxbmo.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2abqiokqd.html


<!-- 参考信息 -->