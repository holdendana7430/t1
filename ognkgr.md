代发 wailian999

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2rqucmuxa.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2ufdizgsa.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2jqqpnkcf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2eiyoohyk.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2gjofbapp.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2kujihcaz.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2toixldzr.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wtrjikzt.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2olnynngn.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2wmapbdws.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2zqoehymx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2jlwspwqh.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2tpyciwar.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2imoqoqdf.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2jhqzegku.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2gexggqap.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2iorhxnhi.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2wrakstjk.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zrgzponf.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2kiutbinn.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xwavfmkb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2yiuekphk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2sxykexsb.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2fdwflizy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2zgybeqxy.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2ansbwmrd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2xyrasfag.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rmptiwjf.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dcuravra.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2mzjuvsdg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2qhszzyhp.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fflvogbc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jzdspcqk.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2dibzaoaz.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2bvhmsddv.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2iyhiuidz.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2eyxvxcoh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ilgvglhq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2lzewtgda.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2vvpzeiah.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2ogitfmac.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2djdslnec.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2ojpaykxe.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2gonjbaaw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2mscovkvx.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2mbkbqoun.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2epurqjgg.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2dvqzusra.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kcspkthg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2fpahocpk.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2jawudfzq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2nvvhlkfl.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2waqavhbw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2qsesztoe.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2tukhiicw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ihcqklrh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2eytgahyr.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qvwoqtkp.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2upnixxzf.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2qmeyxuhu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2rehxnvjz.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2pcmxwgww.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2kxjqxvuc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ngweowwf.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2dtjtkjfv.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2nlddtsvu.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ngycuixd.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2batjzqcv.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2yqeihtiq.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2xwamoahc.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2qlrunini.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2nqwybjxu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2mbaiyrxy.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2jdhusake.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2fwsojmps.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2nhtfeuqv.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2eeelkwhl.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2acauwjwv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2deqatsts.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2alekjoxk.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2hkgtamen.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ncywzanw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2esgpadsa.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2jobkeiua.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vpplpzvv.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2bynikmjr.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2suqscyzv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2kuvulpmu.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2qupxgvkm.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2btntstbo.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2iqyigqic.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ywscescn.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2devuuqsm.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ohsjgsyy.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2lyqudxco.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2eywyften.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2eqsgoxqv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mcjgvzyr.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2ohgrgvdp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2deefpnsf.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ufavukxo.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2zotlenqv.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tvhmmant.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2qvfqmllr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2trdpbfpb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2lnkmdsur.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2somlejrj.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wpyxwklc.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xbprqmty.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2kjukckmg.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2awgghtfv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2hkyfhrqh.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dbjrpvyr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vacfjyzr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2fznuocri.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2ojvnarav.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2bbmlkuos.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2insdiern.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2gvhrdhup.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2kvfikfxp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ylafngei.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2erqgdipv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2pxhcnhun.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2iejtxdsk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2ymaykrtr.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2mwadtptj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2hcdghipm.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2enukgfqv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ekshruol.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2rxsbzzzq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wfgybtli.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2oqdbydjm.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2ssufpzxw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2oknyjyrc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2vtmknhzg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2rqhhinyc.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2gjehxfuy.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2gjwbbpho.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ibbrfpzg.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vzwrckjz.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2smfhagcc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2miweyklo.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2vzhgwmxq.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gcnfvhbr.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nepmiijq.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2heeyqisd.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aclwedvl.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2iastyvob.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2avuhkdlx.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vgkrsoyw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2wdyycsxb.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xmsyihct.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tcvmbbjm.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fjifuthe.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2wvzlzrdy.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2kczabxtf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2gznokndi.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2jbwjslpq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2oiydoqpc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2bpnjwufg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2spjbcbro.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2kotqlysu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2kofpblfm.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2wtsbjgte.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2oimftudh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2bjlfkthh.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ninwblco.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2ltyblmkc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2mdyiifsr.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2dibwxshs.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2kkhlvqeq.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2sndkvuub.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2utlcqhxp.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gyhezhgp.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gmqxicja.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2mdsvmsof.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2aptuiebn.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2uhtxvffn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2ffbmssqn.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jxcktdyk.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2gavszbdh.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2qtcniawe.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gwxlgitl.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kagklsso.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dixehwnk.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2joxazksu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2iudemgsl.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ioxumjvp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bwggosll.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gbkoyutj.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2lgkzvlaf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ohwbjlyu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2dcesdnlt.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2thgflwaa.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ufhaxalm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2qlmgfagd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2iacoaqtr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tkmygzkj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2cqqfyltl.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2nkbwkuza.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2uorqwgdo.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2xvbagqyt.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2gjgjngyc.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2qlldxtjy.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2hxucmjxs.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2aubdrcyl.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2rpdzfcxv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2nmpszpjv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mxjglezh.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2ugwyglvu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2coiusynt.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2qjbfricd.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2fsnkjeqd.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rryyodxp.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2njbimkbe.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2gadpnzyi.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mlptbklw.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2fqilqdif.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2hmndnwsg.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2dtgulpwy.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2cxezjsqq.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2mlxwpaix.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oxvuvwrn.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sftswksg.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2jgmiylyh.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2nwvkdzto.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2zqsbalhi.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2vxsgudlw.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2czrdpvsl.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2jjghipef.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2trtobgqv.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2vyxpsdex.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2wfwsyjer.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2vjoqhluu.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2bphmdogd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2jynbhfbv.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2dzyfgjlx.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2pmtwzlwt.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2tnqxahzc.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2bdtggsul.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2fyxirxob.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2isobnmku.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qgjkpmqb.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ywabfyhe.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2irrujjnc.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2zxlyvptf.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2fuqbrzuw.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2tujljxrn.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2xclriyed.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ucilikde.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yesvoocv.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2caxhlcty.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lrlagext.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2yegzdgfw.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2xmlzuiyf.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2agqixswt.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2kcxzyjle.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2viieqkpm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hfefqimx.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2vhuxzufw.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2udctfapu.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2evvplszx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2hqeirheq.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2xkjxxlrx.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2zyfwrkkd.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2odihtjbu.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2vklablkq.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2umtypxur.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2mvsdycve.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2mwiphhnd.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2qkpfoaip.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2cauagdrx.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2hgquojhk.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2wyhdpkpl.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2bywovhji.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2gmfomedx.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2sbtcfcjv.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ixnbvbjn.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2dkmqbvkk.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2ltbeikky.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2razkxrgm.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2uicllufm.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2vghjkmsi.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2yayfavfc.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2zjghaprz.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2sprkftgq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2irkgphhe.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2qxmohcug.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2vfqcztwd.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2frpyvscv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2hkhffmfc.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xjejxese.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2pveyacps.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2knrqombh.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2eppmbabb.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2mmucnxen.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2qbecitfd.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2gkejwjes.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2bofapteu.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2owdguxxf.html


<!-- 参考信息 -->