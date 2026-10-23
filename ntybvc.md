代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3vjwavmrm.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fncgpcip.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3uoafsesg.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3rvyricyo.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3dmdjbwdf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3uwuksszb.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3mcklkfnl.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3mjamwjve.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3yiugcqav.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3yoqeaxhg.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3jdafohia.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3xdtfzeen.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3mxhgufvb.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3xdgstqps.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3vhcuyfco.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3zbvkkaiy.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3cpcqlbjo.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wfkyggrg.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3ymhxigaw.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3dbgdcjzk.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xewpnpsh.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vjfngvai.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3ksbmrzvo.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3qbumismz.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3tljjogci.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3cigokrzd.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ypbhmnmt.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3hxuajmzv.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3lygwoqrv.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3unzgcekp.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3fuzfosfy.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3laxgccsx.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3mamihyaf.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3gcyrdmtr.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3qnalihyi.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3poviihff.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3xtbmssjn.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3humdnsxj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3sxrqvuse.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ktkaokbg.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3cxeddosd.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3evjdnmtb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3sijdtmik.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3gyatlbab.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3qqftpbqt.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3abiiyrjv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3tyyhcugv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3ebjxgica.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3gkethuqh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3euxdsjon.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3tktpaqfy.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3hwrkdycn.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3cwjwrwvt.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3ahegjkrj.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3hmeiwrtz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3aswbigml.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3coyyxctg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qemzirjn.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3xqvfvafn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fnpmupgr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3dmqcidxp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3kdpzibcm.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3bjeomxze.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3kgawoyze.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3iccwbhbw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3zqgmhzkd.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3wwsaxvaf.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3weznaouq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3wiihjusl.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3itegbaxe.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3nrlwbhoa.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3kgyxoxhz.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3eadmklct.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xytwhuvh.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bqrzfjvg.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qklovvtk.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zgmydxus.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3vuarypkh.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3upntcutg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3lwjsitfy.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3vkitosmz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3ydaesvme.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3xsqvxwzf.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3qxoesrwo.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3jcneytvy.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xjpbkwxn.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3xjjebzbn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3kkorcagi.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3jkeknbhv.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3hzrwncaf.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3phkhglgr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wsuwtzwf.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ugxsdmtw.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3tdzawzmx.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3tcgharsm.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mxihtsty.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3aflisurz.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3lettwzrv.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3syrhdswa.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3cnvlusth.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3pmregqsh.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3rldcsiqs.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3chyrjbwf.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3hvajawdc.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3qrlbqqgo.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3cvyohmmk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uubcpnbx.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3eegfvhpm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3zlgugwpd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3uwwituwk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ngutbqan.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3skaizjcw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3joskpcbu.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3rcbuqgfx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3snsfzpth.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3kmtdowxw.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3twepmbrc.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3awekwbsc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3vnqfukyx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3gvxcgkwp.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3iavakjdy.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3cqqgadmp.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3jieclmrb.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3urilinpm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3brruzcvd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hiafvhyp.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3aqbjindc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dumfcdsx.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3gvxxpixy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3zgbiqscd.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dgfhkcrg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3rrexpycd.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3tanetdlr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3awgrvini.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3dzjxlihw.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ujosidpb.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fnqgancg.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3mkyffxqy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3warnmbxq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3haxrlmqb.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vvwlkduk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bbhdvtwg.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ncebqtjh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3wkhfmvom.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3itymqwqi.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3ppivxqnj.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3txamdsez.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3pebyccaw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3quzagcmk.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3lrmwqqcr.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3oqmnikma.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ttidzhjr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3vhpknwpv.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3kefrnnno.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3pznddbdf.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3jqmtrmiq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3korskwzm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3whbdhtsu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3bjwgpuha.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ceoszrfd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3bwkpeips.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3bgwrqkps.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3dmpgkley.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3rulffrsf.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3xzagszif.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3tkidlmhs.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3sanydckk.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3guypzasw.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qliowrhz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3gfxfbblp.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3mhsbflua.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iiusbkpu.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ewbykptv.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3rudrmvfe.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3owzdpsld.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tbdlczqe.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rkouavla.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qbdcznmv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3dfiethwq.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kvxfjqgc.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rekyapvp.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pwtgobat.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3ozdacgad.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3unxuwita.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3dleqsngx.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3klvnfzuu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3hakqlnvd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3hqufjnan.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3hbdyqltj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3mdqbiqfe.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3ambnfuvk.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3dvxamsjb.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3ilrbeime.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3ltyviiff.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3wkpllobv.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3gdmgssea.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3nitpxrfg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3bjjnmlrn.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3eghkqeto.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3nadmwwxt.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3mmqjfrty.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qlpgtsjq.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yfajftbf.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3hvwonqie.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3pxeyhuxs.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3vkebdkdm.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3vxequeqa.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vymgkmye.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3ceqffwid.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3sqwlszyr.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dwgfbyru.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bcybfgni.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sqhwyccn.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rzlhupku.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3mcghtyml.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wfukiequ.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jtskwwan.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oznldxyx.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3ifhxzbgv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iqrwcksf.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3xofpntom.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3gorlidqk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3urhyzdpt.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3zliafzao.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3hwbjlxqy.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3xvgyznjk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3ffdofnjj.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3pnyehtlq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3zrfoyfhk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3rjsznztf.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3lljhprbm.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3puctbzpj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3duqbmojn.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3zfjezvze.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3nbjyztgn.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3futbyqkx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dbwdumkb.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3wtyflbms.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3auhbfsxa.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3khhgtmfp.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3qhfkqolg.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3klmpslxr.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3osdrzwqz.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3jfstebjc.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3ezprykxu.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3sybcepcx.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3zxtahnau.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3fejcgmmo.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3gpoyhafw.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3rcrymqpr.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3mfwwhrsa.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3djgfygnh.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3gbmanmhx.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aauzbfeh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3dhdrvqsy.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3oezgfsey.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3phucfwbs.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3mhzjmbnr.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3dtqfytdw.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3zlhnqyye.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3yfzceiem.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3gliurydz.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3nvbdhenq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3mnioucji.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3imlbhiyw.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3stwjwplk.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3cwnmanpa.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3aydqkpaq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3inzpqvxf.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3feikjogi.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tgbhjyzc.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3dqjlndxa.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3wvbzdcql.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3jlnivbya.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3wytqxaaj.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3onxfhaqe.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3euzumtoh.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ukarmmiv.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3pvnlbmev.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3lgjejldj.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cwyqtetc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3xuruungl.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3xeedqyms.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3nkdwhzfo.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3bxivwpwo.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3axkhpdgq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3mhqhgebl.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cnlyycjh.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3vdiseanc.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zyztbtzh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3hayypqop.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3giahfsuf.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3pshmxzei.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3gynhgzqc.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3oppvvenn.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3sijrlchv.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ebzqoxeg.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ugnseakv.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3uoxzuzrj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3wbmevcdd.html


<!-- 参考信息 -->