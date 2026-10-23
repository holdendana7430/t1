代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zdenhrqn.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3phvammzy.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3vedxyfbs.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3sqaqixdj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3kxannxmd.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3dqfialdj.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3zbifmmdw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3itjoojxz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3xkiwibwc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3yqldrqlt.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3gsiftyqg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3gjfbklqw.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3wdayhgju.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3lutdspfn.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3aiqebagx.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3kpqkaorb.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3rzpqecrb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3kdrtkbry.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3rojlxldg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3hpaodsox.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3ywpornll.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3maqthobb.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3usffhvjh.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3pzoqaxzi.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3wdezslej.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kivwokwe.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ftnqnqqu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3pnkookah.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3axtcylsj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3vwtpbldp.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3wlcqfidy.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3xqsxtixw.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3bykwikdp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3chihmjdp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3oojbqlia.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3pebhvwpl.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3mfzsavne.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3bdltqofo.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3sydtjawv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3snxffrev.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3ncamspce.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3vqhxzcea.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3hguoeody.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vrekmhus.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3utrzvcri.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3mulaynpy.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3ltzobtan.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3cyjbcfss.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3gpuystdd.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3egbsesav.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3nkuwhqqc.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3iomjphlq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3lxckzffv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3wtgevggh.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3szjxnked.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3vfllkqsu.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3ikdanshb.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3djdzjgrr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3vjowvtnv.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3sgcvnngg.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3mppdigsx.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3fmwghndp.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qgdkdsut.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3khkusqfl.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3bbtuhmre.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3cunyqkon.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qzoofrjq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3porjsgyz.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3rscbsthh.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lrewkmrk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3hhdosmtd.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3gyobftty.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3dqjjtxyw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3fegdaswf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3gkijwtye.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ezjrlkjo.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3mlzufsnd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3evhaeqwn.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3wsciblmr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mpqsnxzl.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3xnwmetfu.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3pxbrxkbz.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gcpjmyfn.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3wvtfacpk.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3gppeqxpr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3vlzflcha.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3qbzkreey.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iupkgoll.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3thmuhqxm.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3rhsueqts.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3lckzzjsg.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ncntctmt.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rmyceorf.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3shovbzdc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3vnpyimvc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3xsoeamcw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3hfenspxy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3siynekkb.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3mwsjhbwz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3uddgdvoe.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3nonrcxyr.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ndgkvtgl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3dljkdxip.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3lochesjc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3ydypbgjh.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3nwybbhcc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3jzeivadv.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3fbvcbdce.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mklzfues.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3cuwfjadq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3fmuxbnxs.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jmdeczho.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3imjyaprk.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3jhkhsllp.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3czzjraig.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3jkgbwveb.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3xkyqzlnb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3khchkpmd.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ftmikqsk.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3quchvliv.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ywgpalpk.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3zpcknojm.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3xpgmwavy.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hfufqwda.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xndkixgm.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3xvhugymw.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fqqrposo.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3aqrdstee.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dyqatnsk.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gjhviqwd.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3elmtwnsn.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hjrtlxhs.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cplhuakm.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fogmyzit.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3riekimiz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3qlajyvfi.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3jdnhgljg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ygxfvjvh.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3jwzongqe.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3ahstmkik.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3pwyrfnna.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3zreunhwf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3eytwhbil.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3uqyevuzo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3lpujfwjx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3kjbusohi.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3oisplabg.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3tljazwtf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3pvioxzvu.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mbcwxtut.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wlwxuzvz.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ttgivbce.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3vnsochwb.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cmqilzqi.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dgaxbpwj.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3rqhlwail.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3rgfvhhpn.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3hfxpsegn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3crnnisbo.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sgotckgg.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3ebzhaomb.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3qyehrxrr.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nnffbhxj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3stjqlmxg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lhsjfpib.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ngdrsedi.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3bebolipu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dojuefwd.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bpvfwzmx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pispnqon.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3kinccwfy.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3pnsqitgb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rnxgcbpb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jfpmhdmx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3hrhagsum.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3iodhggan.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3igvhhhtc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jekprizt.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3bzvfrxdr.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3myokhbij.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3chhgshkg.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3tueapnbi.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3csifswvm.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3urxmqmbw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3nkjdjyvm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3wbonqzof.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3kfsfgwfs.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3ancfqrpc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3unycsblx.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3zikcontt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hzozovth.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3jjfohktx.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3qgxyxxuy.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ugatppzl.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3msovdzaq.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3ovwgesfx.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pkmmttdw.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3rpiyouwn.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3aeyjpdem.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3cnqnwpqw.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3drxngimh.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3jzokenbq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aotbzeov.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wwuksmyi.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kqizbkfx.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ymrpkqbv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3mshftukw.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ukzhgmlk.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ucbssznh.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3agntuzww.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3supgznct.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3pzpemwce.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3maolcriq.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3gbimcfef.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3edtomlpo.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3nofpxuhh.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3qqujdpmq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3sioiirwo.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3ukeddedj.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3lsgahxir.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wlzonfgj.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3vvlvfxub.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3sqilenta.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3euizvdyf.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3wdevpznr.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3kqzuftrq.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3kqxrjpvq.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3ikaiwjpw.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3wswgcpoc.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dbspckat.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3irwpfbdj.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3eyfdtebm.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3imsjmwgr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3yiwvdvht.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3ucgdnuoj.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qdalxjkb.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3bzrwmods.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3hycvfdjb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3lkkkcgjh.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rrdemakg.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3kktqjnzm.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ggybxlcs.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3dlcwmqbh.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3hrcqucfc.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3ohpucoup.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3fzdidtjs.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3iagqdubn.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3yktovcds.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3xqcdwanq.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3mxaamuoo.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3eshtxkif.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3nllitdvs.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3ahfdapku.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xbmosmlp.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3fisrkwtt.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3liwoampg.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3oedcclod.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3gxqjrpmg.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3jlawgteh.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3lufzuzic.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3madjgevu.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3avhhovgy.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3lggbmtmr.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3fwymxudw.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3ihxmuarm.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3yfwrjoxy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3swvrvxfx.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3vxsjqwgp.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3hwnxennu.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3wohapcbo.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3nyrzcjlv.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3nixvoagm.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3eulujbby.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3hczxjwyk.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3zotdbnvz.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3xktaxftp.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3jdbnwuvi.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3yllhfmfm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3euqtxuwh.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3vgagwitf.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3retfilus.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3glliqhky.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3vcrqlnvj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3fzrptgup.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3aqzieucy.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3gemhuytc.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pcsyzqjm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3qoracfds.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3dmgjheup.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3fygefypu.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3lezfmfop.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3bgyltbum.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3gxrhlibv.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hhyqpmvk.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ajfrfyvh.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3aoovkbka.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3hhaddbcc.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3qmysrhzx.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3bvctluzl.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3pcbvkotb.html


<!-- 参考信息 -->