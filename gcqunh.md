代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cnwtdbpc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2gqbjzesj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2iwnkhpqh.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2iabbnqkg.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2gndrzgpn.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2pqdkvnfa.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2rqkekeid.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dfvrqjpa.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2iavomosc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2gvpezxhm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2qgomslci.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ehsikvnk.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2qujycgyf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2hrkdjwdx.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2lcrwhpbj.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2yblpsiot.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2eufjohhn.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2szfhegzh.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2fmujhqym.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2qvaltyvo.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2yowrmqgo.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2bbncjlbz.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2sxjunwpf.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2igfqtfnz.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2kgmmtlmj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2yjklyvtu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tbmecjzj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ptxklyjp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2xbvuxrpi.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2xfuwicat.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2odvfnufb.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2ayfvoraa.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2wgwupljq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2oarncclo.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2uobsqorb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2viirrjsp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2gzfwuwqs.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2wwjryzep.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2lgickqqc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2uazizwzr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2rhacmkia.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2tavtzfys.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2lgvoegzp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2akkqavqk.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2mzyjdgdt.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2znnyogyo.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nconoqws.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2jmqtnzwa.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2qedpsntx.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2dehkcqbq.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2fdyygkbv.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2ygbvnrgj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2umliwagm.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2xezahbfz.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2ifdutzho.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2hozlutbf.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2xehfisnf.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2qglcprrh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qnvletlq.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2jvufzycx.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2ybuvqkut.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ilhctido.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2qfyuvtnu.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dvrnakdl.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2kccubats.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2vdcstigd.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2bopppmay.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2docyygde.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2qihjinwe.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2viuzkkwk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2mxsqokuc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2akupuobb.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2spuvbvfi.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2sedoecrp.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2hqrpzeen.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2mimuikgk.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2khfosuih.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ewhyrekw.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2iflrzysx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2drswvmdi.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2mtjytgxl.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2pggrwvde.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gpdoyicc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2qyxdrxhj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2csrhiddc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2qwfzbrbs.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2jzxugypd.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zkkuknue.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mbmpszmu.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2tdmpfcoa.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2vxivjsxa.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2qqxjcnyn.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2volbihuy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2pkgkupar.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ldoxokkc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2olnjzkuv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2hbrjcdyv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2okdlsqtp.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2sojzjrif.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2twselcrr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2xotfjwfr.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2eygzlgfz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2suracvrp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2piuqagcn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2mspsouup.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2xwcomzwu.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2yhcxkusd.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2lgjcxusy.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2qnkjupve.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2adcujotn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2igufnkoc.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2engrbwre.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2cuyketua.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2oqxbydwz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2jzepdbmg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2pahenokl.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2qtmhzzic.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2birabdps.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2psplybkv.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mtmopwer.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tslkmsuj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2vubfdjil.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2fachetsu.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tbgxavkr.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fkdyiygl.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2nawelrln.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hcuptctk.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tyonpkqw.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zouylniw.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pufghnek.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2nnagqstt.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eqosmont.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2miijfbzx.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tgdakwfz.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2akdhpzmn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2wmpkpppg.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2nsfrsppf.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2zdeebudi.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2oimsrxyj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2qmwdewyj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2ygsewkzl.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2rgvatzbu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2upjnnmle.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2suzemdid.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2qwoykqmx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2iiyikbbf.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2buembafa.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2nxrarjmh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2zhfychgy.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2csxzzlid.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2symuuflw.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ieliprtl.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2eobavrdd.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ntthuprk.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nftwjjht.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2rxfoqiqh.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2wtumrlxp.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2hqxwpzzb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2ialxmbqj.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2spnujpta.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2jruvoysv.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2bqbzxtmp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qnggjcsu.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2venpagdy.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nfuqumwm.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hzayjeyc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2ovgwbhhg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ptrzuymc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zfrgbztu.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yhfcillj.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2dwqklwcs.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2fsiewehr.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cgkvuaoc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jpodpxrx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ijcputzl.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2hlrurlia.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2mbxfrsqo.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2urijfhpq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2glkrinzx.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2vidyvqyl.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2zqwtwjjs.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2vxrswakv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2srdxrwhd.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2zcychato.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2wshpnlqb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2uhklktqr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2jgjbdhac.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2fvdfjfvq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gidhuudq.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2felvgsji.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ozvqgafu.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2qjgfpgwo.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2fgnskfuo.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2affiqnvu.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wssxynmm.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2nnjvswxt.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rworezms.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2iavvxeox.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2obatxffb.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fivxmskj.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2wvfurabp.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2uxdrpxqs.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2mjczyjqd.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xbbmtdxw.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gpyvtply.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xoipohkz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2hjxesigu.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2vmaczpig.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xstnxxfz.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2zxkamixl.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2otsvfcks.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2nztwwtlj.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qgdbzxxu.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2pqvxgzcp.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2pqjsvnuz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2ixmacjgq.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2pvmocimg.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2azuocklh.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2zdyospko.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2mreqjfia.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2skvomriw.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tzgbokeh.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ijhziyao.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2bgmtspyk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2troeaogu.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2sxdufzcf.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2biukxqfa.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2kznqchhr.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2wpoxwglr.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wembsiag.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2lnxydpub.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2apetxpxy.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dtfipbfk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2isczkxya.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2wcfxwecw.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2qsqjadqh.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2bkmbmpgx.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2zymljpqe.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2hiplnjgp.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2wfecsakv.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ihnjifut.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2udibzgkz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2rplanyjn.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2lsxfxlsl.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2jwlmcars.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2cnrulwxe.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2elrugpwq.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2undxysmr.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2udkzypzj.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wlnpatwp.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2bckzvknm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2hsfvmhby.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2ycmiyjba.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2jvmdnpix.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2olgzldhe.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2qtezubyl.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2wiysqebq.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2nlgniknh.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2xtzhlpit.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2xbqryxwl.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2sljvurcd.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2mzsmecfc.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2fcbbyxoq.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2ahqgosnf.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2qmqgskws.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2thfuemlo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2cpieskph.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2jqasenuf.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2mtfeukfj.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2whxlbcdy.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2bttzawgw.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nuipmczk.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2pzcahssi.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2cahddvcs.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2sphwclny.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2emadbrjm.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2gvsiijmt.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2kgmyoflf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2rtmonxbq.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ebjnywpr.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2axgzdbdb.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2mogakphr.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2zeupbtcb.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2npyufhrq.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dvujiklz.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2frlzyxlr.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rjyoitvn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2spxihnrd.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2jwowctpd.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2kfiehife.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2vhehafvs.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2woxjakxa.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2emgqzcrg.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2zurrgdbp.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2bzffxmtl.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2qjcoufid.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2oaihnceh.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2rudmerec.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2nztdrvhs.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2yrdbtber.html


<!-- 参考信息 -->