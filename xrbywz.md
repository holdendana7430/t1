代发 wailian999

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3hpozpnjj.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3fswxvqlb.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3saulgaqw.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3niesdwtn.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3eenuaztk.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3vvhexqrw.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3vgpkebgb.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3uqcfaamk.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3hrbmmncn.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3hqshvgfv.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3xlzymgav.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3ejbikkeb.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3toblviym.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3meevmazx.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3gxgjkuwa.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3wqjzaloy.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3yuamhmek.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3vqidobqx.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3uyagcedf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3aafxsntk.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3fbhnnxuv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3ghbatjar.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rnqzzcfw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3klfuavgx.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jikologp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3wahlzwtt.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3ecmrfujh.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3rjtjycnw.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3iqevtxhc.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3tgmeklmy.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3witfzzea.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jtzbrtmn.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3nqawbhid.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3mhvuljzz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3joqqsnrm.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3ptkphmbf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3imcqujpl.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3lncskdrh.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3tazmrwdi.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3joblgpzz.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3kazdexod.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3wlzyahml.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3wxclwkuv.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3fzcgthhs.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3lrwbdecn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3awjcljpn.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3wlkfnlzw.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3uyzifdta.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3mgaxlapz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3twjhhsnh.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3orhbjwgq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ctftdygq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nfvvvdcz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3bwkwylnj.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3gyfkrmol.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3szpyugno.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3cjsrngwm.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3ttgfsqza.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3nvjrmvrd.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3hviwhjzs.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3vshkvwvc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3urzbkbue.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3khfqiyae.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3vefmdwfl.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3rhytvdca.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3srpxacep.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3teqyhatj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3sjduagut.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3onkwyndm.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3zgixzayj.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3dygterxv.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3iehiscwr.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3vruxlxsd.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3qngpbuwo.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3xfptnjll.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3pvpbquwa.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3ztdrlfqv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3vqdupowi.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3mtexfugc.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3qtlohfzm.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3pagshbwo.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3xmqgsyim.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ekfzchun.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3budxtadp.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3ulvogyhg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3lnbmtwwy.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3smlovbuz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xtyzodmb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3jyudyfqw.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3ueegwqoy.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ojtvjtpu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3cgciboqk.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3wehwqjzd.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3aenknwcv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3fgjlmvkg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3juamvjhe.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3wltpmwyt.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3irjggnms.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3ouxsuyjq.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3qdhoyown.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3jkpbiach.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fdhzfacd.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3nttfphfe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uzjsynwm.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3viijcpur.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3mbivnqem.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uofutwqh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3vbcopkpd.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3vslvemct.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3wzhonuxr.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3pgsujjrz.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qnheiibi.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tszhkcha.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3zbjyrkdy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3cfqpzvxt.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ynxinpdr.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3rxirfluk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3ecplgwbg.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3jkkcpwdb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3xjrbxazs.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3qvmbukow.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3gnuhtqnx.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3ffkvcaxv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3gbhspmva.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3avkpdosy.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3sysghuok.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3csgzehub.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3zsaozuvz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3sadptzua.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3bstpntat.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3npwzlpgt.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3woewhttm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3sdduscgd.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3rrktrinn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3agsshcdo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qdppoyrq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3oocmwevd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3tigqxaci.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3cvyxaugw.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3jrxmywge.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3hmimgbvb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3cekzjbeu.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wzbvdbcn.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cpxlvaad.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jdlmjosa.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3otnojjdf.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3zmjcuvtd.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xzppvabb.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3goiuwqlf.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3ylbbeuze.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cjzfnvdx.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vkhcrggi.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uiqnqifr.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tbrlinqs.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ztyqfvje.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ukrjapml.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vmfewgfp.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3avtguqyj.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3kkrfvcwz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3zhgtmwez.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ervqthnp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3hjadpxlb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3gqnklbrl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3euvekruu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3sludcegb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3zkyteokr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3jrsxfhxx.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3omoetglm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3yegupnuv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3hbczxyka.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3dwhfszrk.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xzkdszhc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3irhxerrq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3ruunjdgj.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3tijllxxv.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ulxrdavh.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3pxhckgiq.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dvlgnoqk.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vzzmvfts.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3vnmmuaxb.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3sxeghzna.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3rkqghjef.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3dckwrpbb.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fvsfilsc.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3brodlbzz.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3oevnawmt.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3szlkczkp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kpnxgtql.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bonssmli.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gfpqeayq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3lxguacss.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oigcdrrf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3htegfskj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kbxwtgxz.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3mojuhgom.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3jvpgegwx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3tzbzfpoy.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3gidukllv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3wkyrogho.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3nyljwpzq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3bgaygtxe.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3xzbmhmdl.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3dtxhbvjy.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3hvxbrlnx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3gpcmxjcg.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3uirutnhb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3ldlyuyko.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3npzwmkdd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3muffyled.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3aanwmgoc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3ilrulwjs.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3cocaulej.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ejbtbviq.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3jjcbqrjp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dgmxvent.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3nvpdgcsy.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3iatwhngf.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3khbaxdhd.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vsodclnf.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3ceblssio.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3cnqdqrnm.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3ypoxjawg.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3acvjdnon.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bltfgepj.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3kayssovd.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3qdtxhivn.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3ejoafzob.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rmawaqab.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3reboxmzf.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3zuvdauqe.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3pkaznole.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3kgljsvwu.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3otgmaspv.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3unexnhzd.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3qeanjixn.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3aczwbzjo.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3nbbphzgy.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3jvzdtmdb.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3zsvgzzbg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3zmaodojf.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3dbycnkgc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3gygunpmv.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3rsfvnkts.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3lhgrsgxx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mwtagyfn.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gpwnljhe.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uqppxpiu.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ilmypyrn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3sevbzanf.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3vkprtemw.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3jwtmpqan.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3xdivzmql.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3vvsivokq.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3soojxodn.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rooxwvxs.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fdbqbryx.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hjdnuvfr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3suwifqjy.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3hsmwdncs.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3wmsxwgad.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3rifhihsk.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3dcxriowm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3kdazxzwb.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3nnnvwkhj.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3arogynee.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mvhzmqom.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3qudcjacy.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3ayolmlon.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3plovsigc.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3lynwbgat.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3sjzibmir.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3kxevppuq.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3pskhjrly.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3oqiyivjk.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3fjeyqjfe.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3cjbsmsmt.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3txxkwjtw.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3yppbrypx.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3dzudxqqc.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3uoohgsfp.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3kizngrez.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3rfrmqvey.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3ynqqlicc.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3griowkpn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3yomqlrxk.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3crwdqhtv.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3skqrzmyf.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3ddkldozv.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3usjnxkyv.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3powvuzry.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3fkltayyj.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3nvvgtebi.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3blkhjekr.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3ynlejfad.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3hmfqwxnk.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ekketrqp.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3ocsxlqkh.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3vmtthgda.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3cfmkyvle.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3opweduyq.html


<!-- 参考信息 -->