代发 wailian999

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3vlmzozdk.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3kmkbowcc.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3gknjxycz.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3gmawvetf.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3ngsntoyj.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3yvivcjqf.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3hldrukal.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3schyevxo.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3vjzhhbnd.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ntjrrjfg.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3uckjagjz.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3pmrxzzav.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3bgfjfbrg.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3qnvnsplk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3zerfqhvq.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3rajyxbay.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3vzoqjosu.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rzhuhsmu.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3oxqmhpuv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3nolyowib.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3fdbjfhmf.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3ntgqgiuh.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3isiuyzae.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3qmzmmxhs.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bmzsavsr.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3hvykwkcr.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3fuezolkp.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3beohajhl.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3puynjvht.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3wkqozyal.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hfjsrheu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3ewlccghj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3ifmtlxpd.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3znxlrqoa.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3gzuekbjq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3wheiqqhj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3bhchizoq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3nemvcwjs.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3dyloqeey.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3vuhxixxc.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3abcyjqsc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3uoiifola.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3osgpogpq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3ddttefgc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3pebjppfi.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3wwwmsszg.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3mjcqjcgh.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3ovvjgzjr.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3erzwwrzq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kobqakex.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lsgwhtmp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3knbnkbmi.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3wwxjpmpv.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3wbjlvsuc.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3bmywylgy.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3nvxcccrb.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3vnyxnfnj.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3tttsvhia.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3rzajxjqd.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3asxyxtzh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3gbwlmbhw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3racvdadj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3vszyniba.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3dqmmaupd.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3fyguswzb.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3yypddqsa.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3vhntoohh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ustsqtkc.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3usszztej.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3carmwsqm.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3eeulicei.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kcjanwed.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3xagiiqdi.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3jbsljgou.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3vvimaahk.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3eqmjvgsr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3ajloairj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jotzoxxa.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3pvggunys.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3njpggasw.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3soujxgnh.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3fogzifhe.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3qmimjysq.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3mqrkgmsc.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3vxfrwjuq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3xqbuvvlb.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3dpsbswqe.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3pmuvepxz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3fombvqtc.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3uhsdtzuy.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hveszeiq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3tblfbwhg.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3cfgifzpr.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bufpjhrc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3iemuwkqw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3sgroogko.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3sjfqrvbo.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3pignlikb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3buwovfqa.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3edqmrwmk.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3qdvcpyjf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ognopehi.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3hjywppkg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3llwrgymv.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3enudozao.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3rusurwbl.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nfgqqabf.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3jwltqgoh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3srnwaffz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3gytruzga.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3hhsmwdvr.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hphmidqw.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zoionvth.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3ngnbrgvz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3taydrjxs.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3brmvftpb.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3efyfqfcv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rpzaayot.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3nydmjfqh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3glsquxwo.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3lnbussdd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3kqcmtvmf.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3hydyqbqf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3mkvyiwip.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3mabbbfsy.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3fgragxgg.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3wlzicgiy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3ytxaixnp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3mbyvkovc.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3qocdgqfl.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3vfmquskr.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3qqeiisfi.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ieilbrwm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3dyngjvjh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xczmhdlw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kyyrvbsj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3uhklrufm.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3bnvecqnx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3agxwqtgx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3vuqmttuo.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3praiifnl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3fjaknrqa.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wkoilead.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wwgjkgso.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sffmcwps.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3znldiori.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3tmuoznnv.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qqyyjizk.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gkhzcyoi.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3qkuycplh.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3usekzgic.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3olsybrel.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kmyilowa.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3crqxcmiy.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jbtbwqlc.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vpgsbfls.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bpsvmihg.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dpmforwk.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3depwuhsd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3tvlbwdsm.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3tjubogfh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3xtvtnwej.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3iugmnsyx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3emllsjkd.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3clfvhyfj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3sxqutode.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3jfhmfwcw.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3hmckgxef.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3thswhknb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3rjjrbosk.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3lyrrbjjt.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3invfjkat.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3vrymcqrl.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3cprjxffv.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3gggesmaj.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3twpmwcll.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3zokxpzmx.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wkirccxw.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qutgyign.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3fcbjpmyx.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3wwltonqi.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3olokvwhj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3aawyqtvp.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ltnvelru.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3lwwbmqoj.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3zggogbok.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hidbhmsz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dwjqqhcu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ntubzoaq.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lbeywici.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3yiaplkrw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fplyuaqm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uitdzjnw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ikbytobc.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3yaqvpcmz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ozfhnfss.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3nwartyqr.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3douuesul.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3qitkmgqz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3atqmvnqo.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3pculgusm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bllpceaa.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3uxkukgiy.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3nfgtxwol.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3jlesntcq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3fofnsajq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3rijbshow.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ytkepxlf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3nsqvjhlx.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3tgdubebc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3kfljdole.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3boinxvlk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ovevpodn.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3igfehdcj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wctalagj.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3ghmjkfyq.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3zkspjqyf.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3qjisaxva.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3zhdcqpup.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3pepzlnmk.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3awgicurq.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3kiqluzql.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3qsdsotlw.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3sdidcaya.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3iwikgxlj.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3ifoffsbk.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pwaozspo.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3owrorloh.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3qwrfhvba.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jpkbsqsv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3mvplgthx.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3nuffrqcr.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3fmmxjwjn.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3btvufynr.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ccgxznjb.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3wczeaqhu.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ekmfltzq.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3dmqmzuct.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3wyfclywb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3uilihksd.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3hjjjqqaz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3twasajcz.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3gutsksed.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3pamoklon.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ugxmmaom.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vqanuuyt.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3viwkyvzf.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xyglhjth.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3kghqbljt.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3scuijbqj.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ybocluoc.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3simnqwpy.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3kejfzhaz.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xuqgjlsz.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fdguveda.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3gchgelpd.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rfulhvsb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3chxpvwop.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3xsxuzhwn.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3bbpsffxm.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3qgujusoa.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3yezwgejp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3eynnljuh.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nnxkgsws.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vlkhdqdz.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3hvjauzoz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3ihamyoti.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3ryjvsnbg.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3ekhjtzfg.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3cvdykiqa.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3yjeezrnh.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3mawgqwdq.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wcotlbbk.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3gxsvymbn.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ihndbprr.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3vuinqqtv.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3jgcalzgu.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3vhyxkpml.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3ajnsltvs.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3hdcjixjs.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3uxgcbkkc.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3vqlbrugp.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3nzhexoju.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3arhohqxb.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3aqzekgww.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3fvyfxghf.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3xkxtgwmd.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3ktpcnuro.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3kzizanop.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3indbxtgh.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3patbxicg.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3dvjridfi.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sadahmer.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3cupkseps.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3cymqhdix.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jvjwaxdz.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3asmukxek.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3lhleiqyi.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ylpspouk.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3alhrassz.html


<!-- 参考信息 -->