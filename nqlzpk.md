代发 wailian999

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3ipvwvsfk.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ostyhkrh.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3mockyfyq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3hvdopwuy.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3vhdjpspx.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3tizqhiuh.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3hnyraasi.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3anbivgou.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3gwmnupur.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3fpkecbnw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3xzmxjsga.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3tjnixill.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3bnimyzwj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pgbidraw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3lcpbwusv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3rxqjiyrh.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3difboech.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3komfperb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xxbxxunz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3ifblvvuy.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3tkxbdeoq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3nwzpbzqd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3jxwelixa.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3cwplpyhd.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3pbrheqcp.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3hjghcevh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3agvfcake.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3stbrects.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3cakdxyuk.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3hrylmnwl.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3kuadozze.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vepfnexb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3wvbyvzod.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3noxmbqmx.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3rorwpoog.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3jqjrbwek.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3qrzrhadh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ugdiszpy.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3opzlvmba.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3amauksji.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3jzphgcwo.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3oengaukq.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3cfywhrgv.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3klpdgabs.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3iaqgibfz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3vchxytcx.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fttaauhl.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nribklxx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xxoplozw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3zbwnfupc.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3zakpihav.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3hijsngna.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3dtuhrxwg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3pdutuhmv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3syfdknqz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3snfinqmd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3bhenxmqk.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ouqntvew.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xcsvplpi.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3mbunariw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3kfjyzurp.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3kissmtoz.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3nfnrcheh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3neoqejws.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ckenzoxr.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3xaskcvzk.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3tmrhsoyk.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3thlrsjdp.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3mikdkdwj.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3kkmbfdep.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3mfzujmje.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3ibtklllo.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3xlxcdasm.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lyxpmhwl.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3pdbjcrzj.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ivhnniea.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3suxyfood.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3idcfhcez.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3wlnduhbd.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3iomicyho.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3igfdehbl.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3cnyizxcj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3nudvnuot.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3iuftcxot.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3wyzobtpw.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3mdpptamg.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3gqgnarip.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3nbwvuaub.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3obqnyqyn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3muloueje.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3jxoarxou.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3vfvsygcf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3xbbhjdsy.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3sjqsjpep.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3ubjfketh.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3tnbjhabh.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3mmzbogyr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3evfcecjx.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3ggfzburp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lrxxdouk.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3txewphfy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3vabfjgsu.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rrcxwapk.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3horwnvwa.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3equscfij.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ueuwnkiv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3zmpwcchw.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lbbtvons.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ometjgpp.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3xuilgpjk.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3xonmzmti.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3jjqfjyti.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3ctohxwhp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zrclialo.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3hiijrqpn.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3mixzczoz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3wxxpmhfi.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3pnwcsfws.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3ndubcfgl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3jqrzhyjv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3nbzyqghi.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3isdlnvwv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3jwnsrazm.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3izwreppe.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3pwapwctv.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3wknifmao.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3gmuyoxnh.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3bpojvzzz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3jzufruiq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3gkbhelug.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3uammnzxl.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3sedoteax.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3fuyftwuk.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3xhbaurkd.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3lzunzcrm.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3ytgjmbry.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3hvcolyjg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3kngktygi.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3reoudzvp.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ihxlltpf.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3picfunmg.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3akiwbhny.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3vnguakfm.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3axhuzpsq.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3atxmjhlf.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3yxvrjsxx.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aihljhab.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ginigxnw.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hunasqfk.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yfaooljf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3absqwfsu.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xpwxcrvf.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sttxcvwa.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3retjyaeg.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3kcuwrbbx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3mzwahetr.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ustaffrg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3nxoifsau.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3bqhjeuka.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3jusssiju.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3nrlyibgi.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3shvrczfh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3fnfwlpmv.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3ruzolofk.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3xajydzjw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3kxzwhoxm.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qlccgxki.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3cntbeplk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3bkciypvk.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ghuqpycq.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3yrmnkqpe.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3hqsxclfp.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3ysbazigs.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vbecjxbk.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3oysbogjp.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3nqtkqyni.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3gwrvimyi.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3yqwycblx.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3etlcbgcm.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lerforjb.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3aizxrdsp.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3xraxiomc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3awrwjzza.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bluqjfqt.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hvagidyu.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yebnzfup.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3vqgcxyfd.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3coewvfxe.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lzorcltz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zfelkuje.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3vlzonygt.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3egrzogkj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tpafvdfp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tcjwlmln.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3rsbticus.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3jhxelcmy.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3zhhjsaft.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3namvfact.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3ppyfbgit.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3oyiqlknq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3fkwozxhw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3gzephauu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3ocfnjikv.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3hgbmngyz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3xanldylq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3mrppqymp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3ajqlkrnx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3suxzirgv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fopzieem.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3sjpbxora.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iusgcspx.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3sizzwkqv.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3wcgvytkq.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bqvfpycp.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3aibffnpk.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3qjgedmyg.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cbhnfsla.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3pycwkdqs.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3piyfxbcd.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3nobqqwit.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3vjiikcva.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3arfdqwsv.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3macclhvd.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3xthdzufj.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sxvofpiz.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3wtalnytp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3ckocwkal.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ouperdwb.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3tjzqgccd.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3zuctndyk.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3puwmrcfn.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3amvguovz.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3kowguovn.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3mjvzghke.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3gdqsgope.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3vumcjlyo.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3fwtqiqrc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3eplepfwp.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3jthwkwms.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3iiblnjsu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3voxokrzw.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3biarfvic.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3fhbxioui.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3yphdxepv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3layffkxn.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3cxkyqouv.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3tfzgxphn.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3zazkjlhk.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3eruesuxn.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3fbraxdbv.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lgfdgrsr.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3jzpogzxr.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kssrvtfd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3eovodfjj.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3obtyvndc.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3dekczayw.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3lxlufwio.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3tvpitszr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lnoatnzu.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ddsoloha.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3imfydbtn.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rumanjpu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3axlyducj.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3qbpagvrd.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3uftgxbdm.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3nklexlrq.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3fdxivpmo.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zdfxlcxi.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3alvfrqqz.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3rxbgrrrd.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3phtdoxje.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3ckuuyhuz.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3thhswtxb.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3bhsyedpx.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3kzcfxdpr.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3twfsczcd.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3aqluyrci.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3efaqncof.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3eadqzhzs.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3havzibzv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3wycnrfbb.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3zvyeuhma.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3qwlggnyc.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3xcuymxeb.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3bjdokaij.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3tsgehgcu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3rlyxkmcc.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3uncarqgp.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nlpgykwa.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3brbhilrp.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3qilujbjs.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dzixmzwl.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3mbulujvt.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3vixsyqpp.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3kvvsiiqw.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3duvixxsz.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3tuiaiump.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3txwmnlvx.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3zpyuknpc.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3qytmtgin.html


<!-- 参考信息 -->