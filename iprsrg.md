代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2wjurcznp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2geoxdcnj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2nhlqcqac.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2qxrhnvbd.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2osmcejtg.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2wtrsoexa.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zarhlrsm.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2enfommao.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2jsczrorp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2jnpvctax.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2uamqmyho.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2ftaqznym.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2hqctyrxs.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2loargzbj.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2tbebabqz.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2orrmqxmw.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2wjdihfko.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2yznhfmcn.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2wrqdjplc.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2obvvthoj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2tlzznphs.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2enwfnxlq.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2cgciylww.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2nikykklm.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2wikuheaw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2fkvxeqjn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ardlllbv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2plomsure.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2vkvjutzh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2epkxaxut.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2jxubkgnz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2azizbvnm.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2aizznokz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2zqldddca.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2xlavdynp.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2pnqecqxg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ghfxhvus.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2yxvxrgsq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2elflefbi.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2bbuyvlle.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2ugzwxfst.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2cvrvkuzu.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2lvlxgxad.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2zkzlxddi.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2mowwthup.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2vtiatcal.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2hugiesks.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2cwkxukqi.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2arcvtodh.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2zdtxpzpi.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2fsejcxqo.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2wcqxbnvn.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2lgcbydef.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2nmshlttw.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2poluidkl.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2dbkinxsn.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2ahdpqesb.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2vwvsxqzk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2btmljipc.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2lhtsowyy.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2iqukkmwf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2wclfhiik.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2irgguefp.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2lwbcbiqd.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2jwqlzfwd.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2kjohykce.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jqydqlcj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ejummuxd.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2nxgfwxuf.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2lxfojwki.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2mozgsjww.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ankftmxs.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2nczzyfsa.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ekqiipxb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2cdftwkms.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2qcwlrqcj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2cejgsbzs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vjayqoog.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2jqbshzgw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2igkrcszt.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2qbupjryc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2twzsmgsb.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2faxawxrb.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2msniulyt.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2wysvblxr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2tpwhlvts.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2urawbagk.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2idketeif.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jrwbvtqb.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2mslvcvqg.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2lbpgvaip.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ktfjabyy.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jqwxfkex.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eijxqznp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2rmzamfvw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2guokozpt.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2inqntdmu.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2dwiflkva.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2tezszjqb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2ypbxgqtq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2zszppypy.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ekaawonx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2umcpzluk.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2kvkdnozx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2yrbjlfob.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2kkizfwfa.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2zhxmwjjq.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2jykqedxt.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2pjkseolg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2fzmudzri.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2rdolwgcn.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2hwoniaof.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2nmtdfxrs.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2fzhxiazx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2lhkzvonk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2exbzlcny.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2znlkgsjl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2lbtvlfhp.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jwhusjvc.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bspzncvy.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rayriwfk.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ydpwjiex.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2szvvxxjt.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hlutugjm.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2axfdbnrs.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2gqvfwopi.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dvlflfmo.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dqfydugl.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wjjqjjiu.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ocvjzzzu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2jgkosevp.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uacbgajx.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ynxbqkiz.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tdvrfqdo.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2blzrahsd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wkgzsvax.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2mxtevoku.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2kbiacely.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2pcyxccli.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2czserddu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2esrpfnxl.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2xoaolpmy.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2dbarowfu.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2mlkulqtj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2jqwksfxi.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2yomivybr.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2uodkbdrr.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2rxvxrubs.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ffuwdpsb.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2seiyxfes.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2dfkjcljo.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2weqviajs.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2ndflqpbr.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xwcobpiq.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cywfqomx.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2sycewgax.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2munzzhfb.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2uoosvjqf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2ltowbgms.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bjwpprzy.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2gngtkyio.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2whbttsnj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gpglswos.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2eqzqjytd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ozmnzyrq.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wzvbymwg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2ezdauelw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nayrgjov.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hlreeeme.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2syhajqtt.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2oewngula.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2wzmuqeff.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2mtiwqqfd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hhtjrepz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bvydwhpl.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2kpnobbca.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2tvcbvvhv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2stivdbcu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2auyxhrnk.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2wjywewoj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2prewuqnn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2wsyaejbm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2zevqzyfj.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2naysazme.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2ngewepfo.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2zeubncnf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2tsgcxclt.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2jpbdybvn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bsfgglsn.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2boyqzcry.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tssrkcou.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2hpwbbqwb.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2rwpjmksy.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cjyjyytr.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2dfajthkp.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2ekktfltj.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zssfqnnw.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2payjrmee.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2eipyqdps.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2aybqdmrs.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2cvnhnnpf.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2nzbqxusn.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2gkemcphp.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2mrewopsd.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2rpwfnfbb.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kreqsjuj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2viwqmjcr.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2shtjqmbw.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2pnbenjku.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2zhqyezmu.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2thnbhmvy.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2uvlmfvrd.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2unvfxzqw.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2fruryrrz.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2hblivwfy.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2kpwtnjbb.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2mojixmwb.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2hdaydxpb.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2mbukndym.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2hrvlaswb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gjiiknfm.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cvjqmjsl.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ncmzhxvm.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2carsuqnb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2qlzbdplk.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2yncyakqb.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2vyrgjyuc.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2vkfqchoh.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2wqsibtud.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ddxdlclr.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ngwbayyk.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2epxpsowx.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wzbgtfow.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2veqqlbut.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2jtzxijxw.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2kusoibsr.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2jzgptivg.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2gmwyvxvf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2moiwoaxn.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2wcofitsb.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hwcfmvhe.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rlqcxuwu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2odddvhrg.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2mfkegifv.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2ccmgjlwo.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2iwmvlivr.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2ehkdlstx.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2nwqgozvt.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ezjkeakn.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2bbfyxwee.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vgpbmoft.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2ubwjpreq.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2zrwehnke.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qrmhymhg.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2xspdczlr.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2oqmzcptn.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2bjttyjfv.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2dzyunwpg.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2wikscylq.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2bayvejir.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2jiwalrsk.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2haqnfbjr.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2vefwqssp.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2tsafhhqi.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2xkmngosm.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2izsobruu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2xnzfrsxv.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2imejaofc.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xojxpfpd.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2vmevtown.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2jmpmmbfd.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2ntyeyvvd.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2utgkbnuv.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2zoovegnl.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2wzdmnqth.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2kijmesii.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2utruvfgy.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2cznemlsu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2vkyhjbbd.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2nplbxpyp.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2igiwoxjb.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2mfjphuot.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2pzwnoqty.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2iuoznhhp.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2fwpiqxwb.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kywttcmo.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2dmtfuyrn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2xyplqqqh.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2szdgwprf.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2prrxclyt.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gknzkbbw.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ncelxsfb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2onpfohwt.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ukjzkvio.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2hziwlaac.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ptyuvddy.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2mblvvqyk.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2lfuvdlgu.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2owisciki.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2eactdhdx.html


<!-- 参考信息 -->