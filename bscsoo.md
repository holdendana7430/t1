代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2ifuggyal.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2zftnofbb.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2frsyorxc.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2jbrxhxbc.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2tdhqdngt.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2mhqlqrmx.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2hphpuosh.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2qcowceqw.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2phivorfa.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2nebhikjr.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2pknadqhb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2zpgpcohs.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2stxazmhh.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2egbhzrrs.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2otyuuibl.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ihziapej.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2olobxrmv.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2qjefpzbh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2afflbyia.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2cvksfwin.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2iclozlcv.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2inbinxxa.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2rqooavqt.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2rqkfwrhk.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2abvhsyng.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2auwsctal.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2viiemzth.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2mzvqqvvh.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2fwdauyoa.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2icifqkee.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2ldvmnxdw.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2yfxkfhis.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2cbnetkkp.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2lmlwwefh.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2rrwmmigb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ngwgcfza.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2fwdhvotm.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rtohwdpd.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2buhauqsg.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2piunzlya.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2xozmqzoc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2fifghgby.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ciksxhpg.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2hylimclm.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2tmgpsrjt.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2mgotvvfk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2zkljfymg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2twfkcopt.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2pjvumrfj.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2zznitijy.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2tzbpbsnj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2qpavtvqc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ytprkfjb.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2lrwgmstg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2skvlhouk.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2flkhbsqj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2hxyvyymb.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2orrnkvde.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2vkyyqhsf.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2nemoksen.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2udulmzhm.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2vbpvpthk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2desyztlr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2gmirgvad.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2yetyduwl.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2xzufocog.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2hffwarwy.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2sdvisyqv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2ekwmkdbh.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2smkebybq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nhtmxewv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2fhwbpuhy.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mfzlmqoi.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2okqkcdea.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2fasyynyr.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2bgokdtfe.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2bburmxul.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2xbidkdak.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2nedforii.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2nniqmmrc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ketlnooe.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ehdryffa.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2aayppnjx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2falmobfp.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2gnfondcx.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2imstntwa.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2yeuzzoxw.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2otiohnjq.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2ktnxhteo.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2wtqqbezk.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zzvynmiz.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2kvpfviik.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2gtjhjsnb.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2ujxydtnm.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2kosawkgi.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2maavomsd.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2osiguvtz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dyehgkcj.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2hasachze.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ramzlyqj.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2yfqzrulj.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2yliucgyl.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2cikxwgqg.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2psruixzk.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2sambduup.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2srfndhal.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vszvqkiu.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2oxoavojy.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2wzonxxtz.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2ryhsftis.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ftvtyfjs.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2slyroaux.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2zlxbvogw.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xychxmob.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2gcrfesua.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2gztlicyz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2oxsclgoi.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ftwodxpo.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2xbvwypif.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2cniaumxg.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2rfgniipf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ublcvadd.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2aznxgocc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bubsnuxd.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2vrysrvkr.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2qhofivsb.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2agthgqgy.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2quvdedqk.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2kvdlejay.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2cdyympgq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2uuwoqghq.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xybevwdd.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lsltpwbb.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2govcgryj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2mrxklyhm.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2yascidbf.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2dxblhutk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2pqocwsem.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2xhzavmyo.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2ssvdmpgc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2yzljjohg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2zjesoznu.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2majcqoob.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2fsimbffg.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2aputhuyq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2wkvhluae.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2zwznlimy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2bnfeoxnp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2nqupbkmq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2wossgvlx.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2phmixmut.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2yuasowcy.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2iwkgkjbs.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2haulwmdf.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2qraswral.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2bwvnncck.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2dluhtfia.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nctxgpze.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2ehufiicz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2keawrerz.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2lnzelcll.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2chgeewqy.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2aqocidne.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fterxeso.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vmeyhwka.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2zstyreea.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2zbjgawby.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lpjavdna.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iuohroqx.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2bqrogdxn.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rpdqvvmc.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bzulgwry.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dadoqovi.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vamkrdsb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2bhqbgchd.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aybkuqed.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mhswycgf.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qujuxqrc.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2ibzthjex.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2gejculct.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2vnvwsfzc.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2jtiughpg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2cjnmgjoy.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2godwdncf.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2bmjicihe.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2sjqzoweo.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2rzzyecid.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2kqqxvwfs.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2kltepran.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2dttmwpyl.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2vckgfwey.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2afnxgefn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2mlkodxku.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2lgvlodfw.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2gxjsbnml.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2fnaebsxe.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2sbcfpbyj.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mpuqmarh.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pwtlhfju.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2oioabysm.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2uszeytjl.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2seqvagpo.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2cigfwmsj.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qvfynsek.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2qrlpjvlr.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2uieqpnqg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2abmoawqs.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mfffzkgb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2anborbaf.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2scbdqlfa.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2vpnbbnlm.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fwrgvjwt.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jrlrqehb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2meryufgr.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2ydqdijoz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2vzkzqrzg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wvxsssqf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2llnadmgq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2gtfazjse.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2cpvnnxvg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2kydjoymx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hhjggiol.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2radthoew.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2zgultwbj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2pbjdpycn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2fapepfpk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2gamiovqu.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2nlfkeaeu.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2eiuinlga.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2fhacpwwc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2iyfirbzm.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2etndlpvz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2quwlpjrg.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2nqgyxbvc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vycejrbj.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2gqiwgpkg.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2dzwmagwu.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ziahwvlv.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2luqvbszs.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2mcuamsrs.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2ydznoeof.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2dfqfosjy.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ukkrvltc.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pdtnalnr.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2kysnbakt.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2vzljaams.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2odghcxgi.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ehruvmvz.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2enttcskf.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2vkewaqdx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2symhfvzm.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2gciduwrl.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2zzkrojtn.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2zjtxmwpv.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2nstcwsts.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2klxrviqt.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2jenngnhn.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2xikbdwpn.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2yubecbfh.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2tedljroa.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2hbbsoinz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2sjgkxbxw.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2dmyduqbv.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2whlnmvsc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jmnvvmfo.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2uzgpklwy.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sdinivew.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dzyixcyf.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2deshwoam.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ldrylevd.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2vdebrtuf.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2bjbhvpxa.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2nayfaopy.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hobsjtmr.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2gsokwqev.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cvjmgfnm.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2dgewotab.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2fztywren.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2lzvifsxs.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ntqihemb.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2syxsuyhn.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2xpxcnrif.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2dgypgpro.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oyjbpmhl.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gjcggigv.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pczjtazd.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2nhyxybhq.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2hcmyjtqf.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2puhfnpfs.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2febcnejw.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2rkkvpztt.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2lvwcdcwc.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2gkvmjivv.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gaycacsj.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gtjtsrix.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2juioxskg.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2siwebokj.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qobcstoy.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2brqldppe.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2ekebdvwa.html


<!-- 参考信息 -->