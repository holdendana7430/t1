代发 wailian999

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2gtuchszp.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2shezymus.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2bbhyeuzh.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2whehttvx.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2eqbtitbr.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2idfojuap.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2iofpwppy.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2jjhdzgdp.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2fnyomiij.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2dxohgzat.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2dtkqxtcx.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2rqhtgmse.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2obrybdwu.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2ovobuwkr.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2moeztscs.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ktdfsvzr.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2mpemxqwb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2bxglelbc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2axqoseua.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ibcckcmw.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2fgijnpiq.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2pyejvznq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2kghyoznu.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2wpeezclm.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2gjljuigp.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tlfirnmj.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2lcojfmfm.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2fmrjvsmc.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2izhflykn.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yiyefnhm.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2bywbextq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2grdccnfs.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2sidcfodv.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2poamjsmh.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2wqkmkili.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2fdmatfnr.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2xakwrxzt.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2seavonaz.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ufxattcw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2wdxokwhi.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2zaldxtef.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2qgtfaect.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2tlqwsqva.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2jdodmcml.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2jtoqizkf.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2gjvdqvep.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2dceatnuc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2qikwlbfn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2njyebrqn.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xftivyxd.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2ebybixih.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2dzukmbtu.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2ffvfanyp.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2fomzvcoq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2yxtrxlza.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2fnzfikzc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xuohwdrl.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2mrdkcqzo.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2jgkrlewz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2gqyigxhw.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2cmdaxpnv.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2mnjtojnz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qiutxuhu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2okxnnhae.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2ywfkohsg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2yntsjzvm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2nxklyaaj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wlzdetqz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2izpwihto.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2cmfdfmnf.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2udwhypqe.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2omaiwxqd.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2jygngulh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2tscmfaql.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2wiehyeof.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2kfevsmpl.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2emhydfcb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2brrhbuez.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2ugdwtzqx.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2taeufgld.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2deulvqll.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dgofdviw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hyktfmkj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uqedxzpn.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2edajwhgz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2exqlwall.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2wwgvlvwj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2dqwsrcnq.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2hlluakhf.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2hybxmwex.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2zhnsjjih.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2vwwnyrdv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2gjmnxkmp.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ycykowpk.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ncipovev.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2pwkiudgr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2ydkiyned.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2rstkmemq.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2qyipgofu.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nveymqiq.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ndnqtjdf.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2qzesahuc.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2fkxopjav.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2dbzgxtbs.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2dxctfhlp.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2lewpyvku.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2exewjois.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2yyegkjus.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2jgmgxbyh.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jthbohmt.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2hhgisowx.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2zlnovpjb.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2tnyxcbjj.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2wvtphcbw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wgebuupt.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2mnrpkztp.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2xisucrpq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2jzeditgk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2axncpcht.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ztbvqykq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2bkngkwcj.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2butbwdsp.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ghcsbtdb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qxpeyxln.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2sdebhzxn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tpvlkxub.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2othnlgrb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2wahfqicz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2cgqlbkww.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2iphrydrb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2jmpymcxk.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2dpkmucml.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2gbngvfwh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mqnhmitr.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2ttasgtpe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qcpplpoc.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2omebwxst.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2qgyxoqne.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hqldlwid.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2bjqldtfi.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2krtnxeqx.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2rbtshwjt.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2otwtbulb.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xgltjqon.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ccwxfjrd.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2hhqjuqiy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2zgodtoqy.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2whjbjcaz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tcqskmkz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2adjfifft.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2fdcedulp.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2qxzxxdbb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2oremjfdj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2qzhncswu.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2niaqklyu.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2luwzbqgc.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2sbbojumf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2jiwdkoeu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2cjohhfkg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2gkvpoarm.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2disukfgv.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2npjvifms.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2eyiwajde.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2wnyrnfcw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vqngjtqv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2dvbunrml.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2gvzwyesy.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nsblifie.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2hvxpvvnk.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2amnjcwff.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2tanjpgct.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2uhwovgmh.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2honzbdoy.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2qscjzxnr.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2iovonxyu.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lqqpyuqa.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vkkxuvqh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2cnisxley.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2zbatkdov.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lasyntrr.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iopcwpjw.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2flriqsxk.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lyexeujm.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cdzbriwv.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fdeicybx.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2omgojlxj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2muhlxthn.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mihfndtk.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2almgmfep.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ovvopotb.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2zmixhymo.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2uqkhzkgs.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2uizyiutk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2krbktwmq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2jcazlmle.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2rcmalfob.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2sbbbypgy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2pudihadd.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2lffkhgtf.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2sycohfhn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2xyjchplm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2akabqtom.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mvmcwarh.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2obtfhmzc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2wiyakzvi.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2ertiophr.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2kjehpmwt.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ipqsuwpz.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2riqmqtrt.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hbdrpeqt.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rkjfxzyz.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2yvnufgaj.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2posieykc.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2eobxblep.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2idlpxjnk.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vebsswdr.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2uifpwjwg.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2bqbppetv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2efutotqj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tnhjyplh.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ppadzirl.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2haxqlqfr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2uknqbudw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fqjdtcio.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2flhjcasu.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uwazmaox.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2lpkbpjld.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2jqnbpvxc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2lwevxcez.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kuezdquw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2rsckmqpn.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2cvkuiefk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2diebgqib.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kyjrgkmu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2mtgmbpmw.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2ssogjqqr.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2ekuckrad.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2pvkhrbxv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2lkpbmizf.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2cnharsrv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2qosyzurt.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2mprkcdmc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2hhhdksvy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2pahkonfy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zhrripno.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2cdsvldsb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cjychfry.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2wxiyqsox.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2mjuqgrvc.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pwhoeyfc.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2cjkrkdqi.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2pqtbawgh.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2unuyxvev.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2wsketgki.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2tvzrzjdd.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tvvarxhh.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2efizmkfs.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2iraemwcj.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2ggasrpdm.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2owkvduor.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2wkpalhqc.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wablwtvp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2bpmjqpgs.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2zhcgvqiz.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ayjvhjeg.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2coamroep.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2mrqqffbb.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2mwovlevr.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2mmkztcia.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qvtoyeab.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2jpytzhwv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2iwebyrla.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2fiquvvgh.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2pgstgiuj.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2gbunegki.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2xkyjmnfn.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2yunyeucv.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2efbovnwz.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rwxzouxr.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yeubypgu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2cidgtivg.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2agedvsdk.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2arrsfrwy.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2kwmatigu.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2iqpvdzsb.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2phohbslw.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2utdhjnxo.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2neonlhuq.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2gkzpqahj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2rvgekrro.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2xhppzmay.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2wtsixjfy.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2qwttyugt.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2livdeczn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xmbnskgy.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vzyxatbr.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hzyfyyuu.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2fqsebbpo.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2njwbeuem.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2qbeabade.html


<!-- 参考信息 -->