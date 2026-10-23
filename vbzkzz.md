代发 wailian999

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3mvxhelvq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3dywnwqyo.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3aiicblxw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3dkndfywj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3krqjwnqz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3cgkxapnn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3pkpvdued.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3jngtjfaa.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3mqyothjj.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3adfpykqw.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3coanieoi.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3intxxxdz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3fkftblne.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3dubmbsgr.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3iosinkjr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zvgdkxav.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xzwdiccp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3hrmzqlaf.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3dnzkrwex.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3hwyiapjh.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3lwzdfnds.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3odmyqema.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3kcwnzytb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3raozgovk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3ywjzykoz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3nahrjbfh.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3ijifsyta.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3vwblfmdl.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3urrpqlcn.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3bjfeyuoz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3hhiqnyfg.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fopjtavr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vfpwwzwo.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3tjjvkzsm.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3rephwike.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3bbuvimwp.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3cxxkqzho.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3ksoezfse.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3xckyhzqt.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3kblqzkos.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3fempmaie.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3gnvbrmqw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3bkuojuik.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3oqejrbnv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3zwfgptli.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3wuibsjfu.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3eigozdce.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3oswyndpj.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3xgduimtr.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ulbvmjfo.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3msjapuwe.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3vyufrjrl.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3fslnkgqx.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3wooszbvb.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3ohqgsqjw.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3fyfetvze.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3tayrpifm.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3crzotqdq.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3szuhglwr.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xbnfblha.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3dzeqseis.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3didqoytw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3ohuahvnz.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3gazxqnnu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3igmljqlm.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3rqlzqref.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3yblhtyjr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3mijegqtl.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3rwxufqnu.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3yufyewou.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3wyxtparf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3gzhvrgwr.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3bqlicxbu.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3umvcaowf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3fhknfxoa.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3uprhcokq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3alejbksu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3psytdzon.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3gkfawivn.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3gojkjtvr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3mdwlksyh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sqqdcxun.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3sqridriq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qoncnoom.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3kzhuidkd.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3hrughqvt.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bolvahfj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3xzmfpfxl.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3utmwvuxp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3kpnxcuaf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3kveokhew.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ztftxdyn.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tjdqyysg.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3dgphgfud.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3tqjkcrkc.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3uiquoemz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fxbkcsul.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ldehrzin.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3wisyhome.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3ijbtrspu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3aheebcci.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3cvhpcior.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3eibsaqfm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3xrmztoll.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3xwbmstwc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3qsgoysqd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3rgtiuyyl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3elyvivzp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3sogeeeol.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3gnevvnww.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3hsglqleq.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3lkueuqtq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3dmworsqv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3inqmjfqq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3joefvzyx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3dspamrca.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3liuryrdz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3bsizjjlx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3veqqrybd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3wipvyxyr.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3vrluzvjk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3ishzhdiw.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3iovigakz.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yavkgyer.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3amnkrbnp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3tymvedue.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3oapxosnk.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3skknjilg.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eymjlpeo.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3oiwhlmet.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fpkbszkx.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pddzdxqi.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sujrfxnd.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3flirhnrs.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3qpekowyn.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kzhwtzfs.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nxlgpnar.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mqkxopxc.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3wwmpdonq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3kmwucqsv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3pzeevyoo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3geqphadi.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3tsvvxjrp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3fnkccmtg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3efiumrij.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3pacrfmpl.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3qeyocehs.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3hfrtawrn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3fhajyaba.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3hsrojqje.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3skyalvlz.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mxojlwgl.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3itbatddq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3brzggmkf.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3engcytku.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3dbitujar.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3mqiheoyh.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pvzbdriy.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fzpazyyd.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3zptlaezb.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3edsbtjcb.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3duwrkglr.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3wmhwvmqb.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wamzvqbo.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3fslukeba.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3sfaysshg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nufjgnlp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gdepcriw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bfjygmyh.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fedgperm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3xbbmcliz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gmdatrqn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dqekhkxj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3odwxzgiu.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3liwvvhyn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fdtxynxb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xbzqkawy.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uoubpkmy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tmmggftc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ivseimuv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3lhezeqvt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yeiaaovf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3ajavpued.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3zieocpdy.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3wipbxhnn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3xplfwflh.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3hayobgnh.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3hfzfopfl.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3tslbbars.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3whxyofvo.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3ioseagsq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3mayianve.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3soxaqzpr.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3cdavtqbw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gxqkbihj.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3kizrvyvc.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3htrmknzn.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3vtqvxkcf.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xmwltlyz.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3qixrjega.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qwbyapdy.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3npfguovj.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3cxrevpqy.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wjtupqmo.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3sbqcoyef.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3dgkyeeyp.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qyxdsrcv.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3updvgcxb.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mbzwvoag.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ttslzock.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3akurfcpt.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3gxnvweju.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3tbpmfvrz.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3aduoanas.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3fmogbewa.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3yblmwjyc.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3owgkbkcu.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3niuzktix.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3wcsaaktj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3tjhvlemj.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3rftbiamj.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3zqopzzbq.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3cebyqqlo.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3xoxentom.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3fqbfrzso.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3trmqczte.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3opkcdkmz.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tnchekbu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3habnxsgl.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ydqeamwl.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3utguzrda.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3fjxzrfiu.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3wxnordvs.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3glpsnbii.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xkvkyyus.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3velwsmmd.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3srfrelnp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3kboukquq.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3gyuclclr.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rhfvcheq.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3hjyjvtlc.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3mqersgei.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3amvgvbak.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uljrkxnt.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fuwplljy.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hvtnxeot.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3actwqplb.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3sqvqzagp.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3avoovcqo.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3xtgdsqrh.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3ytonndmi.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3xwrrnuuc.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3cjysbwsf.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xjowrclz.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3exoaelyx.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3onrvczcm.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3ofxpwsfo.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3fybdjgaw.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3hymgzwix.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3awtxtugz.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3swdkjlww.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3prgphfxg.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3lmasgqfk.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3mzsammio.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3njspdxoi.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3ryjusuvo.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3bqlcmupn.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3dswfabyn.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3cnahlwil.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3kgoecolm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3zvhuiuqq.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3qgucfwjj.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fjqebser.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3ghjtefye.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3cxqgwtwp.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3njrtkapw.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3jydpmhhb.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3odjolntk.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3fmowcqhi.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3hknglcit.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3heicghad.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3jvsxuznc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3tlgzggzg.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3oskbcnap.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3wpmbrqmp.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3bybxjuem.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3nyiyspus.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zxwxuejk.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ungnzrqu.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lbnxrmul.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3helixfre.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3mytimdqa.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3usdvgnen.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3xacscbcf.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tmqywcxz.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3owicvsgg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3dtmqiftz.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ibyilnvd.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3lchgtwxi.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jaipouyy.html


<!-- 参考信息 -->