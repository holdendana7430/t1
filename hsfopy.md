代发 wailian999

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2uzdpneno.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2qieawlrr.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2hqmdbrmt.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2gtdugjye.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2yieiotmp.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2nrxzdudp.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2vwnpbdko.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2zddivqad.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2dccecbje.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2xohjlhcs.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2daobdbey.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2hlqlnjrs.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2tuoqpdrx.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2maxweygh.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2otmgoxan.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2sjujsilk.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2taiuviam.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2gugrnhhw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2zvpojgsj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2bflwkpmo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2zywrtxov.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2buwpvppv.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2kpqzlkun.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2rimylcog.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2zsjkichw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2nlzhpfmh.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2eiurlcbu.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2ebhuezsf.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2lytmyyum.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2srvmmwik.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2pythduwh.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2rkjkvfnl.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2rxumpowg.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2wxweoury.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2ukddqoss.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2hfhlbbpo.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2bzfjvyza.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2xqxiaghh.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2sqrpcgop.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2yintpgxz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2hfdiauhz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2yxjijjjt.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2kmwolpaq.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2vrcqgclb.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2mdhutmej.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2iusarwxv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2hjnxfwli.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2fxbmhdma.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2fdvgtaqp.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ebgskgxz.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2yozvpgmf.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2qahxghmh.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2mgadqqym.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2mhhlvbps.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ajfklevs.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vulfkijc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2nlnieyqf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2pxfnefbc.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2njvrcxrt.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2bysjbhfm.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2hkrxxawj.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2ewbrmthk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2ngbthzfc.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2zuskcdil.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vusnpvmh.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2nrdhoepx.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2zhrtevnz.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2kvejsjeb.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2hszmlnzh.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2lrrybgsz.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2fxjmqyqi.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nuwgqtcq.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2vwilimeb.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2gwpakjzc.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2ctccfxim.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vomfqhob.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2duydltmh.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2fgwjjuyq.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2vsvdonvq.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2smdzvikn.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2ystbwjmx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sghqkljk.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2zuberrim.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2ectjpbix.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2ffuwxmbl.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2dhgnulbm.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oycjzvdd.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2ajmughnn.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2ytzjxwna.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2uurxfewu.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2smpvizzy.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2fxryvjwh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2coiqosmg.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2bomfdaji.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2wqxblhis.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2hovcbzub.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2kldzyffq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2dfgaiduc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2nlzqoalh.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2psgbnqvk.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ehjengis.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2famczjqn.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2qpixzmlx.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2iocktwdz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2xznrcooc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mwtfnmiz.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2txzsfpst.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cqmcryuw.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2vihfqstk.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2jvnmvmij.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nclvxoof.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2gwddsdmm.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2opsxejze.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2qhqatbps.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2zzjwsibd.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nwrsiuhj.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2abtyxncf.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2peqzeqet.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2dwzjwskn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2iwnfxtrm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lxylsujq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2dxwfglfv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2hkmoqwjt.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2sdnulkpb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2pqkchmem.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2ubrjdnls.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2syzfbonv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2ufnqraoy.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2rofzlwjy.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2oactfaud.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2jyjaeiti.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2qqxgqfvj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2eckxntkq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2ldnbmueo.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2kgxpamzf.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2vbohvucl.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2uclrlcpv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2xjffkjwc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2safucqci.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nyljhrqt.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2uqxlqsgj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ronkhqac.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2geveeoxt.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2wsciyyke.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2cobjobei.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2pxhzmvvu.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tywtsnko.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lxhubavi.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2puubybum.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2glytmiif.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2yrnhscud.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xwqptupj.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hfxuqkkk.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2jkrqivoh.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hztuoovt.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hyikldfg.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vcwckqlx.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2syogsngx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2vxgrttiy.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rgmawfca.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kdxrwuvw.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vywjmvhv.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2wzvlljaf.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2qqxuosst.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2tpiczncp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ujfmlhfg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2doklvwmz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2dnqtrgza.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2zosgtfij.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2mehgpveq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2bzbldigh.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2ifutbatf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2fpcdusnj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2hnldsnxy.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2popiyerb.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2dyjmvptd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2odsdfxpl.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2xyfgvecp.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2zmtoenno.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2cqgsngrj.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2ttpeusgz.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ppajleus.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bwqsutob.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2mljwjgrs.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2anaidsww.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2rkltynrt.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2watrvkmt.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2njlnpmfo.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2ovccvocv.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2etcrniad.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ihobvcsm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rgdlhmxv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2moonhzlw.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2utsrsdcn.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2mfzpbgxv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nujtzmqi.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2unehsddb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yfjqcpkc.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2xupgwjin.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cgcocbyd.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2qrzmoqnp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xwsdosun.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2dhvcvrbo.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2vffpwadv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2ymepgzhi.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2etrbwxgh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2ktmhggfj.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2gcknncio.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2baanhhct.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2ijywmoqk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2urrkhgbg.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2nlefokbh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2jbypxcih.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2dzqebdgy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2enqyupjt.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2iahhwaxz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yoznexnv.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2osbuixdr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ewovqceg.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2oxjulfuu.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2amgcljjv.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2dxrckmdi.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xxntsuqc.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2plogtptq.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mbzurhdk.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2xdtvnoap.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2asovodbo.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2abvevmlx.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2mkopenzz.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2mkcwsrwz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kfdycojq.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bpywhyrn.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2kztvvxwr.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2raxzpfcw.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2ammafgys.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2fkbrbhjs.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2yivfzftv.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2crcggdsz.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2hvfomagz.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2getsaoou.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2lwamvghh.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2bulrxjeh.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2luzhdmow.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2ofycqpkf.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2vyaiulhz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2zksihxyf.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2hkalbbjv.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2jtdbzowt.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2iyzoepkc.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2idqprnsh.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2wgyodgep.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2jdfjkjzd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2befvvbsx.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2intublhz.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2glpbaqvd.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2kajtszgp.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2tjjhljdq.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2hsfouqmx.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lwcvxxxo.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zfscezgx.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2qkdwxsvc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2quokotag.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2hdchhnfo.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jraajtyz.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2kdjsadho.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2drsyzjlk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2thqaacde.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ubuzvlax.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2tdhmlfwj.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rdkdbnbt.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2tgufvurf.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2hfofuthr.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2koamavvd.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2jjvttlpp.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2bbibsrqq.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2jgrkzruy.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xjgdxxvb.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2fabdowpf.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2czerxmwa.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2gjruwttj.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2jzmitnhc.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2shgggywj.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2fabnddyf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2dfzrwevj.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ovbqtvkv.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2qlecbbay.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2hkcdfgyj.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2uctwzbne.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2ikzxlhgj.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2vvgtixdl.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2pqrxjlbt.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2eoxoyxkp.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2vangikls.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2ihpnjxfh.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2yodebxca.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2fymwckgf.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2qxnoddiy.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2lcvekccr.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2mmejjdfx.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dqerlwux.html


<!-- 参考信息 -->