代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3gqbvyuxe.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3zhxrglch.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3rsobcgpd.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3zywiadbp.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3gffnbdxo.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ecnzavgi.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3xnzkfcnd.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3llqomvpu.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3mpzydyfs.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3eoxkxjuk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3qfzausjc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3dpbmxglt.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3bifylkox.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3terupaoi.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3wdqwhdot.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3xpgleiki.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3eriucrka.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3kmhxonwc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3mdnlpdmt.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3dacoiefm.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3sfbdyqoz.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3zllxntvu.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3nlewohvr.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3fhqxgvow.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3gcabzral.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3szbfgaco.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3cnzsstga.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3wqxiyqfa.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3ghdlavbm.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3khussraf.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3vufsspay.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vnnrffed.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3mokwxzhi.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3efooalcp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3qnmabcuv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3fvjhiunv.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3cnelzdfv.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fdbqhoes.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3abugnslr.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jueuccin.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3ozydqdkp.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3olumwwug.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3viyxrjmh.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3ptjqhqex.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kqmwfdjp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3prtxeyvj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3cialqvqz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3rjugvwix.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3qldckbvz.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3tuhotmch.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3gffdiaez.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kayuoslt.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3gikvfxqv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3wqzghqhw.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3vnlfzuem.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3grtjxasv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pegeuaib.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oourglff.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3qcqkdhwq.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3aphptsrj.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3zqcxbfam.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3cyupbpbj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3rdpkvxxg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3agviblle.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3rxqwzjvb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3essxnbbc.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3sbfyquke.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3klpnqwkq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3snjvdvyx.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kjfbavgu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3fbxqkigz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3pvhsdygs.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hgbxscud.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3dckeufse.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3dmguaiqk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3zxoeruup.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3qftckyip.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3pquktwfg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3hbivxgxb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3risfrmcg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3lrjyegvy.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3tizcfkeo.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3vubgidzo.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3phjkqfto.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3htmnuktn.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3irjakpkm.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3iaxqbubz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3psdrhlfs.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3rtqitzst.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3zpbkxkzk.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bxeszijl.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qvnejjkn.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3kpoldbfc.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3qwcbaozh.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3rauqmitj.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3qxqhqxek.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3nablekob.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3kheqanij.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3imtomprd.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3fvsbgtvc.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3rhdqnmgh.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3wchnctwz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hcvvyxwq.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3xhqirjxw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3ooofmoxt.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3gyrhlfzl.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3bnlxnjfl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3bgdwnkrf.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3aocqzyep.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3pnqbulaf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ndbkwumh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zyuzavtu.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3unwkfhyg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3itylhntv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3uknziqgp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3vwcihuan.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3vzekakjd.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3spzkovfx.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3yusvmzyu.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3rofdaifd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3kujcjdmf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cvwsanhw.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3kxlcgesr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ppvmykoo.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3nrovfsqu.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3qiwrgymn.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zuyyeiek.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3mrsnxcac.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3cxegawge.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3nuyjaoyh.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3grflswdx.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vwrhoppt.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3amxehirm.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3rbccyldm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3krbmxamp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3jqtxnsvf.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3ljlpsjnv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3scnbbvzv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3xtmwbtzp.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3yootlbjz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3gtgaxquu.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3rgtqtnxt.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3unhtvzbc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3jdhcqmys.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3vcwybxnv.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3wvnuuftc.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3cvnkyyeh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3jnzmumuu.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3bizyxlud.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3qjhihxge.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3whokxtcr.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3psrrvrel.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3cacthgoc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3dhxyentr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3jckkuyil.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3wxbmiwfm.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3nltlvciy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3uvrwjavi.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3jjlgpdui.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3mzrvrnqt.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ycptgola.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3rvvapeop.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3abjzjreb.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3alovrlkr.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yyphhhvi.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3tndhfove.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3mizwxnin.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zwvvtkpd.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3elymiyej.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3ggofsgzl.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eubftfyv.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3csaniair.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dygrxdbc.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gkztdftp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3sxmakbxu.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nmsqiywa.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3slhqatbg.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3enrhuicy.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3cotgyikc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zbxcmtkn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ztrnfvvc.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3qciordqf.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3hhsxnegj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3dfzfivwx.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3ecshscns.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3dfknyrpv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3ptuqktuh.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3nbxnfhbd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3eylaclff.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3hllnlxqb.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3iqfvksdg.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3urdioawb.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3omvuflow.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qsvgetvy.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3nxrleuig.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zovoedbc.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3upzorlmw.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tplejlhx.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zbkbhiss.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3dizuvffd.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3gqegweop.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3vfztefik.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3romainii.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tufnelva.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3yhimehnr.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3xlvyhoxs.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tfjkywux.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ylzbzqki.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rlroinfg.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bqbbdjsu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3uvqlzlkn.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jtxctpxy.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gvfgyuuh.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oqsxythr.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3ykmlptic.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3rlecwlbt.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3gowbymox.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vzjrhigj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ndfituwl.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3iseeknkq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3yiijnmyn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3fkxzrhko.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3jiymikwq.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3lskoisth.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3yyofkhyu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3gpbzjtmn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3yvhhsamc.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3fsvzuirs.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3atacdmkb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3gqyrjgah.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3rajkyqoh.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3ksjpzujq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uacvyjzc.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3zkfmnqau.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tyjxojnv.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3dyirxlni.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3izigazxx.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3socykjfk.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3qwgzxvjy.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3endaunaj.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3sbefoqfr.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3jxkbcmze.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3mxkguyfg.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3rfeexodm.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3jwufjljd.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3zvpagtof.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3qvmxdymc.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3mxvjqxau.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3inzepiem.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3dqqxllkb.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3qkgwymss.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3idrakfxt.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3whjbdenf.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3qxdamauo.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3zoblthts.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3yflcntvn.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3hcnavjwp.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3firfnmfm.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3eaumrzyz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3yqbnvmdm.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3kqvwkguf.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3fkwxddyp.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3unmsoklr.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3cditdhay.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gttqqndl.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iyhwfony.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3trfmrnwk.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3sgmsvdtk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3erosywyd.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3xcdkalvh.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3slknjpjz.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3cjtucvjg.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3cubbkekv.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3gdtoxwlo.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ualvnhbi.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3rbkkxhuw.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3wvwneifm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3zwwbltzy.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3befkfwbo.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3krjstquc.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3hpjdkmet.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3vbsactor.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3fxeptpwy.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3rlowqdlq.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zoitzxby.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3enfarnnh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3wtbqjkkv.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3vnosplnd.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3wnehohoi.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3qldcxdwv.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3nggiofwx.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vgondpmz.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3oyjrkttg.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3aemmjiij.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3rvqximrz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3plhwnoai.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3myfxmdmc.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bjlfqres.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3eisnazfw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3bhzrmogk.html


<!-- 参考信息 -->