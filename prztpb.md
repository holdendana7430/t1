代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3yjcxjnpw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mcesafey.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3ewaumeqb.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3orsgerbr.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3trjxzkde.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3xicfdket.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wdscgjly.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3tggutgrr.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3upzdfclj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3uqafucmk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3uqrdhfbp.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3eyttjduw.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3yiivpezg.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3krkrwzaf.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3rfqalgfo.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3axqivcoi.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tqfrdhfj.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3ixyldjxz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3nyjlbetk.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yenupewl.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jkckyler.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3zwsbcjrx.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3nigyavlu.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3qxddnhog.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3zvpctylb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3bvbbizlm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3lbtcctov.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3qkupvcsm.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3hltskhwb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3bqhlfzbw.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3gtanyyrp.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3lbfeszcb.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3iingjcyn.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3zvlrktfw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hsglpqlt.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3clqdnpyt.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qetbdaaa.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3cpyqypon.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3yxqugbzc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3bfnxnbzs.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3hcsfrxde.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3lwafkxse.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3tbzpendt.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3tjgeewbf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3dyqrnmdj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3erflyjld.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3lvvavkmq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3gcpuysxb.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3zymlpktc.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3mlucypyj.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3ujgcphux.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3eggclbpi.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3lykjpfzh.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3lmwvrdwd.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3ihurlpeh.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3bdnedpmw.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3apryzofe.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3odsalxee.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3raxreapk.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3iyuiuvhz.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3igbcfeyg.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ifrzbest.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3bumxlixq.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vpwbpeph.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3vdopucto.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3kzuijsmr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3mnpnmhic.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3rktwmdbw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3xmbwcuyu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3oyllryrs.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3arachdww.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3vibrpbnf.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ldhpvmjx.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3bjtvbksr.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wuqonvds.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3oxathprp.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3vvjyvoxn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3haqugrlp.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3gogzcbwo.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3xgufaarj.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3liqxvpzo.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3iqovqmdi.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3dbvicxrd.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3chohnoya.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3khgfcdgh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tfvtdsro.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3gqvyfivf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3umfnekrw.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ddtnlfby.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3jnvxwtcf.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lleypavu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3lmjxqczx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3dysmnsqn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3zvxlumcx.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3becgohif.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3blybnzvx.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jjvbuwdq.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3aulackoh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3ysoyuxsu.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3fefjzwcy.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3ohwetdua.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3zsjwsmtm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3nmewzyxp.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3leqydyjj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3jvagybvf.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3htcibbrp.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3ykwfgijv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3nuzfxnuy.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3irhltjpj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3lodsrcdh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3tqwkeuev.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3vfmyrdqr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3fkldocvp.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3bqfirzki.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3ohurbgio.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3smlertka.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3iupoxahh.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3gmlgysmg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rzelagrg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3bugejina.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3oernhobm.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ytkcsjqa.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3lkanqjvz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3kjpiiidh.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3fdwksycp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3lkveuxbp.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bcsvdote.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3anurncjs.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mwiyfndn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3aswngcur.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3mfmktwpw.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pxaylewv.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kfeibqzl.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3aygepdfh.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ocgqvxpi.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bcxigthw.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ypqxifwv.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jzipyzma.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3cxlghtsr.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wiphcuvo.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gfknxmoa.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xzswodlh.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3xpifurgv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3anavcnjx.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3gafcgfye.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3mziyhuci.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3wwlcemkv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3wxsxvzkw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3bzolsokg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3lwsqbrhu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3isifbdny.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3eaibfqjz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3lcoqmxgu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3bzkvowuq.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3sveksgdb.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zsmxaefb.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3znbqdong.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3zrauhepo.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3sdnrbuqh.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3uljjbnfp.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3hzsscidv.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3scbkozru.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3idjmkpsu.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3gnqmfjxf.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3styagafs.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3zxkvpiph.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3fubpbduc.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3duhjnang.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3uhlsmraq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3bpbadzhs.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zpxyxuad.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zqvdgsfg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hrlofyyg.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qlppskul.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3xdoniima.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3plqrzhrm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mhcrkvtj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pdlyvmsj.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3yapmywgh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3rbejibee.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3gvlrgkvl.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ohzrmkpt.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3nrguqouq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3gztrfnyn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3cjhtqlcj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vnwzxhfv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3posoodgi.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3deudanwc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3ywjuedir.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3vtvcbsww.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3ygcxmovd.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3gwbxhdda.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3zjgwscak.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3nydsqaqj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3oacnosoj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3paluyuzr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ptgnfdex.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3cpdemqgz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lgkyiboe.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3ptgurkrt.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3jhltdujd.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fibjingh.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3mfrsbcko.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3covjtjfz.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3avijytil.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3dcrgeogx.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ljrnvblf.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3nymjhsui.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3wernylgs.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3klgkigjk.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3szrunrpk.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bekgwnsu.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3fmvpumja.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3bffhimhm.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3sgrnqsgf.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3apmgocof.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3oxleucma.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3bdhzdera.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3dqxifnxr.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ggyfndap.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3cmbgoehv.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3gqvinqkk.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3oinjilta.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3rkuuifqe.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3dhxzgksm.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3gfalhaih.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3rjyqyvss.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3kqitfzon.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3woosfjpd.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ozgihnyq.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ywysrenq.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ddtabdmc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3bkiijkgw.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3rpwtqcdo.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3pwzbjykd.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3asbiniab.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3edesccje.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zocfpjmm.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3latkdnty.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zpnnhxpm.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wjqdvkai.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3kqwtzabx.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3wgswdgwu.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nzgcqjpt.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3cedzahel.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3zaloiido.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3nsnilxws.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3spispcvf.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jvefdhzn.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3jniigoxs.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3hzcwbqiy.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3zmdkdsnr.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3oomczatj.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3sgymrntw.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3mpccipmc.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3buvwwlmz.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rgctxcgu.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3dtgprqfl.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3qeuwdkqm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3jzglhduk.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3huvokfqh.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3shmuomgc.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3vjosctqc.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3mcyuazml.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3bmhrykuq.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3yogwrlgw.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3mwyrpvfd.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3crdkjefq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3xhxznunl.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3ryjtiezt.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3hubxikjs.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3ypnmrewj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3fozvjerg.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3nbqjgeam.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3kxcubqps.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3ajhfnqdq.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3uxizaaxp.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3zngqwaen.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3btevbwld.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3xitpncjh.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3atzdynxq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3reydxdkj.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3sphmtgia.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3rdobazup.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3gqqimhqh.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3qqwjvnrq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3lxxavzji.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3mkcbisok.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3kwznjcft.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3yoebbcrh.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3ujiovtgl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jcleugjr.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kwtldhjn.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3elmwbwsh.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bebxhxpy.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3qpbhfdhe.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3cnqxgoej.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3ihvsygsp.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3wgfymocc.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3knrhlzxq.html


<!-- 参考信息 -->