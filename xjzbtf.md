代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2jzjjrecr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2qtlbflpe.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2ptulnzwo.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2eyjpjrty.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2eisyrcvi.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2jdmxcwye.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2oayqxwop.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2uavcdpug.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2dnbfbaqm.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pgygupol.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2wudrvvoj.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2depbkqgl.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2yxoofblb.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hhirnvvx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2iwebnqze.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2tmslbrfq.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2panonywo.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ufuduobp.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2genjuivv.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2tffjtcts.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2bxopulaf.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2wmxiemkx.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2eusqxwmv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2kdrqhaal.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2vuaaqozr.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2axvwklir.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2zcjlocno.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2jjvsrwtv.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2bdnehsgo.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2ltkxyrnl.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2uqyvusew.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2xexcpuxf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2pvalgvwe.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2didsqavq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2swlqxmwu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2lwlhjmew.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2gbqygjfp.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2ewaufoiv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2xpvmifmn.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2pkangibx.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uirspkbo.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2bdbowqzg.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2ogdtdnbs.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2tzravkja.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ufbtatzx.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2vqnydqde.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rrxctjxf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2fnadidva.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2amegrrcs.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2cxpbfujb.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2vgrlpphx.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2leicypxv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2urnqcnbs.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2drfjuoiv.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2yersomwk.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2rnlhxtop.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2lqmcvwnk.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2fasuwzim.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2wxirvdai.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2igvbktqh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2irwdcrjn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2ajyclrmn.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2mexgioqr.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2pkqxwaxw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2acdoyjqw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ylnoeucm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2syzpixcr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2icqbngbx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bhlkwvmy.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2ghywxwbd.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2uoyrhuzx.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2pqsqgljo.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2slprlboh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2wuejdwui.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2euesiirn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2bxecocqc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2vwveljqh.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2brkwkssl.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2dcsjzqfo.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2hgzxjxep.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2fvldltxg.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2yzwfimku.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2vfkpdyus.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2vualvbfz.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2xuclzbqg.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2egknzura.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2favrjvtc.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2ujguxrit.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2cvxbnapq.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2ecdimxwq.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2qncsmdzs.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2urgygtrg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2mhcvgpdy.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pkpaohwy.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2mwzeqptr.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2lxrgqeks.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2iwhmafkz.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2yvhpmmyn.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xirzewvq.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2vmjqiryt.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2zousdkwl.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2mdwchigu.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hqqmnowy.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2loiqbeoo.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2yygoyulx.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2djkmqwch.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2rutazzkh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2fawtrtdp.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2kjfbozau.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2jlqdfhyj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2abrhbvbn.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ngacmfnc.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2nvqfhkas.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2gzlznkfv.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2ilwvgxzx.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2zidyibug.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2lbxezisq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qwjwgupm.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2bvpbcpkc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2emzsavgd.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2rgjgonke.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2eodxzafy.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2simfyifm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2tqefjywx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2haozkvth.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ycvtkmvg.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2opejteuc.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2givflwcd.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vujhrimr.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2qopnjqbg.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2holvccgd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2swjinqlz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hpmzgvvx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yxgsgivq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2hvhfzdfq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2zghmkleo.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2pscsyywh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2hemxwqys.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2iiftoomi.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2vspbdhwx.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2xyxzesab.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2klgfzamc.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2nswcpjeb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2vijixtlt.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2cjstodzs.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2cacsjigk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2udrmhcqc.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2ujpmwgqt.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2cfhxzdwr.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2fhzmqfxx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2bxunfhox.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2hbvrdlyq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2uepgbkuf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2txmiemzm.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2uugcfvxs.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2cwioreka.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2mghaeunu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2gmgzoqzx.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xqyqxcvy.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bccstecx.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bvbgdefv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2alykqwwo.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2igrwhuif.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ysfbhgno.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rijoyift.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2uuwyogzf.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pbfpjews.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2erhxhpam.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tslvgcjz.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hhnaxjzl.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2aasethyr.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nhaauwku.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zcaenluj.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tizsycuo.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2itizwgyg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2egfyusbz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2ijppjnol.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2rgbyjsbz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2ghbtxrxp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2fpcxvhde.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2poojnukg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2iwjzvtuw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2rlbyccel.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2uhxdrizc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2clakwdwb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2omcsufds.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2cyqhhuol.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2goyctyoq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2iidrfokg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2aaupyqup.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2npfgknob.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2ypdsbwdh.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2mhqnpqzy.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qorgrqsq.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fngmebbh.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2pybcsfqk.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2abxgjcri.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2yplemllt.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2qfdyonlr.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2snjkwqxh.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2vyolipvf.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2oxhtciye.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zozxugpp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jwnqmqzo.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ynnbegsh.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dlqfslbu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2ulufwuqq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tjneyvcz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bmmcexnp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zjkkrkby.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2goxlsqou.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ntdcjjqv.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2ptjhtwnp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lhykqydl.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ieejoxjn.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2knxpgbvv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2wdwxckqi.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2lbthzxpz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2zwpljprm.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2gzddjukr.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2catnezzz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2tuwsbxya.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2hydyqwiu.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2sbnusrxx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2ewycdnry.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2dldkwbmj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2tlcpbuin.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2vphnspjh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2spuwvjaa.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2fqnthqxu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2whhvoxez.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2wbgkgcbx.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2qouqwzir.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zbgoqoap.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2qsojizak.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2bjalzxgz.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2npdqwthm.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2fvxmwjol.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2egrmdzft.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2idpkoaae.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ttznjetg.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2dxhrbotb.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ssalspzn.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2zjrzzqav.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pdfpuwah.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2szihjqur.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2meesibjp.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2irrkzysm.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2djozlchh.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2zmbuagaf.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2sfqhkega.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2gmcyuoav.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2uvnqqpyp.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ompxpmmr.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2lwhnelzt.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2gmbaajgr.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2qoudydrc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2bkotyczv.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2wpmdgrip.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2fxaonbeb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2xpmxtlba.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2coccbpkk.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gvrgsums.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2giwkdkha.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2oxxnumra.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2rimtaayy.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2tqmvcbrd.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2detdgpxb.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2indfkolq.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2otzzjpyf.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dgeuerdw.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2xmznkhqp.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qxuvuqzx.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2xmmyikyc.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2yvnwmdre.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qrxrwheu.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2akwwopej.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2eqhjuwgb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ksieeiop.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xjxaooly.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dhecbacb.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pjbwqjhj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2ujyjbaai.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2iinmiwpn.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2ssospflm.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2uhneyyck.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2wrdqntzn.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ekvydbko.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2lsrzwmfs.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ejardokd.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ssqlyvlx.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2ewolppyb.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2kjnxicwb.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2cesmmalh.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2bzojsepb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2abeokdwn.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2lcaxzsha.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2mxyrdpqd.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2xbxtulhn.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2myysxoem.html


<!-- 参考信息 -->