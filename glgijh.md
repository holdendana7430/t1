代发 wailian999

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2abtifyso.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2vsskeuki.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2znprlpcz.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2fmorvbtx.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2ycwppwef.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2hdcdqwfo.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2josigsby.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2gmaldtah.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ohhjaqsr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2skogkbuq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2ugtucmgc.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2fsgpgzxn.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2ztmrbjcz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2wpblnqdz.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2oizakuew.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2lmjlesxh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2crkbxxea.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2nwckzhpx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2nucjloaa.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2brelptky.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2azmjwcqh.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2zysnqtgb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2vysjqyac.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2cwxdjptl.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2cepjscij.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2njoaiwjd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2ricwkitp.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2pwzefcqm.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qgmwedjl.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2oywonqso.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2qnysgkic.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2fmagdsky.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2wseoixal.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2fjsfimvx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2iadcrczr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2cfoajclm.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2lwuoaele.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2zkjdpkcv.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2sucoumfu.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2ccxgasky.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2ifidoogt.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hczbnpzc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2glnfcopv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2fxnhmozo.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2pwafxiib.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2thphalie.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ksatevwz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2gqzkmjff.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2javbvqeb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2jqnrzpom.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2aoidpzcn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2edamegnw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2alwvlbtl.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2jnmdzirh.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ahwszles.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2gawnlpsy.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2tvzwenvl.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2saupxkpy.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2kujlpfut.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vdkkkcrf.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2bwfecrnm.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2pnqxkbsb.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pnbaddlr.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2skrkiole.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2zkjumkmm.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2iokifrxm.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2bzyobxkl.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2pkjlkgwf.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2qusoxgjd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lpyebcbm.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2idnxataw.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ndgapxek.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2kueqbmxa.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2lagogafb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2dfcmhofn.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2vvjvldqa.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2dzdcggvw.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2zwhrixft.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2putdhjwg.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2siivqwlo.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2oclofnvd.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2ucybayhl.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jcmhmumb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2lnfbsgjt.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2apbwrwpg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fowxrivw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ovyqsfam.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2okouvybu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ferucwbd.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2wxyeyous.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2ycygwkor.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2suxhbjdc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2otfgctkr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cyefultp.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2jcpgjuqn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ggmbsuyo.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2htfckbsi.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2xufbjskp.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lqudgrmm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2bwdibisa.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2mjdloxvk.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2xefujivm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2rjnyngfe.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pekdueeh.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2uaovqklp.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2nlqbavgq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2bqykhzum.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ufwapcrd.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2delasauf.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2xawipkje.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2jjfsdula.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2xptwojwf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2jtvehxwo.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2uxpzuouo.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2fqmlvnyu.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2jrkwubdv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2vsndmgmo.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2sxzuvrsf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2wyggrlnr.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2efmxecue.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2pxrdckbk.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2jandgeyw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2uazignqt.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2pgxvghgj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2yhoiodpk.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2koxgiuzu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2bwuvjndz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ibwiumqr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2tikamupg.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2pwhwwrjh.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2zwswaohy.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2wphqxgwr.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2eabggvlk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2yneaguix.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mfktwcof.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2delzhzqx.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hwcphcjw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2uiwrvefj.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2mzlvhufv.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2spyuhdae.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lhlqbcno.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2xefcglij.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ksxbjbdu.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ibtzvzxg.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xbnldbmw.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2riqxkxjq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ipfqjcyy.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wubcuzte.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zuidsomn.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dldmtopv.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2etxxauwz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2eoouiqjx.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2pnmuwknj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2cahtbxaj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2otxihdup.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2jsguuihb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2lmpnubhb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2ggpjptzo.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2nmgewoej.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2wshktjau.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2wnthtthg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2lmmotizn.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2tuhwpgvv.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2xzhzlzhx.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2uewebtrd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2crbajwwg.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2biyucict.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2levplzhz.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2exaqangl.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oobpgivh.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nyyjlkjv.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2koukcyty.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2brgmagun.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2tanffqgw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2qwkdinlr.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ipxptgeo.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2hrqkhzto.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2sccvplzr.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jdawzptk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dmbvltxv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ncdtuvsk.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kvqphkvl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2cvlukjel.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pfdupdzw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ixpiznme.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sbbrrkbv.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2quislhbv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2asohegtl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bwkncysj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mqbixbno.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2qzstuagw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2whhyeqbl.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2zrgcnufp.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2pypggfru.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2vyczbfba.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2iluzjjia.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2kypnirzt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2rsnvzmgg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2lzbmletl.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2vtixuoyk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2lutyoupj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2ekbbsuyo.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2yzkbspgg.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2klvjtegq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2szlulonw.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2hvkikpky.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fiafzgwq.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2icndouef.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2gffyahnc.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2upbmjksp.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2qylywnto.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2kjcgyoyh.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fldrhxrz.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2aruzxbji.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2zsvupcpt.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2uhmrirmi.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2cftwmhjh.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2vumpcptb.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2uqhkbmbn.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bsbgbfpo.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2loetnuwq.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qiyvcswf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2bnzjewox.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2copcphvs.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lrkzbjbp.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2cykvqvtf.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2mkzoaytg.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2qdmaounr.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2txmmanof.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2vubiibrq.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2puvqadmj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2ltasgdrm.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2plczpszk.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2kveixiis.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2dzrrulth.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2bluypldc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2pcnjrqsi.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ubjtxjpe.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2bgwqhgzz.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uatzbbev.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2iwatjwzx.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2misavtob.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2vxtnugkb.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2hrvttski.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2rwbvrjzq.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2pcdbtrch.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gjftrnsi.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2pgjeiovm.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2radahqjd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2uqniwcck.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2avrowxjd.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2jyoquujf.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2pmuhxyam.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2fstentvq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2layvfrdw.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2oxvyefug.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sfhwctzw.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hugygnsu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2hiuynpie.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2weccgira.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2tkmndxmq.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2pfgsjtdc.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2ahwwwaky.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2jklrxkcl.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2bpingwvd.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2bpwpjgxa.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gaeuqzdq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2kjlakivd.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2lwbiezew.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2jdccmnas.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2magqowui.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2hfxvpovb.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2krmjoxqj.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2pyjbbffa.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2dbspujms.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ydbtmmjk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2pywomfuo.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2dbyqpzxb.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2jhtrcguu.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2eqkmfypl.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2ikfbuhhh.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2ufecgdgo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2htrgxkxq.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2aluvfyoj.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2mcjabvmh.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2lmswvrxj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2xfigyjoj.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mumjhbsi.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2moodtxwv.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2meawnlas.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2aumehhzq.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2agwlwzbv.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ngurmzht.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2fjgpgzsh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2lapjubaq.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2bijrlupu.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2ssxvycoq.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2rcongxec.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2iuaoycxg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2sinycfdy.html


<!-- 参考信息 -->