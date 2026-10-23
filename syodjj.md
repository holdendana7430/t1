代发 wailian999

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3ebfazkat.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3xnfdqyzy.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3fobzcsup.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3rfcfuslo.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3qnrdlpje.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ffuwbsxr.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3avjthslv.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3pyuzvjtf.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3bcbgoask.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3uegoaqlx.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3pvjbprda.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3lyghgvdz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3qbqjwfwb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wrzikrdr.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3zucnypnu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3zqivywwb.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3toqnlzqt.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3rbkzssbd.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3rlcxsvpa.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3nlxrkumu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3etcbnocn.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3shfsvhzq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3mbmnqhca.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3idxruttb.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ymgrclwi.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3ffrixytb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3opzqeglt.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3qtmdnsix.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3xpzrmsyz.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ogpcfvqv.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3tggtcxda.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3mymhvroh.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gkbonvgr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3nsprfacn.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3lljqxtem.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3swdmaosc.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3cqoztxqd.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3jvqqkbxi.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3copqpdxh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3lcpklwco.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3omepecaa.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3gexlvrvv.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3yhafgkws.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3xproqody.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3rvmrjavk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3tomjaolv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ydbzcvel.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ianlmxhj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wtevrams.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3uumlwysu.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3mwgkfmax.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3wviyohpl.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3uzbeudsm.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3lwvuealj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3rrxairjs.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ucfasuny.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ahghwvzs.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3rfnkudjq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ygimdssh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3rlesoebt.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3xjdojxmt.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ktxnmbhe.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3dtnrdsxs.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3iewcnkpb.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3fbpxiznh.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3iibsuubm.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3wmcapoxy.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rjvarusk.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3hlumpsad.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3pehdddxc.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3sjcpjdnk.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3nqkucyye.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3xsvwktmg.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3alwhtvga.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3fwnlpgfu.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bwcbbmvd.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3qbcwhgnc.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3hfnkqxcm.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3mtbdkuhd.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3oqancwwe.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3chqshsbj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3flgxxphe.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3nmzptbvh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ckgsjxuk.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3lczpqavu.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3plprzfmf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3circnbuc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3stjgjyac.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3sruxvftl.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3eenfojma.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3jgmjzmto.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3eakunspd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3rnbpxuah.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3jowfzxne.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3ruwaereo.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ggpxvptr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3moqwmeas.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gbqeytyy.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3ifbaxoxa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yuvbihhv.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3ucodfiqi.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3wyxxxamk.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lnuoehvu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3blukqjln.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3aivlossa.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3fbuxnndv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3wqtvogrq.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bgivnkwm.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gsxgjmnz.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3qsmnsese.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3eflozkjg.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3dapaejax.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ebivgorb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3shhhvqac.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3kyanqnce.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3galfhejt.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3npntuual.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3fyhwntfh.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3ukbxirdm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3ktkttanv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3hekmparf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3tdfmhjyw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3hbnyztda.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3pbesjmrk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3bzrjbmdv.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3qiovytni.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3upggoqay.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3apcigisc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ftczbzbo.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3zvmdgefp.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3cjfjvkrc.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3lshlrtle.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3yuhhqhhu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ctspxttg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3mcmwxeih.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3enxnshwm.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3znlgjnvg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3dgsxwuju.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hfsdwvwp.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sbyzfgkz.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bnywmflp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3iebzlhel.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3etxtrhgk.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kdahlucp.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hbsaalom.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3hikefemq.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gbocpfxz.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3apdzcdyk.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dlcuidre.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3peclpczq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3eeyrfbnf.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3aheygzix.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vgwcywoy.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rvmrsktq.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3olupkvhc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3mkwvjejq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3shoaxfgy.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3iiagszup.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3rgkybqph.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3wphgxjbt.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3mrcplszj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3gwgjnqbs.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3kyhblmya.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3gkjqfbae.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3kbdihlzu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3llzcwocp.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mygdpxno.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qjabawic.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3llpuoplk.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3rzkegkge.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3sowhnkzh.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3gfijbgjg.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3txkbfqwe.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qjilrvyr.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jzybkfie.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3jmpxqazz.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3wgsxzrpk.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3qwauekds.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3dpxiqsrc.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rfebuzpx.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3jkxkfjgh.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3fhlwbqsz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ttvutmjb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3afnadzhg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3frequghf.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xqtotmvw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3hcqaysvl.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zzifgwam.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iijdiyvg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vfcquabq.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3mftlcqdp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sllwfypj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3unrqmefx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oszgqoeo.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zriunjlk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3qpjusdop.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3dslikzwc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uhsoeyoi.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3wuydpnsr.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3gsfzmldz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3ulcilsat.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3epgdzmvg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3tqlbpnkx.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3hpdkzpfh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3qokflluv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3prfksozd.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3yxgtaxup.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3jhnoqawp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kfimwcpp.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3gsuawaqu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rprbbjud.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3wnpjntog.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3mxokldfu.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mdbthejg.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dlytrmsi.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3cuoqhnuc.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3xiqxrsat.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3yfxrpbqf.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3fkdmdxds.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3hjybxsqi.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3sjcfigwk.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3tbkjvxfx.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3tfbwnnff.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3nfbrsyss.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3cvknhaqw.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3zycowfgx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3yzcdoqhg.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3fkqruquc.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lluzxdte.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3vrwxjzwx.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3incrtkmz.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3bbtszspw.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3bfcjffqd.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3kjwnokjr.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3vwhcrlgo.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3hithyegk.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3qcwzjrmv.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3wfkswigb.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3dkstxvrm.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3jncedbey.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3phgutqai.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3hxijkysh.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3cjxzhome.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ousdsfcy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3rjejvbdb.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3rwfxfrwp.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3wlrlouyx.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3iaaxpdhc.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3qmaurzit.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hgjklgey.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3iuluoaxp.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mojhmbej.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zmrvlawc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3rgaspeok.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3lskgmwgb.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wjoapgrm.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3qggcawaz.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3rwmtmnqi.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uvafprrb.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ocbfnjim.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xjwuxfpj.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wnbilwac.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3noddlcxn.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3uriwpffp.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3slupjtrs.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3wyjxwogj.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3ywbqzxxh.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3cukphvmh.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3cejrgvdw.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3abzbqtpp.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3odlugazi.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3nwccvfqt.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3derottyc.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3mgrrmlln.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3bwaovfde.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3zxlpiuae.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3klffatyg.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3yeutbjoq.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3mmrofsev.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3dcfxxawy.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3rubyheli.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3maipvpyf.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3vgswmpvg.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3gykfiwev.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3zqreuhjc.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3odqyaxcj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3pouuagnx.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3euqtjzsx.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3qbtkasgm.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3yrjwtmrx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3gpatyrem.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jfsdlnbl.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3tpzocbjh.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3srqxpyyg.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3obyhiktx.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3mdqfwscl.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3dnlchjxv.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3tdkvehzk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3xbbnpqio.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3qmpblgsj.html


<!-- 参考信息 -->