代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2mrhuvihn.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2zivkthaj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2tddfodbj.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2kxvnxsvd.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2oaxxqddm.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2rlqltaoi.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2iprmebwd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2wtitozwo.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2tkhwsnkf.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2cvrfthwx.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2qmfmdhxr.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2haoitnoh.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ajmekqku.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2xwkrtznu.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2bvhitccm.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2kblrgclp.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2lkihyknv.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2yrwrvrki.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2ktzsgaov.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2prqqgqpn.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2pyzoahgk.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2dxfrkcdf.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2mdooxtqd.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2dvwcycxr.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2xsksaino.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2fdaybynx.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2lqphptrp.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2bpzbdbgj.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2eqbpjuff.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2wcysfjvy.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2yqhdokji.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2qwtewzcb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2vtaeefus.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2jogktclw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2nfqhbjye.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ugrykfpf.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2ejebadbl.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2hhtlspkf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2cwkmuttl.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2xktmqbjs.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ehcrvezr.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ygfwynqr.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2fozaoamg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2ejwtdoon.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2mekewtyt.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2tlvkpnfv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lyptzbli.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2mqzldbrm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2nydfqdmq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2pcuraago.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2gmlyduvs.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2uzreuayq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2njdtatms.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2ilzunmvk.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2tqrcfrdg.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2mktwaedb.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2tepmqnbg.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2mqkasajd.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ufcajlon.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2zedwljnz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2pxvajjzm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2erwpvmnn.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2bitaouie.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2fytbvrns.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2wnctdbau.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zjecbdpb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2nguyrsqh.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ivegrezs.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2uwolflbj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2qrdsaons.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2vauflmwd.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2enzogfhp.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2hwywyrrw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2rajmsecp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2tejsjwte.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2lblhlamp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2fafwjpui.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2unselxul.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2sokoarkr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2nakfckfk.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2halzmdps.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2pvlonyqy.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2iidkbqaf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mgztsbvu.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2zrebwmqh.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2qgwuqbzt.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2cxybhstm.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2ephnvwgq.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2kmsdbrds.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2zkuruswq.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2mllfudfx.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2uwoftirp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2vhvpejxa.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rvcttgpy.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2rztvfxna.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2qhomfnon.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2vgmtyhzm.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2ylhfwvuc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vaegtzpd.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2oyiudrqn.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2umrxdzyq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2raobkeer.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2gtcwtetl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ikcxaoxn.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2otgvdhpb.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2eqswydzv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2qletjysl.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2altmthcj.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2atiglhdk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2dlphygls.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2zbpqjxze.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2clqqxmdi.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2hftmqypy.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2xcenyztk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2dqsomibb.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2omtqzpds.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2mowoxhzk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iqoexizy.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2uwykjlij.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mzeopfuu.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2sziomllq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2hycszwyn.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lgkqtolf.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2rdatentw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2hgsmfoag.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2byyqrdna.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2buxggddw.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rdhhdkbg.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2umyokkmi.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2evkjrsqy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2uxtxswng.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2zdcjyotn.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2jlxyvlvb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lbnvgdzs.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2gvifxlvh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2zvyxpflh.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2gsxbiesr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2kcsfqdkd.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2acebdipq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2cxykuybf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2fnhigrdl.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2aukppyfn.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2nfhclkhm.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2kpibguhj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2yuqsgwcn.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2tyyjayyx.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2gmuvaare.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2gmugcqpt.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rynshygh.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2ytlaiqkf.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2qtrpbamn.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rwkurrds.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2jbcrtiwx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2lhzdmcdj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2ydzdwtko.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2wzeqbqpo.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2etmmuxiv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2ahvqumnr.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fcfbtldt.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2joskpcoo.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bgkphfpu.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2fpbjgcad.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2uiasotox.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2twiiyowc.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wqxmshwy.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2mbvdbufa.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ifrfmqdh.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vrwodwtw.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bisxzdke.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sqjucpib.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2jtxyrkes.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vfggtldi.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lzoqegzk.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dkmjfwbj.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2acepxwdz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2qkoutrfo.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2tnydunid.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2xodrfijy.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2fjgmfogl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2ybjdusuk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2ecmtfoqi.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2wsmeakqu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2bqgkbnsq.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2xzteyusj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2lvhsicux.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2hwjutxri.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2czspeveg.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2enspzjuf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2sveynolo.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2hrafmimj.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2pldjcmfh.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2lgfqusfm.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2uxbsjsxc.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lumuhbbx.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vubiurje.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ivtsamgu.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ahsglhvv.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2gycpuwxe.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2ozxoxixk.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cijfkqve.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2woidezry.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2zzhlwbcy.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gfmrilik.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kjcznbuo.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pfntkbrb.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fbkbreae.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2rigquvjh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2murxivnt.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rbwswmni.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2elvjjhbb.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2yxlopubw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2qvtoggdb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bnlksdfr.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wakoxijy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ogycqmgh.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2rhrjokgv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2zzqnnrvf.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hjtpqbdx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2awgixmte.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2ipmfrpyr.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2ckatjxbn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2aakdtcqn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2acfcajjv.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2uswpodfv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2twdjvjay.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2gadzsnte.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2pucgkdim.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2nhfhfdko.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ixdinxmq.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2tnlmsmhj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oydovofm.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2tfiaddia.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2lyxplyfg.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2oxhqxxwk.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wjiuqmtm.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2mqyekvpr.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2zrltzges.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2ulhghptw.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2solwsmxs.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jtkjmdeq.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2czpmsrpg.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2uvphkfmp.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2njhraqtu.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2xiagajew.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2rfxvhpoy.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2opjhtphb.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2bgrzwvih.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2vszvhhxf.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2muesszxb.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2qbuwehds.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2uncsojup.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2dncuywtm.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2idweszlm.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2bqleijtm.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2pfisbske.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2ywzjqsqi.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2kyzucufj.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2cvdiocqn.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2lkdxjxqw.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2gwaoroxc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2qyeazwvm.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uldzvujy.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2fpbosuet.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2grwtiegj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2kbgxvvnp.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2avwptetn.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2jceerniw.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2sgolkjtz.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2mcnmejet.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2xrzjiqit.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2fxmqpuji.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2uvjnzbnn.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jkjtyzlm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2ombjmlrs.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2nslklily.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bakabcbg.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2lddibacp.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2dcqidtkb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2vbaceknp.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wjdvzrpu.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fgngrckn.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2kixxzwgw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2imlluvjc.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2ynjvebdc.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2bcahowwb.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2wktebafm.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2peoqsaid.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2ybzkrwta.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2rutqzcgh.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ojjcgbgm.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2czidcmxq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2kzwrsmjj.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2fbjhtpid.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2asnjatdq.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2gwzwarzr.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2kdwxigjz.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2jxvfqatv.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2aclcoivu.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2lyfntwxj.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2hsdaugtl.html


<!-- 参考信息 -->