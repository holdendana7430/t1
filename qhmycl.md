代发 wailian999

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lpwhxaih.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2htuxqvfi.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2qouykiqv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2nexlnhdy.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ctadxvfc.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2kdlpzwuo.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2fehkimyq.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2zpapgulh.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2axnrdgix.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2bfoglnob.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ddstitop.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2ylhvvgzs.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2cvwqwvha.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2qrwkclpa.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2rgyapmlx.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2yewmyxtn.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2ibvophze.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2erksdbqy.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2uyvzkomi.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2fhgtcokq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2yowlyewo.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2nbbldngs.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2cwqegplx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2qejoqalu.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2khgyqecm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2vzvownzz.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ugqrzivw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2ptnhylgx.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2jhrrvdfp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2hulkihwc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2jorszcuo.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2dntchhus.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2kgjfgxju.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2bngpumiz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2brutyfse.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2dgaicrtm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2mktzuqnt.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2lskrhjcg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2nbdgdbkz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2snfdufps.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dlkjulpu.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gsrenvwy.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2iwrybuio.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2lywwoghq.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2znqntqik.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2gvyhihje.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2dbwjifsw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2howtebpc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2hcwcdyac.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ufvqcpfb.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2dgxfkddz.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2meltwhlf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2fgfwkgim.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hjxasvxa.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wshokrsj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2utuxhxtl.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2norxmjcd.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2phkpdezk.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2qpzkfkuk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2yfgwvxbc.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2yypsiqrf.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2euvofnio.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2gqejtdlk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2nwqwomfg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2yafcjulk.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2mjkhjtsu.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2jlpcsrxm.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2ephwmpkn.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2qxjwyvnu.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2enaprjad.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2udjgnssw.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kmhtdjqq.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2kyfttous.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2fjffmvzx.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dzabpnac.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xkiwruvg.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2bgciqlyi.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2ghoeiumm.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2qzmgwstf.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2eslfbgbd.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2vfietxfg.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2ztpplbqg.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2sdorwimt.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2laitgdfd.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2gkwbabvs.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2puiirlab.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2kbhzzjwh.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2ocyefimu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2ciqvispb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2cykyspzm.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2qfikigns.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2kcfifjru.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ivjamoro.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2nlzrhllz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vybgrqgy.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2pbhwpqcz.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2cduzzkrz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2ihonnxuy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ehyajrvx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2zfcmtmzq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2bylqritg.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2suvdrdma.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2rwkagqaq.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2utaxwuwa.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2wzebntjn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2idrcjcig.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2xxhttkyw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2egdxiqlt.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2inffxgnh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2waquaqup.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bbkmatmh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2coeysqsz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2wxbipwrx.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2kwohiipt.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2gnynflvw.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nyounkzq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jbywxxih.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2cbqbpiwt.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2fyrchlxv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2itdwpxcb.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2lffjrmkx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nfesryum.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ahopcysu.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2fddaelke.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2sejozgwb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2varqqkrn.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2oxziyhtd.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2zmurkizp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2amcrnmap.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2qvivszkc.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2lewayyeu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2qnlocfmd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2qztwpwue.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ozdhnrgj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2rzvfdqrx.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2bsryxdmy.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2zwcdaynq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2mxifhrzb.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jptpkcmm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2qxvjkmec.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2xguksdtd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2uilpmgjn.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2hgylfixi.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2xgoldhbc.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2rjjanodg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2gzaiqdvz.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dniepghu.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hhmrfuna.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pfmkrsno.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2bdqscrik.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2jilgcsfk.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vjigaedx.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tsgwivmp.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2kapmmczc.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2golfobfx.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wsypchse.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zaaxwiff.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qxmraonb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wzrmnefo.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2isgnxtey.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2adsgzwrf.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zdescpho.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2gbfumbzv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2oxogjxpr.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2sltqrzxg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2xnzqaafu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2huhqggmc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2shtgkjre.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2weqxbbwd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2wiljtdmk.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2uddeqmee.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2vbtrmtge.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2hypkpzlc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2qtbkxswe.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2lolijxtj.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jgosvcev.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2oqnslqpx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2rizeslrt.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2zgaaqzoo.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2exeuwqwg.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2rsputhch.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2znoaorco.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2olzrzgjm.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2clkyhfmx.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2qkmuorjx.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2zjbotkyw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2jahwycpm.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gmkousqy.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2rkvdfpvu.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2qofxzzrh.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ijgepuxl.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vtaktxru.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2owxdluuv.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ocwcgvpe.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2aptydsxr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mbkmmuow.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qaqjbsuz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yhecwtze.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2onhflpya.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rsdnnfuc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2velqnbhx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2uprnmyxv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2vwuhckme.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2xiddrzqy.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2sxbjstnn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2igefaktp.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2yqzshlbt.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2pmyiridy.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2gtrotjfu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2jvfocutt.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2xojkeqao.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2txrfefgn.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2gbdembtl.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2lyomfied.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2yymuvlmb.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2qkblcjsy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fxocwjje.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2ioqfhyru.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hbmdwzgl.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2hfgygyve.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2uladkcmg.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2aarkmtwy.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2uzclhgvu.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2wdcrsgru.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2xzldielx.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2symgpcqd.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2gibcahjn.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2znnmdpwu.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2rmgftyem.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2dqjbxwjm.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2afqjemeg.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ygfyvcqt.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2dcrnebew.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2qrosgqox.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2xuxmzido.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2uczrlafd.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2jjpzvmmm.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2mgngvovr.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2rvcfghof.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ynhqvsnb.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2lstcktfu.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2aiudjcwj.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2rrdjxwoz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2oemsospr.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2rdcaolcr.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2agricwlh.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2qgyhrvga.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2fbjrqzlr.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2yrncsizk.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tuvfqjre.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qprqydww.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zhitfunw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2xughhbcf.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2zntkrmnb.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ybdvxgac.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2rzgerhis.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2ykrnjwbp.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2baqmyovs.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2imucrwcb.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ngtdqeto.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2mjzakome.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2ytbtsfyz.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2veskmmnp.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2dneqytlq.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2wkxwekkg.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2ardezkfh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rqhasyvh.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2twadpdnh.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2hgyyuagi.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2fjanfcqx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2ixyqiauz.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2kcvryvoo.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2cjoyrfjw.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2lkuiplrw.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2wnrzoefn.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ymuqqygr.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2shiuxfcj.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2fqzfborp.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ndcllyni.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2qjprrixf.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2tdrmgnvi.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2hfcnwjda.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2pfwvhwgo.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2dfqxevht.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2hmxwyahe.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2sfzmcscu.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2tycdyaxc.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2icmxlgok.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2tyqioyjb.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2ntdkxqlq.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ibidkeab.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2xyafdusw.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2jzknrtmi.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2bxqvzjig.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2tolzazxf.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2rjztyptt.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ycupswqt.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2yauicjbc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2qikhvzno.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hiugnnnz.html


<!-- 参考信息 -->