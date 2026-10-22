代发 wailian999

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2giknpybq.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2bwnejwlz.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2smmgnkop.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2xjlyrkiw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2fessopuo.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2jpwuqqyd.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2lvfjcesl.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2uypoqtyz.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2vvvzbmwv.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2tgieprkz.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2vyvyyior.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2qndhuhvi.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2isgxkzaz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2qpnmczse.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2ffwhazum.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2pqntrfnk.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2giqobxkg.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2sutnmepd.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2srydgdod.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2gwhkeelk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2lzwphvxq.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wtmgcaca.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2iwfgbsps.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2jqphgywl.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nrenatxm.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2scnletmo.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2vdqkspin.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2berukwdd.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2zrqryitf.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2hhhzwhje.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2xvagybbg.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2udafmrsn.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2nflpzmpd.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2gjgbweug.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2dtbznohf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2mbncxuwd.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2lcgwqtwf.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2okmedqxs.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2zbanpkmr.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2gyzyjuuc.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2eunyzgeh.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2zismznpj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2mfrzjxyt.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2lkvxpfet.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2hyqtlobl.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2gxskveuc.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2httnduak.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2inlxcokp.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2ousgbhle.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2ixqfrurg.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2illwmwgt.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2xzlnojfj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sxntsqar.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2sowngdcq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2inoxeguk.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2trnnwgos.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2whykzzev.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2ussoguna.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kxfsgkdb.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qatfktbx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wadeccyy.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2dejtfgya.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2fjqigiky.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2sgahoeow.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2ywscckli.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2edqmwola.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2aodevxju.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2wbanmyyj.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2cykoaeom.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2msktwazq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2aawlnaeq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2shgndzxx.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2gomnfynr.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2rjvpdvbh.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2nhntuxnc.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2uimkqvuz.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2zclkpmgh.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2iplcrndi.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ojozuctp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2whlobnac.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2prxocsed.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2abgrnlub.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2gfyeloch.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2vwhbtvjl.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2nyjssbmd.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2quvuqqim.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2vccwmhff.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2dmjnkoij.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ihgjclxn.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2tjindutv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2nqfaornf.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2znchtgyb.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2dqwjsrrq.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2zkpuyduo.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2hxhrnqxk.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2shjueflq.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2qlczafge.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2tbqyhkhe.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rqknxgtf.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2ohpfiytq.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2hettfget.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2twmffgqw.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2brilhhti.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2gemefftv.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2lrkdktsi.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2repijfdl.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2iyftycne.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2fjjxksot.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2measumna.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2cmwvkdeu.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lrwclphp.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2bcfqgrbv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2kzinfnhd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ommxmbmc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jsuvgxzl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2phyfxlga.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2bdgqedci.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2pdkwmoks.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ehqgjxhw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2xmbwvhnm.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2jwoivaos.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2mnokwtek.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2udgwpcoo.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2nvorjlsr.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2nslsrjgg.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ouskfbpw.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2xtfjohgs.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2bqdxyyix.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2bxhnynhw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xyioyjfq.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2fzigerpb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cyvysvka.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2mldtncez.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2nbqoutwu.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2frougmwx.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2typzaeqz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2qeqykekz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2wbdbpxqp.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2vcwfovve.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oprftufw.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rauqzxcp.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2kjvfritp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2lgaoxypv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2kizbdrim.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tiapqfhf.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tjsutpka.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2eucjqqnt.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2zuyrrkka.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2snfkdlnl.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2rxkdroop.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2xohsopag.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2jlyjgytf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ocebtnid.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2vnddcwfu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2grqlolno.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2udzyiavy.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2sjqoxcrd.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2jkzlhjbj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2thxdnndb.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2yqfkfrih.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2zwwpibpm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2ekwqysvy.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2sjozuzhq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2flmvqnpi.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2ckfwemmf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zihiehdj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2ddcuditc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2emwtpebj.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2ikiubeeb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2iqwpryxq.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2uoxoidnk.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vvctephc.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nfyscjzq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2dwqkrxpb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2rgapxqgk.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xlumcgtx.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kfkocezi.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2hkwqjuou.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cwtauhvh.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xzptzzcb.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tdykpmnc.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lgioxgbi.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2sqjmtbuj.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zfegeixc.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kpjgmzap.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xxnogysm.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2jkfwuhts.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2mzvwqfzv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2pvwbvgfj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2izvachnd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2vysprjvm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2bkumvywd.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2mqnftugu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2lzeiohrv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2qdprqnrf.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2xigbuzge.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2orlpfwvj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2qqiotrxi.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xlbscevc.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2bmlqtjjt.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2eapizrji.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2xdxigirx.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mtjqyslv.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ubvxnuik.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2kbcgvxzr.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2okqblhtl.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hyeuiofb.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2zeeylssb.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2owcybgnb.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2smtygmls.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2uzzjyohy.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aocvaphg.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2wvfbokbi.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2zxjmnorl.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fbcjcvel.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nfunugeb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tdczsikz.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ybbkzuco.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2ihwdjqlv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lslolxwm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iinratjg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tlugemfe.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2lixyvlbz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kibjbcjc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2imzmhlwe.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2cqdteltd.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2jhlbffsd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2cpnwhtln.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2kgelduke.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xuymgclr.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2oitlpuuw.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2otljhygr.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2ojssfzbp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2jnwarsfo.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2dnpffzmb.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2hzivtium.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2iknjfuam.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2erwybgvw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2wdqyqfgc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2fdskggbd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vapxcroa.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2lrblzbnq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kcivykdh.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2vdqohulh.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2qhiquwnn.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ardbbixo.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fefibwpb.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2naqvrzwu.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2vzcfrprl.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2fkslawxs.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2gmnlcsbu.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2sxdtkaqn.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2btrohbzw.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2qgeazjoz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2pznoaaod.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bqdtmyrg.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2reiqllax.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lhjvhqht.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2dgojmwli.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2rkcskmhv.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2umnszmbb.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2whmfscms.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2sbzmzuvw.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2kyjokhdm.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2lvvmhsvy.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2znsaikzx.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2cozwprit.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2npbdvkkd.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2swfyfneu.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2ankvdzdk.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2wfqxjcch.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2znisnpoc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bjdnelgt.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wbtgunrs.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wmewalbz.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eqqvefmv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ldgylfdc.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2tovojkma.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2yphyphtt.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2gkrozpym.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2xwtdahyk.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2imcdycnm.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lghpqemp.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2njcykhlb.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2xskxfyyl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2gczymbgc.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2lwttpwly.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wpiozpqn.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2gpgmheiy.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2llkukdzd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2spgsutvg.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jdjrsbmj.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2kzdvztuw.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2hokvqakq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2dcscwzrn.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2ryvdrkkk.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2pvvicyic.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2qfbxnmcv.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2pngcdydi.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2ynbqucgg.html


<!-- 参考信息 -->