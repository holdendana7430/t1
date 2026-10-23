代发 wailian999

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3uatplfvh.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3mmclwgup.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3yicnlfqa.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3rbozgdbs.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3hdrqxqbh.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3rhtjeayh.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3pjtaiqjn.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hxxvhmrd.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3duqrhfje.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3kbxigfbq.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3bnwyskux.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3eoozrgyk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ogmywppk.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3uwuhcfub.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3bdmljlac.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3vcathwke.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3jumpyhtt.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3jdxifecb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3shguivyq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3sbhoqdgi.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3djkphtdl.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ghomhizl.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3jdqfydkw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3clfgvcow.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3lsdiasal.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3sluhnjju.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3incwerkq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3zojnkdrh.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3mfqwbyan.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3kglugtff.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3zvehqaqa.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3hlurvnzw.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3zrrbuqmc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3udduzgsq.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3wofxmdmm.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3stqcxutv.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3nxecniag.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3dnktjzay.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3wasezowm.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3qntpgcgb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3qvljjewa.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3jehbktqt.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3jmneboll.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3iadqqlkd.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3jwrtuvqy.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3krbdfuou.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3yhgiofiy.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jowutucr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ewvabmts.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3mulosewn.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3dcowdivu.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3porkhmng.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3wcpiatqa.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3lsnrippc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3ymexfiyd.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3gnufdout.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3dzhmdait.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3plkgedbc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3plzbvahi.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3zykexrhp.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3htwkqghs.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3wwjbikpu.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3mmurhnzu.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xttuiqtf.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ldzfosvk.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3phzodtcm.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3udocpbsu.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3robwlymw.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3jpiltrkg.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3jlwtooxd.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3ramduvfw.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3jhbqauiq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3omwqeszl.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ypxcsaae.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3czcxihkq.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3zpbkoqjm.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3mouyorqk.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3xfyuophr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rfjvuxzm.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3kqqpkegs.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3nrcctfbp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3eljyeqcv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3zkinllpc.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3cracnwty.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3cbuftjsw.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3ipvgivgf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3fhjexztv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3doltbxnr.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3munfpuac.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wnxhkqfa.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3vkeaogqu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ulnpknmq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3erjuibhm.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3qyxgitps.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3owuuhtjg.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3rffatxif.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3jobfrmcp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aqdlihcf.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3roxhlxlx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3icrbnpwl.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3rpxqjidq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3qqzyaiev.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3umfffxdo.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3ccmgsujz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3eekywnqs.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ismlmnmp.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3nrnjiouu.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oeqirhry.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3myjvrxxj.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3ajyetumi.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3tqdmsxcd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3tibiueil.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3uphxwddt.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3khcaygxv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3denquvlt.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3zwobyzrb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3amabwavc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3dqvbfste.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3zbtfbvto.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3zknehqea.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3ygpsacdl.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3swnigbnk.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3kfuuozkp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3dvewtpul.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3bjjbcvwy.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3tdasbixc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3ftinelsk.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3ordzriwc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ergirvai.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3ztcfnihk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3eakcsios.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3lqptnuwn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3gzkydpqb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ldvdncut.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3owcmmpym.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3ctoxzizx.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3bgctimoy.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3ebqbizxf.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fnszznxv.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xylwgbad.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lbaddmgx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3egxpisrq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3okapbtsg.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ngrupjjm.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3paeuxzfk.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3mjqviisk.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3etmtazuu.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3eqkkghti.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yjgqxwmy.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3beafwkve.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3dilxkfor.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eijiypox.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hkxmszsg.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cocwgnvw.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3gyzndrwy.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3mgkejjrt.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3nmyvstag.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3fhyrkihr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3gccjotre.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3iarxszmr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3rbkfuvwa.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3ztdcybym.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3plwjgdqz.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3rkpobfvm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3rmirdjll.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3dtmaclrv.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3xnlywcuu.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3szgqrtgf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3gxjkhzmm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3opojhion.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3jchsvxek.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3gxketzvy.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3ppnqrizd.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3duummsvf.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3srmlqgrd.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3bnkkptvw.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3xurhbosv.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3hinigzju.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3xkhoiyhs.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ddmxrgeg.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3kanphqif.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3npwcayss.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jocugebe.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mpjdrtwt.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3szmrlbnf.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3itltpvct.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3jtttxeqd.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yxgiegmy.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hcvmnkcb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pohseuxh.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3xaeeynjm.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3siaiirck.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3wpeyrrui.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zpihcosk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ffqqpbwu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3fuqfsdqs.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3hnsvybwf.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rwrtqrcz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3meurcwrq.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3dwhrturx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3iacabygp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3vfbowgsa.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3zflcibfj.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3qfilzefn.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3hnvprovp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3rmpfsioe.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3uhwticdx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3sfekoqra.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nhqoxgrh.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3rbpeyifn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zesjexdm.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3duxvncgb.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3lpogvlar.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3vfgyfrzk.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3zoecelus.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3kfzrskcb.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3aesdcmht.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3ckoigspe.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3bujplwlu.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qcofyyvb.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3pgricrwo.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3wsfwfhoo.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3smjxsdlk.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3xukqjlcw.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qalskhfj.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ojlxdnbk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3mmiuawfg.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3hcrosmkf.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zptzrrom.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3knkjjphb.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3vdcmlxdf.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3snucfesd.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3yhwweerd.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3gsodrbvn.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3xdxerfcc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3mmiwfbbn.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3zmxdjhcn.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3cueuaege.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3idyvkvuq.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3oalsslww.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3xpyaeivd.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3oepfusuj.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dskpmtwn.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tyhyihab.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3hrburdcx.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3dblloofr.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3vaqcomoy.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3nxfzqzhj.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3wdhigyjx.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3aldhveut.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3oqrxlzvo.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ccyhzwzd.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3gymaombg.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3itqwwbma.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3jgqgpxkc.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uvzntbgn.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3hortxihs.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3lymmjnhz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3grmarxcx.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oqwytahq.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3xpcxradh.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3knudpdfv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3bdrrjmbd.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3heitjivp.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3iehegcpw.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3uinsfxbz.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3qepnjnrs.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3lzztwzpu.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3zwrrxzpz.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3zyajdsod.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3igjhuohe.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3bjepsqpe.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3ammrslxu.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3uhjdywfb.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3avawmrrh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3hfikyhyg.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3gzvtrtry.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3msbsrdbd.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3vdgabfpl.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ekzlvhsm.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3wodvucib.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3kuprnctf.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3gdeonauf.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3gpriksyw.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3jsuhawdc.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3mbkoszsd.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3sjfoijaj.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3qkxvlywa.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3ihzhrkdp.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3cctdlipp.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3uaibmcde.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3glsyfenf.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3pttvgsfa.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3hthwuaeg.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3rluwkwks.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3zvkbilka.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3atmhhzgn.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3ioamjljo.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3deinorka.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3uxhayoms.html


<!-- 参考信息 -->