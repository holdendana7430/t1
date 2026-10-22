代发 wailian999

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2ecjmgnjf.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2qjcqlwtg.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2eukctrhn.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2vrhwaukw.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2ddycicjs.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2zwlwhgip.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2jppqrjho.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2xprtesuh.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2mzcftzpt.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rjxbkypu.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2bbssmphd.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2vdaazttf.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2dvtpvoza.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2pghbgwnp.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2tpnvvtrk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2yspmynwq.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2uhkdozjy.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2thlaxllh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2cejxrrii.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2rjgwizbf.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2oiplicnp.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2sgxkpbpj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2jwoxdjfz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2qrnpycpw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2ohtxdhqi.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2eqgjvpfd.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2pwjmqgwq.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ajezmudx.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lnjzjkbv.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2xfqzntcj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2dmngpdjc.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2tyfwzlic.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2cohqcbkd.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2xrcadmas.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2sfgbvayp.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2lfevuzvo.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2efvfeupp.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2owaivrto.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2ropqiwvx.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2vjhvkkmr.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2qagzxkps.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2uycldxud.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2pcfcppib.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2vbivcnas.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2gfuodncv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2egzfoubz.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2swwwdpcl.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2syhibdan.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2dijbefix.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2mrfiiseh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2elnztkqp.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2hadkcbpz.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2udpvnkuh.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2vcdvswqs.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jylqqvmc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2ykhyeurp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zocwnsmg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2rpxvvhsu.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2nxzdopmx.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2qmvxokst.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2jngaxyga.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2nvfjutzh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dtxbmlot.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2pkksidum.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2xtdmhgxz.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2rizffohw.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2shvovede.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2nacftste.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xkuivtjx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2mvgnrvhv.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2hghnbxay.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2apmfuyct.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2ekqdrwmj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2lcwgvgdr.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2pyfqgbrm.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2aboezwsk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2scaijbjv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2fuyqzovt.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2kxxksdot.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2hfbywytj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2hfvyeinn.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2nbdwipke.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2kzzylwfv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2dbjqnshd.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2owyslkis.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2bbvfnauv.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2leavdobx.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2splpdxmz.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2dsjjrdyw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2rxlrqjzw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2ynompymd.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2nuakeqcs.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2roijqhin.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2rzhqdjoa.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2idfqzwdq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2ooxhdnnt.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2bfxmbnbn.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2qvtesgny.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2vflemwzz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2rnxkzkpj.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2hvhzstvs.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2pmljrikw.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2geuifskm.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vrxenvkg.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2qqojwjvt.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2huqwamph.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2zgixpmjd.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2edxbmulv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2mofengfe.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qnwvnnsv.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2dncwzntj.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mmihwjfs.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2chqfavzq.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2wdotpgpk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2kuvshhov.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2clnxdswa.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2mtdtwhot.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2elflzxdc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2mnctcyvt.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2jvnqrmjd.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2znongmie.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2xvxcxzcb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2bxvkpcxa.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2gdupbars.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2vwciqjtf.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dsymkijn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2pfdyrxhv.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xthpyvui.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2swhuzhmh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2wqwjekvk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2krrhcbyf.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2lajadsfh.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2yqdnwuxt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zblotlfp.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2cgdviyjj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hbuwhfkn.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2qqxaswmk.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2wgkxrsvl.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xyimbhoh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2jhasfvtf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2bkremgxe.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2jhgyugvg.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2fvhxktii.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2guyxymyq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2elyvraiy.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2xkhxwhby.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2dkkhgqzx.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2thcnpmzh.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dxqobrmi.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2cvkdjgfi.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2rivnzzio.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2uzruumyk.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2jinokyyq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2hbnxvysg.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2autadypc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2dndfhfun.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2hkfxzsof.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2iahkthra.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2pveaohoc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ngnordlz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2xghzpzar.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ckbmxjhj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2xpmwemro.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2sbcpsosb.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2esyboghd.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2hbtmugsh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2unazlbza.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2dnpdcoxe.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2vucttron.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2adrxdevz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2ktgljalg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2dxhtuyyq.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2frqxcwfj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2ahfamqde.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jwwrohao.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dncomzuz.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aethajtx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2gyzenqqi.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2fkhlipjf.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tzayzatz.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ndfjbcjg.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2hrqmzifx.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mgtageso.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nrlautcv.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mbchtopz.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qxejopzc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2cbrisgqh.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dnvqxxfr.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wtoyevha.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pcwqtkdv.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2eypkmvpv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2pqvvcztj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2yodeqlfm.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2atslsnoh.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2roiwmmns.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2cdtttsxq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2vtwizfbj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2eqppuvcj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2pzzeprgt.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2bnoipzlp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2owqolydh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2injmdjmx.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2htlfqtqj.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vdqivyfp.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2upsfakof.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2wmwtsnlp.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2djbqzijj.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2kpnqnvzb.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2qcqvbzjf.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xcdbvaex.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tkaqwqgd.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2rkckrclu.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2nhuylojs.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2uinmfmeo.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2owsbwvts.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lkhbjvrq.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2kykbcmmq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2uulqqkth.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mknbkwqt.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jttrxxgt.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pgicvmmp.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zklexxvl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2yzbztbvk.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2golbinnl.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ijulvhbz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ejhmsevp.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2yclliycp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ycjoawjl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2zsdimdte.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ydstagga.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fxhpkqxd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2gqwbnwmo.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2apkryiku.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2qvepzgak.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2zqaxsvuk.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2erknowbk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2xaaizkfi.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2furvjmqq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2mmplmtln.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2pjffvhhl.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2vsbxmcam.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2qhfjfsfu.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2hxtlysqi.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2lpyfgonl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2szouzxbm.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2zexhsbsd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vtkxlszy.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2buacouma.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2cekeefjt.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2fbtirxxm.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2oppolzdd.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2zponuuhy.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2vghxwwph.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2apfmpaey.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2hmvzfrhe.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2nsjojphx.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2hqsnojsy.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2dnkvpdct.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sukksyxm.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2odsyrnyc.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2penrlvso.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2fynvrcjf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2vkbvbqrt.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2zjaradke.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2beefhljn.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2umhtowjg.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2uqsxtrho.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ipdajatb.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2dootxetj.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2qwmibqwx.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2vckqhcqw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2buralnig.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2xgsptkri.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2oaganqbp.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2kwijchiy.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2kxxddjeu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2hzarjvso.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uotmkpkv.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rntqoegq.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ealgrzgt.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2kqyiglcu.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ltasekom.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ipqaryjy.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2svuyaplh.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2kkvjxzuh.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hntdsvbo.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rxwtuuvk.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2idvoeslk.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ptjmxlds.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2lcgmsglu.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2uionifnj.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2gwcnxgoh.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2bolwpfca.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2xfqbvfpl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qehpfkop.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2chbhmhhi.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2huuptbkw.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2jvwdpgdt.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2ipzlzrym.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2sfvnfuro.html


<!-- 参考信息 -->