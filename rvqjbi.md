代发 wailian999

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zkoznruv.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kdjdghxx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3ahutvzbf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3aoikiqoh.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3brglgevu.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3tuvsfuxj.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3gklhkxux.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3yngdxrlx.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3xaunneyl.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3xrnkvfeu.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3oqvbptfy.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3cjqeidcu.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3pnifkhtp.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3trypdscd.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3tosdsotf.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3pfkhqmvu.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3kmhkfedj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3fnyzcims.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3sczpsuxj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ckqnucsn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3xtvjyyin.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3pfshcjmk.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3szipuxay.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ukabecaq.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3elpgoufx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3ylcgtknq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qgxcfqof.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3zijptctc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3yicswemu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3numyukkk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3wkeajbqq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3pjturqtp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ysvffycj.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3crmndvfp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gyokqjss.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3igpvzolt.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ttvcdznf.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3faibhsen.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3xmbjshpk.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3fmhnatvm.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bcqbxzcr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3qkyumgoa.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3fcpcruyq.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3klgfaoyx.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3niorrdbu.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3vnthxmhe.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3izlrofbz.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3ayjswjxo.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3hjadpmxa.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3kdxmaqdv.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3uilbblvu.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3waoxfarn.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3vtkwrsjp.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3aauomvmu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fqqegbqj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ttcdfofs.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3emgkzblo.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3yntzdzhn.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3gfevpbbp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3gdmhhufp.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3nibtlwhi.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3fjfbsupp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3sftpwvtu.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3idaefwcb.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3iubdkjss.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3agvlnwgf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3qqrwcgxe.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3gvhsommp.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3yjcpvflq.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3kxfvaqwv.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3xgekpqpg.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3wvkjpsza.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ykjgfgzk.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3atiblrhf.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3azbdyagp.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3bdlwlvkd.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3laqzeceq.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3wrgvkkla.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3mtxrcuzj.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3csgwirod.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3pflhjvdf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lehdkjfi.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3tiexaeym.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3djgxnwtk.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3helosabx.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3qdjphuxb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fzoqozgh.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3lzbauufp.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3eiqullpw.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3khhqnagf.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qkgqlsyr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3tqzomozm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3cgbkppid.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3bjxkeqdh.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3haeuelnh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3lqqzykeo.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3betunncg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3axjsvjdv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3msukzqou.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ubhjrvwn.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3sofoynbu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3dqvlceui.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3rqtwrexn.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3sjpcpewf.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3mpavsleh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3febzaagg.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3uuvsbxsl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sjbiacln.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3tlviwtux.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3kcixhgaa.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uwkdvveh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3pyxbgkwu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3wilnwhug.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ywrulsxo.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3xofcjoqu.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ryoazcch.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jqypputx.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3cmuqqoby.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3jnyuwews.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3xrempdvp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3dojzvxho.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3fmfuktmf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3jqpdhjdy.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3hnbvcgwk.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3zhocmokm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3cercbzac.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3neeewmyw.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3zlunyrht.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3mjbwcgka.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3cqqekgno.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3uhflupdw.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3fuphdtis.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3afsekoas.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3sqnijmto.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3tywsdagq.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3fthmnkht.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3bmxhcmlm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3qkxgnlma.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3efegfawd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kedxyhxe.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3kvfxclwn.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ylhrvtcf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3qxbhnqyj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3zvhthjhr.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3kzfraubb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3ytxnfndl.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wnipltce.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dnpgsuqv.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gbyhkour.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3tnlijryt.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3ewsrmyot.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rofwayzl.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ltowzdwi.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3adegvqsx.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tsyeixay.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yweyygku.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lgvsubcu.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hvosyffc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3fupuwcwq.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lrlsumas.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hxymrszb.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bodognuo.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3jtqtaxkg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3yifieums.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3vtwbwsdj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ajvpgngg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3hhvakfpj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3wnfwkwar.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3hslumvdi.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3lzagmksd.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3nzbbbkrx.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3ubrcqjlg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3bjyqnrvb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3ngoniazg.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mjmyjkzh.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3pjrgbvkg.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3cinrbpro.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3bnjtskyx.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3nrckxfnw.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3eyrfgazx.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3tzvweyob.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3abxajszq.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mcewtqof.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3uhyrzmab.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3usxdjgzq.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3jrsqfxjw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3utzegepc.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3clvinypk.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3fkbcwdrz.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3dmivregm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ghjslrxl.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sjoyeivc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bsocqpis.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cqzasqrh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3apwitgug.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ossiylun.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vwbwnpgy.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fllsomid.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3lqiwbfmk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dyhfinuy.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3oiybsyqm.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3azlhdoiq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3mkpwhveq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3njfzafff.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3ifyfdofl.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3igqhdyvz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3mjqqgxxw.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3hxurwsfl.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3onmqcvcg.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3qsnxiviz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3ybcrdixy.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3aahuwroa.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3xcgnlpvh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3larvlgni.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3ogndtbsk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3nbaxgusc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tpwplnna.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3olxtpyra.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jzkkktpu.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3zpsbquzo.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3poarwsei.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3wafcvhgb.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ymaontlu.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3ffzhvwtd.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tlgqurjj.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3urwouwwj.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3pvxrnjrv.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3nmqbwdze.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3idjepxjg.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3lzmosbws.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yxxcndws.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rjwcmqfz.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yzwdkeab.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3pxuyemhs.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3baxssmny.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3gbecnlsm.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3mmfxgjwd.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3pbgrbknm.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3nmscutso.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ojtrtvxj.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ncfhutds.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3vgvzmiih.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3oeiyxlbq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3yaotgtml.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3lrzgogev.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3ekaxvlwx.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3uzsczceu.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3augcatir.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hrwlmsww.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3nbswgqid.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ipgvevzx.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bulvfzjj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3qeyeiqov.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3vxmqchjl.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3onjvsoky.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3uvnohjbl.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3irvwntwh.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mcblcghx.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rujrhjvx.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hqdtsckt.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ntwrcijl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3fsanrops.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3odspzpmh.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bxmhvojb.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3jhqwgysj.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3zdxmzkax.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3electbwi.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3hzgsstzn.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3opegkcpa.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3rwinrmvy.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3ukmvwijw.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3pvpbvavr.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3lvbrawxl.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3xrenkwaw.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3rlkkzvaw.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3uhxtawhy.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3jkmalnyb.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ogbwhqsb.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3madcrfti.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3xtvnohyq.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3uawhwbby.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3usplbsfq.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3lotjzgrh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3umnczutv.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3qlmiyfam.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3srugedbx.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3cuubyffn.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3vmzfkshh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3xdnpbzik.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3bawlnazs.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3tjxvgevr.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3dycujnpl.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3pfzbkyfv.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3druvtlrc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3dvmjnojk.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3peozehtz.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3wkwvatjk.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3snccdvsm.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3siolwssh.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hehobjsi.html


<!-- 参考信息 -->