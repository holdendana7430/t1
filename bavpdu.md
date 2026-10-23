代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3jybdcwta.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3lufmwofy.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3dysdcyyb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3gmrbuthh.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3blvyduzy.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3qnnpgwji.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3twfouvcv.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3cllnwojd.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3uolwpqxo.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3yyemsdkq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3hgjticub.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3peztapke.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3efbhieaw.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3aikagiov.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3njuyyczz.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3edmiovtl.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vkarudum.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3reppzakm.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3tjvygqav.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3prkecnbw.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ekgxshbv.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3iwlylpqt.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3dgigemyf.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3njvhcjvu.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3likmshij.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3hxnlgoia.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3amrrruug.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3nsjvdkph.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3wpvpiypr.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3rpqwkbue.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3cvxqygnv.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qzoldgta.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3krnogtwn.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3vuzgyxlw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3rdtuzfkj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3vosrxmtp.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3udzidvym.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3rkvdeztm.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3iwviwgmz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3itgwbulk.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3cldldbsi.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3gfstxkgg.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3bwvpbnne.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3gjyopuuo.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3mlccmwks.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ikvsjcnn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3lbajlrtm.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3ssfwundo.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3mjggbeqs.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3lnpsgtto.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dylwzjtw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3aspgthab.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3ghwmfoto.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3uzhaeahh.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3lcqnglxm.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3alsfxmrt.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3drktrcod.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3hlytgyfq.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3zfxxgxyx.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3bcomuyga.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3ejhmxxuc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3hqllittx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3bpqquijc.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3oizhvcgj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3vnuxpjcu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3ilavekly.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3iwwcgdsl.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3rngmtjxy.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3mnagbegs.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3lforxlzl.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zvkafonn.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rfkaiiye.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3cuxwrujy.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3hgitixmn.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3bihkxxwj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3szqjvpyu.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3tqspwqwa.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3eslhuolg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3jzkrwpok.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3icsnlfxz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3tyxmayzc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3dxqivosd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xtcbechb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3zniytabl.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3rnvsclng.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3higdvyub.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3pjlmoycy.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3mbfvxsxu.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3mcfqdkgp.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3bqsjviji.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3dzsvyyly.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3figjzuoo.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3gildjwbv.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3pupuboee.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3ycystquq.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3ckiyphlo.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3qvnjzsty.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3rxsqaowp.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3dbapjgkk.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wgjfyxbs.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3ltgrzlpe.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3ejwftlja.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3sppxvynj.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3nfeeixez.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3gnbrvzel.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3qakebaoe.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3dnwxrwes.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3bgpjlsbs.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ypoeqcet.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3uvzbxgps.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3agojgjma.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3bfkmjtju.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3nkyotewb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yvvigloh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3myomlcbn.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3zkttaavt.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3euaiuryj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3skqmazqp.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3pdsmnmjo.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3oxkmcsyu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3myyxfvxz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3varsaodl.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3uhzhpwgr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hdceldzm.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3hxkngzsf.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3duthqivp.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3engajhed.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3zcmtseda.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ephcdvxf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3metqzwdg.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3tyaznqcy.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3apxsdakm.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3exdwpdmr.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3rhvytjot.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3ogbvozfy.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3ellzwajs.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3mmicxvet.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3kfrwjfhm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3jxzyqkij.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3xtxaxxvz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3ugqdwmkj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3kdopowog.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3ydkzimwj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3inmyzpnx.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ofadzpwu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3iazilehf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3jophzzjq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3akzyxett.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3iqbibpzf.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3rixuweut.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3cnryzykr.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3qhzzwvae.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3joeawupy.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3ftzcustd.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xdmzgotl.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3knekhxfo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3zjakjyqa.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3lgmfegxr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3uzfcdemh.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3ielnxbfc.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3tshsueoi.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3fhbtfsvd.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kxjmgdsi.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mhpupqff.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wjgmqimm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3hmiefvds.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3vbsgohlq.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cwpahrbt.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cdzsbhyw.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3nyschews.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3olikokly.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jezmjtuf.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vduagvba.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uzdugaxe.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3uxxkofpj.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ysuunhyo.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3txjnmocc.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bczodduk.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3yqusolqu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3peykezek.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3rpdbpmoo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ykadlofh.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3gkhhlork.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3ljnkecei.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3yrlaneyp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3vdpyqejg.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3vxrytkfx.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3zrfeqgrd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3bptomdnx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3dwjrmxjc.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xvoipmgr.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3aixtsoxr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3cnndodyk.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fayfiame.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qxzmwcwu.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ggjitvfb.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3bqhurubf.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3msxcofeq.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3reoxcjwo.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3chinqsip.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3lgphbqhl.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ailmqtos.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3tgtzjqvj.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eijpvrnt.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3tusxamgu.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3inrsmevk.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oymdzupk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3utywseox.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wvwuasml.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3auwtlcha.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3ipcgzxnr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ejxdbzza.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iyjfucmo.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lisswhwe.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3mlhfgria.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nxgdzwvm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3fnmrhzrv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jrzhvspe.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3fzrovucy.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3tjyrgvfi.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3gjgypnai.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3uaczuthg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3ywrodcxw.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3owbdcsoo.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3bdnnmjxa.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3qdswuevp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3nbfqorvl.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3elizeiwi.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3crewdfha.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3kmkevhld.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3vfzsamkx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3itgikbyv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xuoqtdur.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3xetudbid.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ofqnkysb.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3uoifpjlp.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3lzgzxppp.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3xycyffpf.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3zaezqzjc.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3ygqemwdk.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3awcsjfxn.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3moapepsh.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3ksbssrob.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3yupedqog.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3qqrvrjur.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3gmemegvi.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hiehtkqs.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cyhffdtv.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xidtqliv.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ebfruxfh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3xderfzea.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3rpkxqkwi.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wjncdsgt.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3ulswsrxe.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3hhyubleo.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3lvnjxcje.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3yovudrce.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3knmdyhsa.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3kcumrbzt.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3lmaqmxvm.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3diwnlpur.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3fucyfjdt.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3xkjapabj.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3esbiyikr.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xdikklwq.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qrgrfvfi.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3htbtwfpv.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hivmjtsp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3wmcxuuds.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3xcsodcfd.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3vradfssx.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3jjhnnthc.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3omlbnqin.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ocehtzym.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dhfodjmm.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3gvigtzdt.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3aygrqmdg.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3yjhbzahq.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3bubnegox.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3yvibsnyc.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3rsozijof.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3xsncklvc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ffmpilli.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nbouaowj.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3efvhafjv.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3fjjnplmi.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3wexovkop.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3gpapjdqa.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3okbhrdiy.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3tziqohnv.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3ooxkclps.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3uvmzemqg.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3sadvcaey.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3doxnkvfe.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3zssxfcdo.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3jbgczpod.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3sdwzggar.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3tyfvceql.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3hvskifpm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3jpxihslw.html


<!-- 参考信息 -->