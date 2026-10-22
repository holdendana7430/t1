代发 wailian999

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2bidmxvqo.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2zimgdbtd.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2fmohcrzb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2adppvlzd.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2lylykuaf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ouiuhyoq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2ktmbambo.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2gxsmjbwk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2tztygvns.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2xhttjihd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2rgkmrysk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lytybepf.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2knniemcd.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2wufaxxag.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2bgbvqyxo.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ztghjgea.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2ibauajrz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2icyhcvgh.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2urbcqusp.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2tqjkysxc.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2oreefkag.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2vrjmaabq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2mstclrdx.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2cdbqflpe.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2rgxvsgbn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2svlloumm.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2hdusfiaj.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2kjfejnat.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2oxohntpg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2gbpzbdsd.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bnvvjxjp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ndmswfey.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2hkwxjdzy.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2yjjsozds.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2tookkwpm.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2tlrgmvni.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2segdsanw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2ochavyfs.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2shmuvhsp.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2lqirflwh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2neawllkh.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vftvmdxv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2wbkzqgxt.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2jqgnwiag.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2yvvrinhw.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2nzhhlrva.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2fryiozgv.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wdwnpscm.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2zsvfmdrw.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2jpefkisn.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jjwdkshw.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2fdvgsmsm.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2sjsegzsg.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2njkxyozo.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2upzowggt.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2catlcszm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2zqliptrf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vdftkbhr.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2citsrwjm.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2qhvkkoot.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2jbcnnqoy.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2rrejzvow.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2pygobsfa.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2roozcfpd.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2ltqtsccc.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2oinkmseh.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2wafreswb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2wfosypfw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nytahjrg.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2jbuvtnjc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2pzcwvqlc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2khdbmvyv.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2optdoikt.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2phjcwfgz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2rwymvffy.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2rdcfldeu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2hjtuhmoy.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2esaclaib.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2kdhqydrz.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ipdfwgeh.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2bimwosgc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ccfprubg.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2wunfztaf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qcvshpvb.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ltmeszbc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2dpluqqyo.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zrbqilkq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2wafwllsi.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2mpxzkjhi.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xajxznte.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2duhmnuto.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ouufepja.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lkmgbrpf.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2enwmyzqj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2klmsldnl.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2cpiaafpc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cdfxtvqk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2naynwmnq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2gmnehyxs.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2kynsuqnb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2lfyqpbga.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2rcocvpam.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2erpmtxpf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2pkqnvbyv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2bovuuhpd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2cdekcdzu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2vlvndcvr.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2zfeamcei.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2zojdntth.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2tphephrl.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2dzamhrdu.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2wvkipqat.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2cetpzlpt.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2xzeammwr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2bcfdfpii.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2keqfjqhj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2tlpzvich.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ameztmly.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2owwqmypg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2sluenigv.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2ifdwyuzd.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2qkhhdbqx.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2trfockbv.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bsdpvgqb.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2urhmkoiw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ngyuguye.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2nwnnouqt.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2olmvprfq.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iihfxovm.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2qbhaazqm.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ryhusjzg.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mytzggdz.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bdgdjajh.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vzeioqvy.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ytinmops.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dnfwjeqt.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ttdyzhdp.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nfoylspl.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2lusoeirh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ptmyucnw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2kkempldw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2dgexiiyw.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2nlkjaisp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2ktmhaanx.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2emwjftdb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2opozwlfj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2ojlrosqo.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2dqiftbqo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2wlfbqsqc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2pycffqxj.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2dxqrxbeb.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2timzrixg.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2getaqpdu.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2pkibwymf.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mskrdksh.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2uxtiaaoo.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2hkkkavlf.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hemyjzmn.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ljftcmov.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2omhvgqfc.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2owupierj.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2eacwxcaw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2uvjubepx.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uxxgdgyn.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2lkjynxoa.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2yrbrifje.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2davodsqb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rszjadzf.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rgfhqaum.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pxmnyesn.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2dtpdvoyi.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ystulbfq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kxiavzyx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wvhcqhdm.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2eaabmhtz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yojcbuta.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2zbnvoemk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2aaqliavp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ivnryfjr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2lsiptvtf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2klqslrvb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2nxbxkwyu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2kmebuchb.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2xlvnfytm.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2rrqvfogn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2bbfoflqi.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2ljzlzoll.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ohtfjvnh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2ynxhxmjz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2owgblfts.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2pmulgprv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2jcgnpnxu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mvabxwde.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2niunullf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kpozyyez.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2eflyxjkz.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2czapfsnz.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2zectsubz.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2tpddgmbd.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2drnuhdno.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yycylgvy.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2zsxhfsvc.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2utnpbhiy.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wzmgamxo.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ogkzjjjz.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2hpvglgnm.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2tcxyzffn.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2rtgtjlni.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tpzchstg.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2naemqizh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2ugvbtpnl.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2qpsywdqb.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2wiownteo.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2gtdtrcbp.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2asxtdvve.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2aitjwfbx.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2yhdauebr.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2feazvweo.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2ypcrnhgy.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2tzvhzifd.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2eqpkcpwc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2cgqbturh.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2zgqinqve.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2tphjisro.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gmumvyfm.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2naeroehq.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2tklygwoc.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vcplrlgv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ipmfzsqw.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2eqvxaihp.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2cadzjfyj.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2imwzfiyl.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2pbopspxs.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2suopgxih.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wdixbqts.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2fozzakqo.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2jnprkklz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2szwfhzia.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2vtgmcyph.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2ykbzjorw.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2mremyspo.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2etsfyoym.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2blsoozlp.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lyotlxcc.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2qmmqoucg.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ttiqjqyr.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2wjzceupk.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2sbsrxtqn.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2fotggaji.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2iaqsvujj.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2otdgsqur.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2picgrroy.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2tiysgqcj.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2wsbapkdr.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2xkryiniq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2epohhwou.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2wcyspfgc.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2nesjqdea.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2zpwkwips.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2vihymeus.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2zhlsdnoj.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2amkvhipu.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2yepalupo.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2jbugbffd.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2fkrwfjbu.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2vjsinuro.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2avqobadq.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2hzxavhdn.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2vilvbzti.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2rtazasuc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2wyaoybmu.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2giivdlyq.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2ugmmiwks.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2azbpzhhc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2iupapbhr.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2zcttcpdk.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2zqaqztml.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2nrgmtocl.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2zhbpzjcu.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2mqmkpgqk.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2klkdbghz.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2hjakftoz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2ixmnchmq.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2cztrpows.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2sgxuwmst.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2jhzewpfq.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2gnvvuiup.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2imzlkykl.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2adwserwh.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ppfjfnmq.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xelgyiss.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2jvdrbfxn.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2fzpydtua.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2fteimhgw.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jxbobtnc.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2pnzqyxkf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ebswybbo.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2jeseahvx.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ougzhcld.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2svwrbnne.html


<!-- 参考信息 -->