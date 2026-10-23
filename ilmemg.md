代发 wailian999

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3sjboozkc.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3pbioirir.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3qqyraatu.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kwwcilfj.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3htxtvifq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3ixrdwgnp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3azjwiqjz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3jcwgyrum.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ketusshz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3gnkthstq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3dtoptfmt.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3nyrwmtvb.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3kqeprhag.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3zoqfjvlg.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3gbtqngeg.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3ijtwfjfc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3omubdnbv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ayflepcu.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3bcwlawdy.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3obxqcctk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3lktjkmew.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3uisnvkml.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3cqdopisk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cpydpnlu.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tzdtauzm.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3ybnjimqz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3sppcoxes.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nylndnmz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nnlnyrkt.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rtswbohb.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3xbwiduqg.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3fzztgjwq.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3arxyakle.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3wmklvicr.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3dtecwjtw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3nkteuywl.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3gbcsbdxg.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3erryxrrg.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3ntwibvbj.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3llxtaacp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ccvmdgsg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xxumgjgk.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3cxmvwcax.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rpjddsxq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bblkfvan.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3wxjqpdjp.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3seeuhcsj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3cwiovjec.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3ocqpxbrh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3gvsnovgc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3dwsshskj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ejvpyzsb.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3jvpsovha.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3anpjpewc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3vdwqdnqr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3vgrsytuh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3jkonyikx.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3hgldgjem.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3bzzlkpaj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wgbbgzkz.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3cxnpdadt.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3nlqmskxk.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3nwouirez.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3lrsdbemf.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3hatdxowi.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3ebxxoleu.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3xkprrpxh.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3dwpzxgbu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3qlmconhb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3ifygwdfw.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3fqmeewek.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gwyizynr.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3mqvycfeo.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3rvwlwyzp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3evbusint.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3qwmxrtea.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3kxohuyxw.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3jlademng.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3mqphfhwr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3mpgvhcgl.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3naqohoti.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3jyotjkdz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3opcphlvp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3krnhlsfg.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3rqpxwgfk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3trfopttl.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3raruwpmb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3wkaksccq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3rpsquhmu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3jeexxivc.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3swiletkn.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3rvrkpkma.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3cqiypkgw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hkdupjke.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3vlmawbln.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xjfdlymy.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3lulbyday.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3pzfulrsu.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wouxbqgs.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3wnueoweb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3rtouyjra.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3nyxlxdpe.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3ohdhxgdo.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3stsbbiwc.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3axvmfktl.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3zprfqenx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3mpvjmrfn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3nzehyjsr.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vchkkvrt.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3bijhlmfa.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3whamiafi.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3qaobpdbg.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3xqbroqsh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3lwthqdua.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3xvxycyth.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3lnkaacpm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3mssgnsgm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3hgtcgrzm.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3dikidpwm.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3nnjpfobl.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3fzihkwsd.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3puiaxmrj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3fikekpkb.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3xhkwwjwo.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3tgoyptqn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3wgdvqiki.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3siuccqkw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3waprctbs.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3dfbphocl.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zssijniz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3kfigizba.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3pgggpygf.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3cnpjygex.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3cejelgsl.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ttifbgtu.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3deebbyon.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ebhlgnyl.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3qyjmdhme.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3fdiuxbwm.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3akdmdfhy.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ywjrwdgk.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3mhuxxqsc.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wxdmprtk.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3iapxeepr.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3byfsounm.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ktelsgxa.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3rrdtwkaj.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wdkngnpp.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hixithyw.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vaxhklnp.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3xqifjvww.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3wgffabdt.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3hbsncrkt.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3wcvzidhw.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3mmplziqk.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3gqgemnhg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3fdeorxuz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3lfzewmfe.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3ocrcyycd.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3ihhqupkp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3qojgymtu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3lofoiiyd.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ujfmafvn.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xftuubxc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3rmyhhleg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3nmibrdkt.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3jxhnpiqr.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3dkejyqyb.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3sssyfbmr.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3axyewcit.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zzmsufxg.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3zntijzis.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3fwqmicnh.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3zmgavuxm.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3hvpzaukf.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dnbtswlh.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3cemoryei.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3wyapakhg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oabipevj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3omeckdvn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ruhmmvxe.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fudthdhg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3rmikliyn.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hodqwqdu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3stpbhsvq.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lktebaar.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3xrtgvhga.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ivthlqcp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3wvupcwpg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3lffeumoz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3auneojyv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3jbnrrfez.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3lwzquasx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kllpefmx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3jheqvrcg.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3bhxequxu.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3qpynortz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3bssmkdvb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3jjruohwp.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3gmmmtssu.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3rcfpgwpl.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3ivsakewa.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3yjatlhlc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3bvplksgp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tmtxrhpd.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3ebxrrdkb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3burkkubh.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3njpeolkw.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3wasqwfrs.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3jhwvokrh.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3osacibbt.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3jkveeosr.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3hpydbnil.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3xgdwbaba.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3lfbywlcm.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3keddqicr.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3dukkfhli.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3baebodwj.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zbounxvq.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3prtzwjra.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3bdnaaagy.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3cyzvdukx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3dwaafwdm.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3pdgyjdvr.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3trpcplpu.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3noonlgcd.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3nhuxyvbb.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3vroaeumt.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3crqtfpps.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3itqszhsb.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3nhwynlsa.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3shrzplce.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3oyunrsgn.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3raizixhe.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3tpqgtkvm.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3lltnzpqw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lianznkl.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tbfbxclu.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3yvwuboya.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wdksadbf.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3qdzvxeba.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3rwnrnxeo.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3fsxdlozk.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3seuaocpz.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3obmmlzri.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3popvcvbn.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ydzdlzle.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3jtkbtqyx.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ssfaqcsp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3mcddgexr.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3wqqhacys.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tykxkyli.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3vvfrsehj.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3wssuagzt.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bthkztzx.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3drqmudcf.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wwdlzkcl.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qprndeqh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3nvdssuru.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3ssagcbyn.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3goyazwtk.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3zwazqpgz.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3hdwkasii.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3spbgyhvz.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3kcvlhzfb.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3jvdflmdl.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3pwyansgb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3yklsxsss.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3joxreiti.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3epjwuzxr.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3mmjmdgsj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3jbelwtjj.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3wnmjlozm.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3dkeymwom.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3vrkxieaf.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3zpircqgc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3temyvqpo.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3gzzobmly.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3mnbxrskk.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3eybnyiyy.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3gxacpuvu.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3ofgkilma.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3hrjupskn.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3cvxayqls.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3lzsubcyx.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3djnrnjzi.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3tejhxoyo.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3tolirvvv.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3gctmqnwa.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3agenovjd.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3umnxjebs.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3tjmeutpt.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3bddeplwt.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3zzolwaia.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3iufkhypv.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ebplhptx.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3dfohcmrp.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3uvzfepgb.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3ulejljfa.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3riwtochn.html


<!-- 参考信息 -->