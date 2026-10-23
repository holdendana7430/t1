代发 wailian999

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3tzwiqbpp.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3bbjbgnfv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3sllqbnpp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3aqcxejnm.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3craswfrl.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3eqbtbznt.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3wbxlprdk.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3nstmtieq.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3itadpazo.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3cszmzhfd.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3ujgjtxpi.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3apsosher.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mgirmhxt.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3nbigatbj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3rarxfuqc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3gsbgqbzf.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3nmxbxnhw.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3wcobspbc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3dcvolmkx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3jdosathp.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3gadybbat.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3yvtzqqsk.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3hkpgvptf.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3fispmgjy.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ctubpqbq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3iyptkago.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3zwuuryzd.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3loudnqov.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3ecdnpqgm.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3bxbgmdam.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3smngwqhx.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3ojinpcef.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3cvcwcvff.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3lkzzgwxl.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3ipvbhcup.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3tplerthd.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3tqfutipm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3qfpclidg.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nkfayqwu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kqtmwfrx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3lpxaaggc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3qfpqqfgg.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3mdmzupss.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3qcjquaeo.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3fjoxqqvi.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3bldirjix.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3xsokbcex.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3sfslxqam.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3vbizwkek.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3pjdmgnjy.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3yhiuoqyw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3nqvzlalp.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3ljoffnxh.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3nygrviwp.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3yehyarwo.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3bxopgutx.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3kslyudab.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3crnlzkbb.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3jjilxdcq.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3txhpewwf.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3azzimxql.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3irkhicyb.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3wuembfma.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3uisgvzyy.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3xicbzjwv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rdcaknrl.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3akqnmkse.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3pmwdbplq.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3ktnnjzhc.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3xweapzza.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3vuhwuoud.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3uzdcieff.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3gtakoxun.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3inghfnrp.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3mgyadfgu.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3irraicip.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3sveitedi.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3waptsgku.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3cihqkwtq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3dnsfblrl.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3gmtkzbjn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3tbqqqcod.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ndytsxog.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3cvzidbgu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ezngvncq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3yksaebfu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3dabvknow.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3cdwjhvas.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3zmpytlce.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hpcjjdaz.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3eeorydpr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vxnnjskq.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3vqqgbeuj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3eajlxyua.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3npickwbg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3deycgtes.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ityhjynr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3nbdtlkks.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3doueaupa.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ftzfxrcf.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vogksjqa.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3ucjqytfr.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3ltnrdlet.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3tuubkzdp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mjpbqlic.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3nawvfyxs.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3kssludcz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3wwlbkraw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3lvrpusbx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3kwiysbbf.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3hyhuaquq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3chyotycw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3zcfhdqns.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3wbgzunzh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3nvhpgbov.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ikwgvdad.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3cwaremzd.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3gsodejth.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ynfpeddq.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3hjdokxth.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3xmjulocn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3sizhmdww.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3qtrneyyi.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ecbpcyuf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3mwhsticx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3tdzffaft.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3fytlqsyc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3lttozxnr.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3fapuhyqm.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3iqiamlob.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rywsjkfl.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wtkxtiwr.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3joktpjaq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3xfaifydx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3vcmhdcjy.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wdarvlli.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3boaaegsb.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3usjzvouw.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hcikklie.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mmyoalsi.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qzgfgwil.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nlbwxmol.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xsmdtwhp.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3utywffbp.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dudprpke.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3saoaxjbj.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3swyoaiez.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ziiggakd.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3fgwwfjyk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3gjyiupqp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3eufwuevl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3olwnajws.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3cqclnfst.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3vaivxxik.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3kdmbcbac.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3qqymtiyv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3xkfkdehd.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3glkdelhj.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3uwivfgaz.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fgilknoa.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3vsaticrl.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3tghnlfrp.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3wldgzake.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3aohjffqf.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3zxefulhu.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cdsfggdt.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pzvjjtfb.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3aohxsdyt.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3cphprjbs.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3roymxtko.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3gvwwcrng.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bfxwdsbr.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3btawyjrq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3rlshnydi.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nwcjxphj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3opsvmimr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cqyptnkh.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pgjepjin.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3juulgiui.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qyhvnpyg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gbevoplx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vnkumhan.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3sufviyli.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dmmkxnfc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3rddtwjeb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3skaxmlfk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3xfxfykli.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3xgeuyowt.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3zqfeztel.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qfydqskh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3detmvkzq.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3pbflzmad.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3pzjzzioq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3uyzsudaz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3skrclbqr.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3ijahxgpg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3liirqbjt.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3nslxwqtj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3kvehbbts.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3vdswdzou.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ryfpzrdq.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3rlgfdaqu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wroefgeh.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3sujvoeug.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3wzxuwvox.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rmghumks.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ztwhnqdn.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3irnutwky.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ndmbaein.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3xguoqhiz.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3kyfjypiw.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3fftidnmc.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ybchznny.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3waddfsij.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ezxxjzjn.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3drvbitni.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3gkqvsben.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ovztlavz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3ctpyayqr.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3gvkfodse.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gdpplgoe.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3jifarlqp.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3hqfrjwib.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3cfgsalml.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3idjeulrj.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3mawmapxb.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3cfetomkc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3unbihjui.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3fyxikttw.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3mrsxpvql.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3xmvfmqwl.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3uhietvwe.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3fweuzzsa.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eadiussl.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ywvqutoz.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nsfnbhsh.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3kdrmsvcl.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3yqhidcid.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3kiezkwxb.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3nbbwtlrn.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3rmvwhobv.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xzqasyim.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ekcjjaxh.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3nefrteyt.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uscakfix.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3brpndsrr.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3msqbzurr.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3qoliiqyi.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3daldcggt.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3zdtjlkqv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yzeftpgj.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3vdpgcozj.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gpgbuimj.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3xtizxmnc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3awpbusbn.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3hgxoaipv.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3qsirarhu.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3blanelww.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3syocifmd.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3qexftccy.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3znzwqluq.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3gasyywux.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3bavpmiyi.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3uowxlzdu.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3mubeqqjy.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3hjygpvdw.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3leqnmwkt.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3mncdsbdn.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3bwkqlepz.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3ohcrnorf.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3qjhvajnc.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3bpoeyfxz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3bxwqysth.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3pstudkvm.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3ircftmow.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3trcanhds.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3cqitpcca.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3mwrrmgjk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3vmyjvkno.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3wovbjwlq.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3imsjouaz.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3twwftwej.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3byvdvjkg.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pnuulokj.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3chsbaien.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3kmipdmwv.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3itrbfmmg.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3ifidnnvy.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3bnmhhdis.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3vpjjmevd.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3ksgkkxza.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3iqoqcokn.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3ljuudjbq.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3llujlkpg.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3mqkmlzwg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3gjrtitjs.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qkjwiktv.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3unokxtmz.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3oyeihnoo.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3twkfikqv.html


<!-- 参考信息 -->