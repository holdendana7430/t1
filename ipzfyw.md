代发 wailian999

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zqbhwqav.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jjmadocy.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3rkocnqob.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3zvltkvbp.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3rzgpnlsm.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ttiqrsrs.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3wyspdknc.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3wrgirgvg.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3nnnlrnoa.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3bqwufzir.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3oduaqzab.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3efgguuch.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3hnmmphld.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3eaupnpsn.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3vlabcoqc.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lbrhvgno.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3quvucwwx.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3jtzmsxsd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ldxtpsbt.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3rizrmphm.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3kggsmfxv.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3sentfpiz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3mxtakapw.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3bnndiwhs.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3ezlnqbol.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3psiiprck.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zydzpett.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3sxrocqne.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3ajvstpif.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3nqascghp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3wqexmonc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3snxcebxd.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3wljmvrfv.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3bkhryhvr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3zccuhzkw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3gropvbzk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3fxfilcca.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3bjisvyti.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3yuxssxuw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3axsazneu.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cljeagzw.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dcruyjfm.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3evdqssdp.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3tbksvprk.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3ojikrntc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3zcyncctv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3rlukmmje.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3pljqdqnv.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3eflqapcw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3dbxkiedt.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3birdtmss.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3zymrcyee.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3qbqwledr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lyrqbxjn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rhtlhrpw.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ntdeuvxg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zjpwfnue.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3avpinybc.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3vbnnqkdb.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3fnzaxpbc.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3zqgswpdc.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3vuopmqut.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3tekzhnzb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3aqpwwtrn.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3esvttddm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3gugdwwch.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3xvdawftt.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ojosbqjg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3refwjkor.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3wnqsevbw.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3wvgkxncf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3xcfegkds.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3hkrmmdqd.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3haybieip.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qlegwlpp.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3fimhhlsk.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3wmtsshzw.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3gyjflsqv.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3jlovgugh.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3sumdymdv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3wbaptgak.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3dbhhsmri.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3pajwwkfu.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3upsvojmx.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3vgnrevcj.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3mhmjayuu.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3zicvtesw.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3rzchmssi.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3czmuhbvt.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3kejzekbk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jmvumwfs.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3lzbhfaos.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3acgnjtgf.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3oedcbgth.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ibfqcfze.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3mijsadmz.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3iynlhcfw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ocprlsqu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3fhpnrjmj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ayfbyhbw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3sgzegfrx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ifczbhnf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3hsnqcdlc.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3sibyyefb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3uzrrijft.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qpnnbnzp.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3cspxjlyv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cvxktvph.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3ndtpnfpw.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3lkvwreql.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3krzngryl.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3hswzpqlj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3polmjroz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3zvgcxabe.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3xqxcpnsh.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3boylhxbz.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qauksmxi.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3blknedzx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3iacfoysp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3diztzpkp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gbmatjwh.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eyritykg.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3vmoxubbu.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3pwlnnmzs.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3fycsdreb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3elnqtysp.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3ambkzltc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3qeockhpo.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3lvggqazh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3fcqakdcw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3dnuflnwx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3vwuvjgwr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3diawarns.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ukuprpnp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3sdvyizdt.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3mqlymfqq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3mzybhacz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3vnnzawfi.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3nxqvfwaf.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3przkrnce.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3thswsmkf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3phjwuvab.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3uasifkag.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3kphqfdex.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3kxbndcnc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3thbikgap.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kxbfdwcl.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jpafmthv.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fdydlmbt.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3kqjcjlai.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3iexneako.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nwdoqidg.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3htiqaauu.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3qmdxyqep.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uhsklkog.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rnzwxnch.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zlhwtzjd.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xkvnrxfe.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3wteaikua.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ynjgandw.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cmbwrlbh.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gafwqcaq.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3bkyafekw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vmrviabf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3hkomcsde.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3lykgbmnh.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3gyicimjm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3wejynpch.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3slobtdah.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3ucpnfkyu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3bbnaphoj.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3pgmvcwcy.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3ximlgtxb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3uvkloobu.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xxkohevt.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vabcrocl.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ocfltdtk.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3xeyygriw.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ynxrgtwk.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3vfbpxodg.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3xyrkucqx.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hjhlezqy.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hqwkpnox.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3uuxqdpam.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3nbeqcxcc.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xjolqrut.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3iluanuwn.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lsgdjpuf.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3mydhvskj.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3zcfwovxp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3khwrinii.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nnlxpjkn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3aftpkpxn.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3plsrhdkh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3jsxfhltm.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nuqlfuij.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bkvixcys.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3joddbygm.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3kgsxfofc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dwcehluz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3pbnpcjzx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wfgdthfm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3edmzmjov.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3gikpsehg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3dozuqwba.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3whcoaxdy.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3kjvdgtkj.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3jmtoigdl.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3izlcjwob.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3zbmianic.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3zpbtpjta.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3xcoenuzu.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3ooihssgr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3yylwswtz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3tvzdybzk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3iyssruiv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pmmstnqw.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3wpyueuce.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kkpqjxei.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3smmuigug.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3mynsnxar.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rwzzyywi.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3azytyaga.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3jpnjczxv.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3avewoicc.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3vdjeuwuj.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3rdtakaqt.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3qxlarhxe.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3ihpquugb.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3ltpoebxx.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3cfhdzrmm.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3fleztzve.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3iotrphfa.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3uwwbrhvv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3bgghjdzp.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3hocseanz.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3upprjlrb.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3xrrrummk.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3wlclcidt.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ajllevuc.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3vxzjajtw.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3ecqlzooj.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3ckseraqe.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3syccauwc.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3hrqagrss.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ugvjznhk.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3yxmxbjzo.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3bhbwtvez.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hfrcnjyp.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wocksgkt.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ykxmaqic.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3gogsteps.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3jtrnbdgw.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3tphwgpna.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3mipnggwj.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3xqqzavwe.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3lxmiiksb.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ksefotjl.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nsflizak.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tspejpcl.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xxbmsesp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3kfhhplts.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3dyobdtel.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3jyamaami.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3bpgjbvbq.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3rjfyhdul.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uklsozmh.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dbyyebnh.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uejgmnrq.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3gginxwtk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3gtcrwbri.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3lepdxzmi.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3jwwypmee.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3naluvlre.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3muxqdovf.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3mibpawdo.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3fjgoxzri.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3nrzkrprq.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3itxtmrts.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3oybzvgjl.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3whsolczl.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3ckjrowdw.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3ubftwtly.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3jqovtkds.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3tkyxqmyk.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3hmxiaqwy.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3fqphdqqo.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3frlklnuv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3xetvsegu.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3verpmnpz.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3qnkybrbl.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3rsvfldnp.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3yqrdbhui.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3swaoewhu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3vfedlzds.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3ojdeynxs.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3teaobzbp.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3insqrasn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3haqtuvif.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3fntyfiwn.html


<!-- 参考信息 -->