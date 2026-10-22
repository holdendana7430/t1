代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ziabcsbo.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2jiwshrty.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2cpaiykyu.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2dbjwvytw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2sgqjyzxp.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vpingxvu.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2cebpivmd.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kogqhuvo.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2fqptlodp.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2avqtwpbj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2rexdkhxh.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2lkredvwn.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2smobprig.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2lhvxwgzr.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2hcgarbps.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ygzvmbus.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2wtteiqbd.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2lppqxeer.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2jriasopc.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2wzocukhf.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2wajanxyw.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2qhdxqeww.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2fgoqvsbd.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2jwnrriyv.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2ezpgvfqk.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2nqsdzifs.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2thnijjqs.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2esibmani.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ibvgfoyw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ncxxoldd.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2swesohtg.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2matntoji.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2gcsllmgh.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2ffkkuwjg.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2uwbknszz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2vaoetabw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2xzjpoftw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2dgcdnrcf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2bkwunrpn.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2yjvvjktm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2nhhwxpoy.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2kwxhpmhu.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2zedsbaui.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2pxlvdjla.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2rgpuxcru.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2osnaxrnb.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2uepbtavi.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2drrxcyvv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2byzifjtv.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2pqltprqn.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2hdjeexgr.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2azcfrcxb.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2rrtvzssi.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2tvybeosi.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2haymlzve.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2tlwstshy.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2mqksfwnj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2kzmzamxg.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2uisrnjlm.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2wpiiickk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2tteqicyj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ejgcxfvc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2aeehlgwj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2fcbccxjq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2dhxqcdip.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2jewozdtx.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2zolyzcmg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2cbgebwfi.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2rywfmhkc.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2tzfllluo.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2nstejjbf.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2rwmfodca.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2sdszdfic.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2mqvfjtbi.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ifmolhon.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2siaaqqsz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2pfsvzkdi.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ykjfhsfz.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2uyfktuio.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2dodhsuqa.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2fpvlrmbz.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2ulymtlir.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2ymmzanmg.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2dcpfhjxs.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2fgypewel.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2gjfhnmym.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2mmbcdrab.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2jearpymp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2badpggda.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2zfczlyjt.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2kdrnlluy.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yqrdpvno.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2ltqkiqfm.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2dmqrjoiz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2shqzqoah.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2llvxxcwn.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2cskokgdj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2soeotglx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2kalxrgkz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2wuwgngpr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2narrfuhq.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2mdokbekq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2cvgvbaqn.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2efipznyo.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2ndlimzss.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2lzwnfane.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2wwdyzwkz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2fpijrtnc.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2pqsnxdqz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2limvuuep.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2genvkqpf.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ihlwobaq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2tynkmruu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gllptdaz.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2zrtyoraj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wahhdlzp.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2yayrrwmm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2aloekyti.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2roswowro.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2qdqgybpu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2rbhmhkbj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2gfnoenfq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2mumbmeps.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kynmqoyx.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rmvjnuwf.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2xvldrdgo.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2znbzrmvy.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ukclpbhl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wawwpdts.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ojttlwqi.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2vdzojyaz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2vozlfjqj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2uzcxhhrc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2uxlxehql.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2fbtmwziy.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2soyenulm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2rfdzdwqd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2uxhplgww.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2zwmjednc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2qffoeeig.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2tslpediw.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2moeevlrz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2hymljjey.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2miutjgvn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2kacskvvk.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2zqozstwf.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xzkhvbnv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2qyzukehf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2xreiygvo.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2iinqubuj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2cohdpaet.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2bxuqcaxl.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2bhpelvgq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2ffnsmtlc.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2haypjmiw.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mwgbidub.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hilgagzy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2lgyaxxlp.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2kbfyjpzx.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tsjfgpxj.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dixzgstj.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2mxfznkam.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ztjdjuqe.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xsrlotng.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rtzcuoiz.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bmlkrknn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2tdrczmam.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nmwawlgy.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cqoqyroo.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nsxaatlt.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2mlkdtcwo.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ztxliijj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2caxcrrmq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2numaxuou.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2lqrhbeyl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2nugvmjfc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2wdxcplon.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2kknlhqpr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2jwzsejqe.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2ooimlciv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2sudzklby.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2kkhvzuij.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2ekcviszh.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2nhazgycv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ywvnldon.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2qdoqsalc.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2onjirpzc.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2xahrplqm.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2tfzcddyy.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aofkkpdb.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uvbpbesv.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2agcdvodl.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2zpxyqphc.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2jnoohslz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2kxjhvszk.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gohrsbil.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2npzjpeyb.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2hzcvngzw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2frgtueeo.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2laaadenu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2htjaspih.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xnumtbjm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2nvyfubui.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yzfsvats.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dybvuoci.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iafgvohi.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2travwqlj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2giuevwgn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2tvcdecva.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2evyflyqb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2tiwfcntd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2nkxtgqlr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2fggsmhpn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bkuadmyo.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2slzyrmhi.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2btvwqloi.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2nwkrmebl.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2zdwqkwer.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2tmcvhgng.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2qbzqdhor.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2iylyffwv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2wyrejwva.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2lhaoityx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2hpmkhvtq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ohvjirfk.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2zmoajwza.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2buzdciwd.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2sjqqvrsx.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2cjdxhtdi.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dmvszbgl.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ydhyhzxl.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2fujezpmp.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bodrwruf.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2xfyxjrpx.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ofhaihml.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mmgyevqq.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2iinomigi.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2jxpitrrm.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2kfhpogwh.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uznxidce.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gkesyncc.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2atrifmpo.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2cuqlqlgc.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2qbifmhun.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2pnhadfuf.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2hdmskfng.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2jvkxzvdk.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2riparqdg.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2gumubfma.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2oauchyxl.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2hptkxgqn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2ttkethqa.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2zfxorfon.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2onrljnyc.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2mmjflaai.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2erfrpzvp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ykchpogh.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sngrpjpc.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wxqqdlyi.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jvppkjez.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2rpgtedgz.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2nowksoja.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2cwjahdfj.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2yuhjbfow.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2vicxkwbg.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ufcwmugx.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ucsldmam.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kghioldl.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2hozdbyoh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2pqsovcbl.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2ocmfjhqv.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2acxmaxzp.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2mlqithff.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2vawkebuo.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wauatvkn.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2tgollrdx.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hbiuiecp.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2fdjlwdac.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2ywjnfpml.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2pgeoxrtq.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2rxmpedpi.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2ogtnszhj.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2cotpldnb.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2ryaedxsi.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2rqkzuyex.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2yyaywtbp.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2fnuyrlrf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2vyqdclzg.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2vqqyumme.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2qqszuihu.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2ohbxafge.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2qhxdxvzg.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2qvzcplpk.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2uejmcyie.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2whtzdisx.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2qhnlpeha.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2nyenenbr.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2wpgessfl.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2mwnpghms.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2ctjvnghx.html


<!-- 参考信息 -->