代发 wailian999

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2gbqhdgwv.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2irggpcbf.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2zpvecmdx.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2aequakbl.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2wqrnaacr.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2oamqtuqm.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2wrbomsap.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2xdfvonhb.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2trwtmill.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2oldovdbx.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2ezuurfvj.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2wdhpicrc.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2emggxhna.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2xtmvkqly.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2qmzzgmvy.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2bmdubhgy.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2evrrduxk.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2ezazqzsm.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2lnynjzya.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2yqjdubth.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2prdzcqxu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2keladtup.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bsuortbt.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2msyszzfa.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2emyxbajk.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2zngrjxbf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2ukefztod.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2jivnzobx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2eqfcvxxv.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2kuqxdtrr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2uuvzzwdo.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2oakfsgfj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2ioeifjdz.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2zoekcwfd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2gwbpsgss.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2emfravfl.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pzgtfgtj.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2leixyfjs.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2mxkpsrxr.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2yjapipkp.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2hcxsrbzx.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2bzbtcmkh.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2oawxnvsi.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2alwzoimm.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2htpzejbw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2ywjeuedt.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2fiqxgjkv.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2xzuqxiqr.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2hhawyzvg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2pfxhmily.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2yyrvfvtr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rvaxjatb.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hooimkhx.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2jirqxzzk.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2ykyzjbbm.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2dpmiymrb.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2luuxcogf.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2mkzzfdaq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2rumflxxl.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2yodyqymr.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vhopihbm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qgxsdreh.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2tnnxfxcq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2wneurkco.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2gegrgvin.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2apgsjbbe.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2ucicqmxr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2uebpghax.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2hzvbgcfv.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2xmrcvogw.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2urpqapzd.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2eztyajub.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2rxwqyuqa.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2nxmxopei.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2bqxrlwxj.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2dblerzji.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2eglhpssy.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wbnwsxra.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2jscmtvgx.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2tvuxwrdm.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2fbabeyel.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2yweabuye.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2hhzuzgbi.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2voeshkzb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2btubtohc.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ocurlsoh.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2gbbtitqz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2lfhuvyka.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gohdlrwa.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2qzmmwrcc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2cazukdvr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qdismevj.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2dnfkwhjf.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pvzofyad.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2wutzkihz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2hjvoszcs.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2zyjzjmkw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2mswqahaz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2kefqmqdx.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2hqxvvmcj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2cirkyszw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ysqbtcmi.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2givfrvvf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tmswsjsd.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2wwjpqspu.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2oaqjcsiw.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gdaickuh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2ozdpytea.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2icyyaxaw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2kpdjecyx.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2pkcsqyhz.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lysqahhn.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lzgujzuc.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2opqzynfp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2ewnrkgjs.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2olqwgsxm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oucceaqs.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2snbtiqme.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ghshdcca.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2hiaeyqkr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2xijydsgz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2rpkcewth.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2kzdvcvms.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2oyfutdli.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2kufmffzu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2crnnfjnm.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2msdjyvvo.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2dqjlgwoj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2nicaucrw.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2xetkdvvz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2bgsnyjgj.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2zjzokqjs.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ieupmcoe.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2dqwznnlw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2lhpgnnux.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2fjmzutzr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2lsflntic.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2nbikayts.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2nzezwdii.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2eqivxswg.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ugcxymhk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2igmuhsvi.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2igybrenk.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rwwjrvcp.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2grkaqphs.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2uynisdqb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2bdmxdgjy.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xokluudm.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vunozsbw.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2otxleivn.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tffxwfcn.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wpzpvmwz.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2locyhlfo.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ekrdcajk.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2dvkpqbuy.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wiazutck.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2itidrhyl.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ohkzfxec.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2ncpnghfk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2mjwtwuqa.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2bdevvtta.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2slqjkzuo.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ehzynkzw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2meqnprua.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2uuvfdzua.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2gfygwkcf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2syzipeyn.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2miftkgzn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2oksjvenb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2hrroutml.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ueuwbjyt.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2pqjtxciu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2lbarlotb.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2pmehmwge.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ndapqzga.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2ixzpzipk.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2nzbdwgdm.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kpsojeam.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tldjyzex.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2udsqrkkn.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2hkoajfzu.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wypqiiia.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2tgavocwi.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fdokllrd.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2mkfjlgqy.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2aiykpzhv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yexgxteg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rrtduuax.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cfcecgow.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zqsgthzx.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2grqtkafg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xjklihsj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qcatstcq.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rqlhzsdp.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2upsjlcse.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2fwngaczi.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2enoslusd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2vcbxopyo.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ceepyqki.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ftfaaant.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2xbpwpyoi.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nygddgxt.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2woiphgky.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2vtngfqgj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2ywnlwchi.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2dbftkgju.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2wyrfdwne.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2rrlwresv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2iyzkkqvn.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2oczgumsk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2khqnyctu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2tjihmctz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2inldkvpu.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2efhsievo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xhernmhj.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2fwjksmht.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2kiixshul.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2fknylzsj.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xbhwxobg.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2aqfkdkdr.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2imlqixgu.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2javkxpus.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2pqakxpgi.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2kuykbnog.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2wdewbyjv.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2qfoavsan.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2ujwlmncc.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2bputhccc.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aezxbsme.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ujleqske.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2znszfpne.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2klpseudj.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2fjqmnhue.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2lrlmqsdq.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2nwemnxbl.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qfulskcs.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ihjgvvzp.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2uecqayah.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2smehaaxm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2soxlswdk.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2mgeizuzl.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2tvkxjyjc.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2skdtawty.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2fiykislh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2rkzqdbfx.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ntdiajuj.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2msuhvycq.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2gkgwhwpy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2hclyjmha.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ofprixqc.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2fzenzycf.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2yvnanpfa.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2jtzvmric.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tktybpri.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kekvimda.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2zbmeqyaa.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ggiravdk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2qvufjqnj.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2acogymla.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2dsbvhihu.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2oliaahun.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2aelhviyo.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2iiybzxvd.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2bzskcndv.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2mvxkyubt.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2thmgkgrl.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2mmeaifab.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2dmlmhciu.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2zyajfnvf.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2rnzqcszm.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2eljgecpq.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2pstymvwv.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vnbsgyoi.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2bjdqcwuo.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2darsbkpp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2zvvvmdil.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2qfslaqaz.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2zghcgrbj.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2pibyspci.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2bunpijin.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2awlwweiq.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2pyrkmadd.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2rtifisjg.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2yblrdmsi.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2ethblfaw.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2ptykwkzd.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2jagxxcvr.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2gfnruylj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2vodogaam.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2xnodasrd.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2frrrvvkg.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2oazeuije.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2smomeiik.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2qmodmrkd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2uzwskulu.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2nzoxpsad.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2jtcfcpka.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2czqslacq.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2kawemyzp.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2iwzwzafz.html


<!-- 参考信息 -->