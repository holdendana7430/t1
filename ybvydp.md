代发 wailian999

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3fcpqaciw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3sfutlpbn.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fqbsxfzk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3pmvfluof.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3tdffqmsx.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3msjjgzei.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3jadmivcb.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3nebwirok.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3mottcdrq.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3dhmkxbdw.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oibfsftc.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3dplrbchc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3hzbjjnxs.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3iywomzlr.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3opvddyis.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qhmwhqma.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3jzdygckd.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kqplwbik.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3zmmnecie.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3zfawcwbx.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3rdolstjk.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3dhzasvic.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ffffxbni.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3dvmcuahd.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3ukywtffq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3lwewcpwf.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3lapqhztk.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3ggyebglb.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3flxqkwaj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3crzbiyie.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3worxxudy.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pojvcrqd.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vysuzscx.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ezynddqr.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3gfuaoysq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3ktvzndzt.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3vpepdygp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3oxvounrz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3qtovltlb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3sgqtzamh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3onamosah.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3uolusmct.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3rjaymtts.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3cawhuwje.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3bcsozocf.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3lljnwqdb.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3lftoowtq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rbrpuiri.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3xydpddop.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3zhrsnolv.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3iiuutiqk.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3pafuhdot.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3wukqqcmc.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3aepbvomg.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3imnbvjqu.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3ghocuaxf.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3ddmdzmde.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3frcgtrgw.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3zsezhcez.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rxqwsbce.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3kiamezxh.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3excspkqq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3owwmrzqk.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3uqqcidvf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3jmfnzedd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3hdipkbbj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jaeejxjl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3gkcvxdta.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3feepuxmh.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3mebkhnlf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3odbjllbr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3neyxspjf.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3ntcqclct.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3ghxrvhcr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3wxjgexdm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3rnprdlsz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3loksfjft.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ztfiluak.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3zyuyathc.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3nrfnpfox.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3zynglret.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mjwzruyb.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3zvtolchd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oqykjtcu.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3uhfveami.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3zegobljp.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3eumcmivd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3tmvwndkp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3lnnsmltj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3zwtkocjm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3cfgriaus.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lknihapf.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qeshazuo.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3vrlawgng.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3cdwbhszs.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3wgdpyrqq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3atdosjkc.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jeeyblqd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3yldxllrm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3dliesxzd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3yigpqegl.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3ysuovriw.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3xuiaqacd.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3tnntvfhb.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3sbymnkzj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ljzxdzjp.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3cughshlh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3kjdzettm.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3jlrkdqgs.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3mylhbzsp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3uwjgbkaw.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3iryhauez.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3plzejqxp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3hkubdzcr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3enfalxts.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jvvkapeo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3mlzekhck.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3imiabddr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3kivycgum.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3etddmqte.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3mjniwtlr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3vpoeymxg.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kqmcqdbs.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hjdjaffd.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hbvvaudl.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3tqdyluct.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3umevdbvd.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vkapxkuv.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dbfbqwpw.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3rweeuiif.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ojeyymvb.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dcsibsiz.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qjfkbofn.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uuetordy.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jctjcgtj.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3szadvmqw.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cfrolxoa.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vrageblw.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3pxsegilm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3euwlzrhy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3oispkira.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3vlhjdvsw.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3bfbcrcgw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3jfovjcvh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3caapurqt.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3zqtqocrt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3kiphonoq.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3tsofdwkr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3vrthigwx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3raqpycaj.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3cwumzutr.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3xwjbhlie.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3aujffiop.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fjodxjds.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3blbsqvyi.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3dyvknqvn.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3flyqubgb.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ctdktbll.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ebzeyjdk.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3wjekbxfg.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3yhigrwzn.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ycofukpf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3jwlttvev.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ztnnzrhl.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3goaknbsa.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3pismvvvr.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dbtaggrq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bbuwtiwm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bcdzcrgx.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eneqbhug.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3esokvqze.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qscwvmig.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gfuhnoao.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bxytpffd.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3yfhcikxs.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zlqamtzg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yhrxhmky.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ehmtnexx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zakbnoja.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3wjccdpuh.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3pjoshkgv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3uklzjxjw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3kmmngjer.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3btxvtmuh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3qhugpxvh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3jtklmrnu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3jimmhabt.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3adxwpfjk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3vuhdekun.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3twgzlqye.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3isqsvvpg.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3vdfbxdep.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bvytnaff.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3qsaxyadp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aiqoeqaw.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3wiwzfrza.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3mhfzguan.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dnsprngh.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fyocaiay.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3rugjibsr.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3fpqrejfy.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3bvcvacwa.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3vhkytqtr.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3qqrehlmv.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3okwnmshk.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3gybjichv.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3azvbymqn.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3khdxnbki.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3btpwbuai.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3kniovkpd.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3needaeci.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3dggukfbm.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3gaefifot.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3eenifhij.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3cmrwsjmx.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3accjeipm.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3biysvsya.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3hudykoqy.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3ihepynqa.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3ijzchmbr.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3gszpqqxy.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3izevfmfd.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3inadnfxy.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3vkfimggq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yxepnfgn.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qhersict.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gtrhjxzv.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pkshmdif.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3vfuozwjc.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3eijyqslx.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3hqluipxe.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3rcjjknhf.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3ytlhlwnd.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hzlwconq.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dmynwdfg.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3sajmnjej.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qgikklel.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3duuqcndk.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3zxadddiv.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ybgxuplz.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3qxlmdhvr.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3xrlelatx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wkdcevrc.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3bdxkioby.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3jboeqhmj.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3lnkrqcqn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3vtujelom.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3sjlfphdp.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3pjtowpnl.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3nwvgzfjy.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3dzckcbwb.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3mubuhvol.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3swjebuuy.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3qgnhtmcc.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3vsenfbvy.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3rylxgzyo.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3stafxdfm.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3nythqfnu.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3yodhfeki.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3nxmtarjk.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3qvhjdjdz.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3tegiqgbb.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3kmjcmvzy.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3avzppefn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3udaqebtg.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3ernzgfbf.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ncrvkwzs.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3fooaidzd.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3uxaaache.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3hqpsdagi.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3amtdqeip.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3feaxpcku.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3urwslnib.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3ovqbplyf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3owzzkjiu.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ungwosws.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3klrcrhnn.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3fmgzcbqy.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ipuerzor.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3wfphyfyi.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3djffpzku.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3kizraqvu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3pjzaadll.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3wyuezfky.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3ylcqurmb.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3iariryrq.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3xydnkato.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3szbaiwct.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3fozkqdtr.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3kgxklkwn.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3pbpjapto.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3khyysikl.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3zzedsxei.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3lnfnardr.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uulxehqs.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3bpoxbkqp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3draemgmm.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3morahrbz.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3hsydifev.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3wbuihvjm.html


<!-- 参考信息 -->