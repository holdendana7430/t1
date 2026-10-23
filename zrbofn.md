代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3jymfudni.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3lsmxvhoa.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3wmocvflz.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3qpwasejx.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ckmlnxdy.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3hlnytfze.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3fuhwscet.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3ywjdemex.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3lzwugsbv.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ozsnwtth.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3lzckffkw.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3iikddkgk.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ngfespkw.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3gwlfalwr.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3gzslwhij.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ulkcdboj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3dvorbmzu.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3khrabjop.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3huijierw.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hbiyfpcy.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3yuxvldbh.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3inkivztg.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3qxvovelt.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3myjrbygs.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3gnkgkugq.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3wurfogvm.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3mawcjfoz.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3vvjaykzu.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3qfozxzzi.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3vvhcaaem.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3iadunsva.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3aqlcsmks.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3wbqadoms.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3pshcirza.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3lomublsm.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rgzezmlx.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3wnotuxlg.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3fegxnshr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3loaqbfai.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ckygjnfl.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3bktyxyvh.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ykhygjar.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3yhqjgced.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3tvhnjodm.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3wevcqwgv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3vdkjwtud.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3vmjqjhdb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3chigbrhj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3wurliunm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3skupkyqe.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3ehgbuwlb.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3encshunb.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3omuikadu.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3xhagiklg.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vxycsnsb.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pscsslbd.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3atrdoyic.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3dgvhtxhb.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3gqrapppw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pfoxnnfo.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3obqbxqis.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3voudwqtt.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3jalaejmr.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3fmehrpuh.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3wdtfobsv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3rnezqycl.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3drztpceb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3yqxlvyke.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3ugyqdqeh.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3poejbaou.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3koddmonz.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3oaniqtyr.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3rtxriwgq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kdyrcubk.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3jhkfxili.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3skxwmsqt.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3cvkkbxdy.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3vaklwkcu.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3jrbbzser.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3sjfmybnj.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3pvxsymhr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3brwcsynk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3vgvlynxp.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3qzgyktts.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3mfnnpenk.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ifhkapjn.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3vbhjnjru.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3hyfailbj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3eexgisik.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3osixgdsc.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3frgbfnik.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hikbigft.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3bhanfyqi.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3xucgcqjd.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3aothwzsg.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3prxxciyf.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3hgklvkkv.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3qeuqfqzk.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3ybgqgacp.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3nyiunsfq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3hbmlqxsu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dlfirdvo.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3hxedenvf.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3vfjeoohd.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3wbaunxek.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3lvwctasi.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tuiluoko.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3jytymnve.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3uvwyzfkx.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3bevjikkx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3yzxoqxef.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qgqgmusf.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jhcttzvz.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3jdojviot.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jiiuxxvw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3vvleytog.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3rfnohcoe.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lnwzwvzl.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ouzomzov.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3korharry.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3wsritefd.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3zwovrlig.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3yonbcpuu.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3tgakrfqw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3zeyulkdb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lhsiicjm.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3gvyxluyg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3feeppamr.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3ocxlzyhy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3zmcheyaa.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3aftsltvr.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3qimtxbfq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3cmworqcq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3iekdqmut.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3sdficijb.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3heimdscj.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ptxvbpiz.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3krnpfuyw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3ymxkshtr.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3mrzkakvu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oqqgxngl.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3zofbyahd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3kqdboahd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3jtsfqbko.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3jixsakem.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3jjyewwow.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3afbbctrt.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3mnbbmexz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3qqnseree.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3bmsemgmq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3uhagkmww.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3woxgocsb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3anrrousc.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3bubcdqyd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3mswgbfoc.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3llwwxkmi.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3bkzlamdt.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3ayddpmcz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zpwvgpqx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3povkxptw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3yuklbiyp.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3puxfymlr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3tpxgumxe.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3ecatjjnz.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ncrxnjna.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3exwzehtp.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vexteilu.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ewdfkguo.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dxclmfau.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jdbkpxrw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3dgisifxg.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wgfkdgmi.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3caewsord.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3cnufyyoe.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3htritqjc.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3eqxeoepj.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zharzehj.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3drywdpdb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3giddnwny.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pkuolwsb.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3igqmldqj.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3eulacitu.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3gyqbgxsf.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3wyyfnvnd.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3zdvbtrji.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3bsrqkjln.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3mxmccavm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3bremgdua.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3dzapoxib.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3xralfbto.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3akmdwdsp.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3ghrdyzxx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3ujtswwen.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3kknhydgm.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3pukrkgob.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3vjjfrbqn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3jjzdzerm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3nizsnvtc.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mclxtrlf.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3rjfsggeg.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3afirpowr.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lyfbffjp.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yxxmycdf.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3wwsajjbe.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3kgnahkfi.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3iosvztkh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3zbsxqdls.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3msnxjcgh.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3poqlsrjz.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3fsvbhpnn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3avostdrm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uecbkdws.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lsjorjkz.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yzixznlk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3jekvnnhi.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hodzqvgc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3icjmzhhk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fivbcasp.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3ohfoexqc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qkxdfzvr.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3tckqbepz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mhstszid.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dosmgsxz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3crqkisdu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3tvrpbdvk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3metvxgoy.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3yndawiub.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3zilbppid.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3mwdmuygc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3ipujgbqo.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3mxmjmdtq.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3ewjvjgbg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3ojkuqice.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3pftrprkx.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3nhnsmsgj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3frebzlyw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qlscphgw.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3fqlwnfzd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ncwkleuj.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3zxwgwhxv.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3dulcjwas.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jammuhlg.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3txtqlxse.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3ktzzaaxx.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3srkrpsvg.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3bzyfhark.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3pcskcdzp.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3wimrulou.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3zjuefuxa.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3rdokfbzi.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3ikbbecyf.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xktlrpzi.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mleximeo.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3abyvgolh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3xqqoevyw.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3edxdixox.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3njwxyvhk.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3jfpsefis.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3snawgqxm.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3rrqlkikj.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3lucfdaus.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3hdehdysb.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3yesxkwuo.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3homllgmq.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3bhgaaupw.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3ckyitste.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3rphbvurz.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3rchyzpmq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3oclfixtd.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3gjrwhssj.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ktvileie.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qpbgsswu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3fkvxddyt.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3aveofqmf.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3lbluaght.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3bcrokjoc.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3weyyqtrj.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hpelkmjs.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3bkfcmabk.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hpaetbjl.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3klqmbehn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3gnlugogk.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3tugowyxh.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3clsjiazs.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3ctmolfhz.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3gvngrgdz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3zcfqbsfz.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qarsgmfc.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qyeuoljp.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3mvrxzjiu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3jjecponl.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3tkmceysc.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3jbeowsle.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3jfbbqrqu.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3fkaanmcc.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3mtcgwpkd.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3fowwpiba.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3wqwcxvpw.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rcpmjoxq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3cxpnrxsi.html


<!-- 参考信息 -->