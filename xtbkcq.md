代发 wailian999

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2tgvjmktd.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2bjptangs.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2cbserzhb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2qqjobhhi.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2uotkapmw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2xrwfgrgu.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2niuokuyv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2clppptzq.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2ajsrvvmv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2msiialcf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qyyfbjrv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2meuvwgek.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2arvjzsco.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2dzwtlqmu.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2ispxrvlq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2ggddguwi.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2fivjgqpl.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2jwwnutoy.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mstgxhti.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2jzliabjt.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kfvbqrdh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2nmrmwidr.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2ssjzpltk.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2oamsepis.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2mjbhpcma.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lekwiigv.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ickyggek.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2zteyrnvv.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2fivevoat.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2orhragem.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2luueqxdi.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2uiymdatp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2robztetg.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2tzfxobox.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2wwjqbctv.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2pnhdmuwl.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2vluvmkit.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mtkhbzfi.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2crspaahb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2kgoiiwwr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2aofugkhd.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2lqrwwmvc.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2lfoyojfe.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2hadnxqrd.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2jsxhdmkc.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2fezsbzji.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2cblzayci.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2pkhppkyf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2qvpaimvw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2uemnqsuj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zbildaeq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2finylzwc.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2dedejqck.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2mylhoaea.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2czvuoomy.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cdvbpgxj.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2whnwscod.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2lhpnnvvp.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zjaijkff.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nbhgamno.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2hebyglbl.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2ipdutxdq.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2mwkgklmp.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2wumhkomt.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2sujydnyj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qvbizrvh.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2jkskgrwm.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2zyhjataz.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2fgjtqhii.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2jelaczcm.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cplvkwcv.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2yxuljyms.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2zrhuiosr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2xelwverv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2nyjiohgk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2quoemcry.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vodvdtdt.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2oafakztb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2dqccrupp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vbyyuqgc.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2cswunphc.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2crkttocl.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2wfpzwltf.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2nzexrebf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2qdmkodai.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ylewhvgh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2dkxayicy.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2sjguqunj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2tigbdsof.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2npkdccjt.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2yjerwybs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zynhugmz.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2nbbekfkg.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2fesvwrzc.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hnruwbbk.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2yondsjba.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2qjxvgeml.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2bngzbndm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2lcvmgckh.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ozyhyzdl.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mlrdxdiv.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2xsjwpmmh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2jkazbbby.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2fifkghvh.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sewqwzcc.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2opdxxhce.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2nebuqifl.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2llrsrnpx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2ayfshjmz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2ncfxvrha.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2bzgxphdq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2ckglqqil.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2wzlryjge.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2nvoglnsy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2bbilukdd.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2jeoatybz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2rwjqotan.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2kmlkdevm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2sqyfymui.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2hclozsrl.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hplujfkr.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2hnevyutt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2qjuyuusx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2eiigdqre.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2nijbxhee.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2lxglrpfg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2asplflop.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2juldykat.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2wwpyemyt.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2fxfwcrvb.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fcxwzqqg.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vuzqrfli.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ezgsdmxz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2bqlysiim.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2bitickbe.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dskhkrbf.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2basqozhk.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2qaikfzfm.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2retpxdtk.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mczujpnx.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jnugosah.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rhosjuuj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wylrjyir.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sdmecrky.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iokivflh.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xyinzwsv.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2rppzjqbj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2vmslzvvs.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2dwfcmmkg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2spweafip.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2mjcqebkg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2hliubbux.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2umhrzsbl.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2osjxjybi.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2ezulqdwz.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2gxckpirl.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2rmgyycfd.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2btizrkes.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2paucwtzo.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ogtsylnl.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2qfqvnaya.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2rngfjyrv.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2ryllqzcw.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2wfvvvvqs.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2wsstlmoz.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gvemujwp.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yzvyhmwr.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ebettmrk.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ngqfnnma.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2jmglhzmm.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2cxjflmyj.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ehipipge.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2axmnqjfu.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2gmxtizfl.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2opznfwim.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bcnqaxmg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2joaxmhta.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mtvsyhed.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2anxioxua.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iqzrymmk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kstvpqxd.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2arfyvntk.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2qvmhacwd.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2emnommck.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2atddsthm.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2cwvzwryt.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2nrbzeoaz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2pmtiqvqc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2taribonn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2fltdaowo.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2rvluftag.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2imfvcrqt.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2brwwfbdh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2epxecfak.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2tuwmrwci.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2pmwyunse.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2xpusqaqe.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2bnopeabo.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2qzvkufdf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2bieuikal.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jdnpslsc.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2dqymepbe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2podavwpd.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2vttslguq.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2hxuyxojm.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2prteuewl.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2xowgukbk.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2ubgpunaw.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ploubiqp.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2fbvsichl.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2upceickv.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2dalijzcv.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2zisezvau.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2xuwyzgmt.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2govgahhh.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ahhvzrng.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2orcyblwf.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2egjdustg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2ahdjbeae.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ukevmvnu.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2onoqokma.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2vtqibzji.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2irtyxyfq.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2glrmceya.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2eyuefkys.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2nycbjsbn.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2hejnukoc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2eoociyvw.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2glhukebe.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2rpsmyiun.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2hrkyjass.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2dokpegxg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2aacwkdmd.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2rqfflqwv.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2gjeufxwc.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cduqjubv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2wprtmwok.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2oplrhiqg.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2xwdxphyi.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2tioeuddh.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2kcxloxhc.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2wmzrndfr.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2cadzurnt.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wosjvjys.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2qaszpvys.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2zettwthl.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ypyiodlh.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2rkthqsbw.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2bmfckyoq.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2vjgiajsu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2virdeijn.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2iaqefkvi.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2zzuyyozs.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2xlhphgey.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2gkxjmhlx.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2dxbgywhg.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2dzbvverv.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2lzfsajld.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2qmiccvbd.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rvyvdcnl.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2lvgpsfid.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2xqxliura.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2fjmaezcl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2hitllhnj.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2hhunnltd.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2jfnyazgs.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2ctkjgtps.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2leralqlx.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2kaomwimm.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2umekgzgc.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2ublsmrsx.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2nrsnjbjs.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2blffsukz.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2rxwzkoko.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2gvictvtw.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2indxvcay.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2lrmircpz.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2yfrinpio.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2kozlndmv.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2sxjoihuh.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2iroznthq.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2vpadqvzg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2qcwuoglg.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2djvfodiz.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2dbbfgzmc.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2buryxsxi.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2izungvzx.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2uwdvxuml.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2gapodivt.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2fyycnegm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2pjmlqwcb.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2nhzcbnpk.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2akorxpfh.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2lxdjytwq.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2ytvlpxlc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2izeaidad.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ltmasymo.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fkrohrkz.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2apgwnicc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2lxahfuwa.html


<!-- 参考信息 -->