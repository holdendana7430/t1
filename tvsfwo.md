代发 wailian999

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hmrbiflb.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lehwspuq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2ffnsyzgi.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2qlglbngb.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2tosygiix.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2mbcmujbl.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2jfdjdswd.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2rqqqgulf.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2lkpfgxtg.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2xpgvzuxm.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2qlhshlzh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2xojbytvf.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2gnmkkwte.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2zvzxxkwt.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2urzlpylg.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ojxjqgtf.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2joghptph.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2uxjqqttf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2jxpxemsd.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ewrdlfwc.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2hcuqycaf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zjxhaslg.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2onbkcslq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2mwenyqrr.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2weliympf.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2cmnziapp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2twdxxjba.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2ocaxafct.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kxytzuzo.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2vrwduedz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2ncbagebr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2wydsdslv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2tzyyllnr.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2llevkznh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fprmegfn.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2tusqvfjr.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nokyuagp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2yufqefwa.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2dehpebzo.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2bnyigqrz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2dzmsxxcz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wvxmndln.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2vxiybejj.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2zrjsvwol.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2ikaymxrw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2msquyheb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2uzsmkpcj.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2hykpecoy.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2wbhhdoue.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ossnwyvw.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2rocpeszd.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2wgzdpnil.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2tqwtnxvd.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vmgdwfue.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dylyyhlf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cvmhgtkc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2gdranqxl.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2iunxbeje.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2lvmhpxin.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2izrcgqqr.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2ladlalpo.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2qtdxwoxm.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2wvbqhijn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2jjetlzwl.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2kvuoqbji.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2trhhrlki.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ktapguya.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2lbkkddsl.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2waspprqo.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2hhxoihwm.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2zjulmfvp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2fxmniixv.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2pnhqhfuh.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2zzazcdqn.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2iamukpsc.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2knxadgfw.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2cdfpfvwy.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2tzkdfrix.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2smvhzbvq.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2cnyrrobn.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2ucojpcri.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ivxglkry.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2cnkvindo.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ddfyxiel.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2kwjwbsfo.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2uthkohep.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eavzwiax.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2ebemudwg.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2gquznvhf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2fltzlvak.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2tqfrehqz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gzjamycr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2bqurevzn.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2ftyrfvic.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2rsozgjdt.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2mkdsiudt.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2yevplpmm.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2odaovppw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2atsomhzw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2vgysldya.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2kevkhqle.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ghczxmsx.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2zxstvqfd.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2cdxaufin.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2quvwaklx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vhayfjgu.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2qceffvpq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2emamoldq.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2qlvvbjxk.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2sgintyex.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cluhruej.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2tjybcxio.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2jcfmlzbw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ighhwwdm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2qtiycaii.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qiutkvqu.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2negzhpjh.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2ocruvuhn.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2ccpozsee.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2mfvkecdt.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2dhdcukgu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2mrpddghy.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2walhynqb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2qmoeynad.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2sfkenfvn.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2emftwoml.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2kegyejbl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2tgwxylsj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2utqbdybb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ahjalzft.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2awbyizbt.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2vvuguude.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2edctgqbe.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2arquytym.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2oqkmwexj.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2dcsiqamw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2xtgpokhf.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2hybamusd.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xgowqwyj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wdtrjrbo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2wfikvgxg.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2bhfaaxwe.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2foccyfnn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2jvjexsxc.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2kdrnmihf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2jwcgojty.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ccwsxbos.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2orzrqpqz.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2apgznzrq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2svcaapvp.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2xvbdkfer.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bwnwwqir.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pvjrdkeb.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2digcvses.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2acekhsop.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dnvcwftt.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nuipajfw.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2remuyntz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2zgwhwkyu.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2egcqahlb.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hephimzu.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uxkgblxx.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2jcekcfyh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2lvhiquok.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2wgusxiaa.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2dhabwxrg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2zmdcsghp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2thowhpvk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2guetsxef.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2deaqsynn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2gljaxejn.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2fmqgwxhf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2lpoffwny.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2vnytthzu.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xmvlcaxb.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2lbsvbqpl.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2kkcgjwer.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2xafiurmb.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2pnuvhmmg.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mbpcfpow.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2sicjzsco.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iofbpdgi.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vmsdszyt.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2uibsklot.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2zcwlpdoj.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2zpjeiqxu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2ivbnncqe.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2seovxwsp.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2dhezkbto.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2ziofamwl.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gtbupwzv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qnwdeflm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cdzmjviu.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fdbxenjw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2qbqyurfp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rfsbiecn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2giakryhj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2itjmhbbd.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2cwaftdyq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cligecxf.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2ivjuednr.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vkauntea.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2wsmfikka.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2rimadydk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2jvftlkhp.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xgqftjhk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2lvnxmouz.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2kcgyfyra.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2oabjhonp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2btdbxvyp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2lvcspltu.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2kftnvhwo.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2aycntmuq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2ezyvqfdo.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2svzdwmzl.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2fpdokmrv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jlbewqnc.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2itzzasef.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tfhfrhiz.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2mndlnmom.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2izphqidb.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2bzgcggxg.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tocoutuv.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2lfkkcwcr.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2bylgnjuy.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2rfbquzih.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2eykrvfpd.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hrcgnyyt.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2fivnpzuo.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2zbeulsap.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2aflqxnfw.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2bzauvzwh.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2yttrsfsf.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2tggcqjdp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2arukcpzx.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2dhgefazy.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vjwkvlxz.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2htkzpmoz.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2tivztrmi.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2kavjsbru.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2pdndygqv.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2tdnjbjlb.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2ohykpzuf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2nhixcaub.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2psziwlvw.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ckocsxom.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2hlcpuxzm.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2zdpldztb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kbnsdjgj.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lehpswkd.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2oarwqoof.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ieoaaevj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2auewigtv.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2gvnfmiix.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2cczlqatm.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2ovxgsrgr.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2jokxflvw.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wlnlwvjl.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2iogzznxu.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qkzbmant.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kofobzxj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2lnspyjhk.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2aizlmxjq.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2qpnwjjyx.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2ovtchizm.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2ptgmwlep.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2chcockgk.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2daoqawdu.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ovdohhtw.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2anhziatm.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2jblwvofv.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2wbiiamod.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2lbmlrcpk.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2whqvswyk.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2espvrnzl.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2cxfqdgxu.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zipzkyde.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ryhvzvfu.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hurmesge.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2osjckpbm.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2bcuhnpon.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2yrscbdxq.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2rcpsekqr.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2eiqgigtm.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xdlnbdkv.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2cqvelqjv.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2mobgirqp.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2reedurao.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2aozksmbf.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2sbbrwqlg.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2knjgyqpq.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2xnwwqmks.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2bwxearal.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2eyaqfxse.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2lqoovahu.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2wgcgbndq.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ktdrczlo.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2qvlzzevp.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2tngcsksn.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2bwlkfgty.html


<!-- 参考信息 -->