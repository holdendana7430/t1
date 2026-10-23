代发 wailian999

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3plgbttsc.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3suavbwlu.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3scujxqho.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3jeuqwigp.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3osdwloay.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3bniymjxk.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3jrwsxrww.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3snbexasz.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3rwwuycqr.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3iislonvk.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3lbpcqevi.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3tgwimqlg.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3uifdxfhk.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3sjzatwrr.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3bjzxcwdi.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tnnedhqv.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3hwcqodiy.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3zddkifrr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3yalmihpw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3lrqbaaer.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3pvmvnkno.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ghdhqjat.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3wseahcmp.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ezzxhhwp.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3kcodzmdq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3bcrkmhtx.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3xyanoqyj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3ettcviue.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bgusmaff.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3upqiedbb.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3pniwqhya.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3mkfeqtei.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3bpednqvn.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3ijgwjvlk.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bvuwogoz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pptkuxbn.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ljyomhpe.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3xrfiypxi.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3tumdphry.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3uilheuza.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qjyoyvzq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3jxksdpsd.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3mtsqkbly.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3hxsmmnxm.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3ekzlgabf.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3ethqgcwz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3jcjoddml.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3chfeyksy.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3wvueguzn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3cnbqooff.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3swbtuufz.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3vffndcxl.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3pezimaxx.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3pqitbyqn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ekmokauc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ojislebe.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3xgjqmdri.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3gnhprsnp.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3fqelvycb.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3npmpajre.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3ghjegnph.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3ojwquskn.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3uqnudwgp.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3szkokqkt.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3zwzollwh.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ovkxdfxh.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ijokmtuh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3sjlqcpoh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3zlmflgko.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3pifhqdci.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3yyfxyqzj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vkctprrs.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3tibyroms.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3fjybthcm.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3eyktlqug.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3kihhcekp.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3untsipiy.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3yncpnpjl.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3jolgnsrj.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3tafwwnkc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3qehhyaut.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ksxusugd.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3hxyjsytd.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ejgigkum.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3nvvhekxe.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3bfjjlzty.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3zrhbppuv.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3glnmgxvw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3pfmlgmrx.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3cncbziof.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3pggvwcwm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3keukbhww.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3saqsjxyn.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3mebjmtgp.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ippzcozq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3dkbnoxpm.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3mmombnyj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zqjtvqxe.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ldvpqwcy.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3kecedsqb.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ayinehcb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3rbxnmphs.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3mdzjkxhh.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3puvbtgzb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ezpkhrkg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lsoekkrg.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3yckfblro.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ntrmhnkc.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3ginbbkpl.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3ukwjmgem.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wiihtoyb.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3gvsvsect.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3oeqwvsyl.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3kriexeeb.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3wmihfdet.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hncsembs.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dxzktyix.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3qjomqtgz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3vmbwtxog.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ditbixwm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lmmwgbeg.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mwcpbkus.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3yiecwpja.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3opafubot.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3yqchvhmi.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3dwjbbhxb.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3oudtaick.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3fguuprdv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3zzpeefjx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3vjovjwhf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3vpspcoyg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3hflvbwcm.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3hwlvexws.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3qtxlweir.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3mcnqsmpc.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3zghpirkt.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3pnuzjarl.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3fhowevtl.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3mmgpdthp.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mtphsper.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3exezqctg.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rigbsbzr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3ogzquaxt.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3bdkjflsc.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3odtmksne.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3fxqpvsqa.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3eznaeouj.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ebqczdch.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qntiqccf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3siyamhhx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3gsbubxro.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qhefclev.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ddcwxggr.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3vwsnlbhw.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qqcbryzw.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qtxgrmmt.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rstnowlu.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sstbwlzg.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ngduwqma.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rwvsvjik.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yqmsazpy.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3urzwsjhs.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3fwkzodui.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3fhohvduu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3kpfstvsw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3qvokdzey.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3hsigxbtv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3dxmqqjsh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3hwardaby.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3rlnikczp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3wvbgrjyi.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3vhcsrphn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3gsqzuzys.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3brinluig.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3vyztjemc.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3rhvngznr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3elsdunpk.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3shmnqrpj.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3puetwdwp.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3pewhiusl.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3lgcuqwyg.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xkjrgnvp.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qxhuhaub.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3gcnbasvk.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3rnjqssyc.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3loduimcu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3rbkycxwv.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vpeiylnx.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3twruutqs.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3otmyfdie.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hsntpizw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vhdracph.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mjbpklyd.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qfctcswp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3svghyqkg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3phkxoque.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sbpnvgyd.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zycablqx.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3btkxwzgc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xpcrmjwx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uvyqbsqm.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3scamguiw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wdmsrrmn.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3gupoxjlg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3hwiwosiz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hqhzqvfx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3iislzcym.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3whpzdsaa.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3lbcvsrpn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3cvvvwfmv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3fbkhlyyn.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3vyrrzoxt.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3vpegnoek.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3cimajkcn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3oiphjldb.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3jiragujc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tgfwxclb.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3jbnelrfb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ahgvtkxs.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3wvkiupok.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3bjytyglr.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cdkmhqsa.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ugupefux.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3ccqhklxd.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3aycpkhml.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3duslmyqk.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3qpwheqbu.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3qlyvglge.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3htavezmq.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3zlvvfmhn.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mrogzfpk.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pzwkghji.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bwyronsv.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tkkjcqvw.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3xlrxnzty.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3ayjfvgdc.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3xseftffh.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3wkchhtek.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3xdzcvgyc.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ydbimkho.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3yoaisbon.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3wfhbycpo.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3pelwllep.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3gzahrnyf.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3htqcwwsw.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3yxgelfrs.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3bqnthrew.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3kypajnrg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qjiacrgq.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3lmbkqmsr.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pbpswazm.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vnvzykrm.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3xtwulfmx.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3bqqzivls.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3aegxynpj.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3qgfdzsuj.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3yuoetixa.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3rkgdteac.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3qfithfwr.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ojntvzwo.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fldhbimu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3pzvdyvtc.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3bbrfohye.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vbpmbxxk.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3bqmfgpel.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3rraezkke.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rxcwhket.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nngvpmax.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uftdagxp.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nmajxufi.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3bufncrdo.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3exdvgzqu.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3kxocqxzt.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3vdmbtcwv.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3qzvjsvyr.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wkqbsonm.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xzefazll.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3cmpwckxs.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3kuqgdxrc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3nnhpcbxt.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3wfysroll.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ranmuaci.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3uehbvtae.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3gvyztegt.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3vuobigye.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3vdmbvpdm.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3wqydexok.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3vncxsfqu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3qfuseswx.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3phsfuumj.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3wxddpwlc.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3llsiunwx.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3klnfpggk.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3kugdrxqi.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3ipnqsvxb.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3bpzlhnxc.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sqmtuowi.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3ocyxaake.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3rncbnjjj.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3aodrjytp.html


<!-- 参考信息 -->