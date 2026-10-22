代发 wailian999

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2trmqjhtz.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2nfcbclvo.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2pidkgvxo.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2ygevfxcc.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2ueqspqau.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2ndwncgpi.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2vfzjleaf.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2nrjgyomj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ibchficp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nkkdmqle.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2andfjsft.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2jwbpqhiu.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2ugwlbnvv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2rcgpbbwy.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tedczzth.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2wicigceg.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gemadkvh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2gxonjzoh.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2yoiurvus.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2ayuxahzy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2jxchbkab.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2sdmuisew.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2fktluyab.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2annpfxdc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2oxduutyp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2zxcgmtkj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2nrxgqjhq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hhkxnplb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2uanxnjlu.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2jfvilyuk.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ghewenpt.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2eatmgksw.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2dridamay.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2esjzvsdy.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2nxhdzudw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2zivfjvlu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2fqnisagq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2qxcldagp.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2jotxqwzc.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2ipjjtcic.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2vwcrlwzm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2missdsfs.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fthdlhbi.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2nmevckkz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2dyzsfrpq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2epcjwvsa.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2edyqujvl.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2nrfivrlj.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2emwfgaon.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2rukkacwc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2csvowrip.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2cgsxuofo.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2xpmausmn.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ucgerwpd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zklwamgg.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2uffivbgs.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2thijrand.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2znwhknbm.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2ppjhying.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zftmxcbm.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2afxewdog.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2vbkrfuqt.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2dtddggib.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2djxxkvmj.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2vcfpukax.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2gauiiafy.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2mrnocpil.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2uwqiqvej.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2skeromdb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bffuengx.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2cuefbbsd.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jiixevjs.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2jslrngkt.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2jldgvqvl.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uuuomtjw.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2gchzkrtv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2wrdneido.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2eeapualw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gdulkxbx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zupuxfjg.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hzsyyatx.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2bnfaqurs.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ahwkiwhh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2kyjlgnwl.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2wqswikke.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2chuthuqq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2lhanjrvl.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xnquijsr.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2aqfzpvcw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2hqreiboq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2hqukfcfb.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2zanbbprb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ishhstvp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zlknycvo.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2wleodadc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fjunckzk.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2ongodggw.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2hzerhgwy.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ebplzoof.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2qfetdjah.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2bnbfryle.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2qtjbgnbh.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2oflnqpzd.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vdicxiyj.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qpsvxhyv.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2rdjnxsaa.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2snbtqxge.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2kcmityhx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2roxxqmov.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2hyrzgbgn.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2jyjoogki.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2lmfeqazl.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2avjcyhze.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2qisffyew.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2wtkshwln.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2wvatpqoq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2nnidnwqd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ykiivdmc.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2pildlpwa.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2jdjnplom.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2fpxpoais.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2fphmiuvz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2zytrdlgj.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2ecsecyeu.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2veonkblv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2maynoscw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2druukiel.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2bzsyarot.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2xsxotqyr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2enivnllp.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2rivnfdrf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2jddwrddq.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2mezkoibv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2wrgpxpvg.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fvakkifk.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wniwchvj.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rvplorlx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2wqpcvkdi.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2rljoihwk.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tvrgkdnz.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2whcuptbp.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2tgmsgbun.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yrpvkwmb.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ugsukvfl.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ybfskrgg.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lpyscqgk.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2jtmxkowp.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2upptdtiw.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2inffmhoz.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2uroymtfi.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2jczvrgaw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2tjymwmab.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2ahrlgggr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2nmtrrshd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ngzgmcrd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2vaqzawqm.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2wkypzqxv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2ertxatzn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2rfdqbaeh.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2fesxtmao.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2fvxofgwc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2oheqkqvu.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2dyoqiqrd.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ubarbsdz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2kvbeyvkk.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2cwyjtjoo.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bvidvuwq.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2avmtkbru.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2zjhvylrs.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pafhsfuq.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ddkmnlfn.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2sxsudmng.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2knxuwyvl.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ckaxtzxs.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2rdrgzdfv.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kaxmyzlj.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2sanyficj.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2ipfhmcqu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ajqqjlxr.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xcjoahdr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lgetjyhv.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xvqjrdtp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2wjqyvuyc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tcqkejvs.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kmcqhftb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mzpskxtx.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2xblpvecw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pgtzvkco.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bdbmxtly.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vepedcfq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mfbzwwce.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2kotdtavv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2edzeyxwj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2enivkjjg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2xtowyezt.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2yarlncdq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2puvnbsnb.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2bpmchlbv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2mcmqcezf.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2pvnhtamn.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2jxifzaty.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2bxojatej.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2ghdqquow.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2mybarqgc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ttocheam.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2xvitvgyu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2osvmldve.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2tyjmtbgh.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2qmbvihoa.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qxvhyvrb.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2nurxcjid.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2jgnbwthv.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2btaowtpl.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2uyczvdgj.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2muavooio.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hbtnxlzv.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2bikilzjs.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2zducupxi.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2fjksjdwd.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jrkjafuh.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2karasnps.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jehxkznw.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2bzchjhdz.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2fhimuvds.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2creohjto.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2voegmbtc.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2cnhdgmow.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2vrtczzce.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2uudincbu.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2nuldqvkj.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2uuerfvtt.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2hbpxmake.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2zharwcgr.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2cglditux.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2vjhquith.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2yedxsyss.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2osvfdgyl.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2plnvpvdv.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ccfwxqqk.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xtrbvxsl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2adrynzhj.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2vuowsxnj.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2hcfnutco.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2lxmwtauo.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2syzwftkf.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2zyajtkss.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2kmsuzher.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fofpfumb.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2euueszaj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2dlgvgysp.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2gqnhmuql.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2rsrnjtyo.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2cpklmffs.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2yefmqyty.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2njiuqqih.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ulnchcqy.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2essqcljs.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2stifaglz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2bztgjftw.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2dnkfwnpo.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2hgokgllu.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2hvalhgvc.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2uamapjrq.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2rupfkppn.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2lgbwwyzp.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2oyvafxqi.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2cbdvnjfx.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2eocsspqa.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2zrhiwcyg.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2itcbgjtz.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2qkguhfde.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2djdwwbrv.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2xnhiqjjd.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2tfwgeout.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2dcsdrbkj.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hfzwqpmx.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2wxfmjukm.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2towjsbdf.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2afxkhxxw.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2knktwhno.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2ffdevxze.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2vxylsgae.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2sydrpins.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2eijxdhgt.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vsgzyeib.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2ecdcsbrb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2ectpqqtv.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mmornnol.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2nkitvbab.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2nqihllje.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ujcjehiv.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2feuvbipl.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ujtavywi.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2lbsobcse.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2xudtspwj.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2fafqlett.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2vabiskqi.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2jonkxzdj.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2pzljrvjm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2adrfzlkf.html


<!-- 参考信息 -->