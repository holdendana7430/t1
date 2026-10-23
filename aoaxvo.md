代发 wailian999

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3ecnjtwlm.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3jqbwbpdp.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3heorfyvq.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3skuvagjj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3zffqwied.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fmfgxtso.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3nvbjshne.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3okspwjeo.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3hgoidkjy.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3rtyzetho.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3yngenfvg.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3gqutcezg.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3hckvdfrq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3pxsgtpfz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3qtehjmwh.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3zkxapnnz.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3savutmia.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3wdardmjv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3zlvknhnp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3tzkqvchc.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3veeoewms.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3cawzcvkr.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3hlbuomlr.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3houmdzdx.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3clcabqkr.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qfitfxkl.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zftwvumk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3aaflovjn.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3surzwlnf.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3rjeocbtr.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3dprlfkqp.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3svmlovvq.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3qgqywuht.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3qcydkyia.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3zzrymfqv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3rcnmqeha.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3gftewzeg.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3emscgvio.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3bbwopdjc.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3ymunkvwt.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3moftlbrr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3hpjenzlg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3mjzkpfug.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3rrhvblsw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3lkbsiske.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3oorwbmwj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3iropyxkc.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3urnpwmgw.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3gpfmwjnz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3rqnbwlpw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3clhwydcd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3apkjldfa.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3eprdqsow.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3bwhgnsqn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3wwuipzfo.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3nctvzgko.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3saprsrbf.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3gqbmujrv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yvuofmdc.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3luexxbyg.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3zweopucz.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3hredbjof.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3iiwwdetr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lowlhsig.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3fgkzlxvy.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3nbmwqnzk.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3edcgsatk.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ktyxbise.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3wnbyfnrc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3btbkkxax.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3pqmpbclm.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3xxjsqqxo.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3mwiutgae.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3fwfslntv.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3nkihmhpa.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3thmvwowy.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3xsluiwnk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3euybpprb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3htmjxpkb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3vnlmlcug.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pxtydsih.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3zsmowldv.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3jjarhfsc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3nhdxgelm.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3fggagnii.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3dggtebdi.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3dcpohakj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3gvxkrzjh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3jdoyzvai.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3qngbsprk.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3cxklrpyv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ynsqirxh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3tsmycwzx.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3xuwuodgt.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3aktgfkuq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rhcolksy.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3itveiqmr.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3tafuicov.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3qfizszft.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3wxitcykd.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3tvswuhdz.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3lskmrgif.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3jjtyvxvl.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3otvfpujf.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3diydwmxn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eeeahgpo.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3svumjjfj.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mqornlpf.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3tmcdpgmp.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3beistonx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3iwawchjk.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3uknkubhy.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3oqsdtxuc.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3pshofwwy.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3uqyazhdz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3fyxkszvr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3rbwjagbu.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3pmdytygx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ouvbtxqz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3uysbooux.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3dubzsgqq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3xkdeolfc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3idserdai.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3oakhpzzo.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3psqslyll.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ncflaqto.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3cclvdinn.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3abqaynla.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3rdqueoud.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mtspultt.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3bvlsssde.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dddvwkay.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3tjhmlrov.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3jwajogfr.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3stmtshkx.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3wdwwndlg.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ssqmhxlt.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ouhusrbp.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3cqqifiay.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3todcfajs.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pawfvuzn.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3ukanvevq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3knbiyvos.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3smafjbwt.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fhngkjav.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3nczfwnmg.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3jzbsutqj.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3etmymykz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3xjnuduxh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3vlzyyrlt.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3suzftxle.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3bqsrjiax.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3utyldnbv.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3wcfpizwy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3kgihpaom.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3vmzdscee.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3puveviux.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3sdmjyvze.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3oswraufq.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3qzdansee.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3fsvmboyg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3chjlpffe.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3chriosel.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3szkhphoa.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3kotutcpa.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ckefneol.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3oafvftqc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3syzuvxax.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3sagbyckd.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3mcoudeqd.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tehkzabn.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3htzunjwc.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gjwyubmu.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3yeddwsye.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3mgwmazlz.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wskqarje.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yzlisutn.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3vcpbkanp.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vtgnkgvx.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hputdson.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vazunurq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dztewlod.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3wogrlefp.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pbxmskob.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zmjhuyxd.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ogphppuh.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3hwuxbxfv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wfrzoekq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3fzhahxhj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3wpslbxwj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3vfhilbjf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3qypqozhr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3mlawzfyz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3emmvtzns.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3xifkweze.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3qieepcgt.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3corqjdws.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3ukjxsahl.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3bzyinoho.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3aqimoxok.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3jzsvbrhj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3afjokljk.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mbgkmexa.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ezwjqyij.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3bpdtpwej.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3adosggsr.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rizzjxsq.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3raqpsefw.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3cvtdnmsn.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3doqzlvob.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3ugdootep.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yfwodbyl.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3vtablfvu.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3jsqgdudq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lyzpspkp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3abtekyzb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ddiiomrm.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oiuxmquj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3deeozgwp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3edoksauy.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cvcbommw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xcuhxlwu.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3qmyrdvrc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3htwromxk.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3sjqcepmd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3adyewhxp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3oeqtcafi.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3fgdibgad.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3inqwoyck.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gaqaqnhe.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3imxdqxhr.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3rvmjszkp.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3bxnkwwyx.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3vozuhcrj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3kjkroyvz.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3ggnrfqif.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3tshzuujy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3mxchbjjm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3nhhgcflq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3rsggnmmj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ctghjmrs.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3hwmahesq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wrbgusrp.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3zosktxaa.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3nuzfkwbz.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3hjaexmln.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ovbiqcnb.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3asdmevtx.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vcpxdkrd.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3irgcsjso.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3ddbjoyjj.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hddosity.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3hhxqqldq.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3aiidqynm.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hbkphyxz.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qccrfsne.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dreuwhpm.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3cznttfed.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3mncyvecd.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3qgbxivrz.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3twbxnfxh.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3fbgxsmov.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3fjhhftrx.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ptwtjqlu.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3cklvscwd.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3celxcgut.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3zftoiqzb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3tolctvux.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ncspjnfy.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3zfodxqub.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3czcjysfe.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3gjkazmel.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zntiozvc.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vlfiwtgp.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qwixstis.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3pdsowmnk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3mpfudeqq.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3mxztoptv.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3pkpdoijt.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3kmgbwmuy.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3txxwqszf.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tebdgkcm.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3gwphlivk.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3dyteskcr.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3uuubzjkr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3uffxfoyq.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3qmdeggmc.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3ewgdiazn.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3knnvwtgs.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3brfvfwgb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3kvejmbub.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3yvbdcusp.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jqhcwqwg.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3gucxnsqw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3zmpteols.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3qsslnpsq.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3mcxekccw.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3jngdekmt.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3whfjdxhn.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3pytqswwh.html


<!-- 参考信息 -->