代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3jgzrklae.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3pjwxzogu.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3eeyhxdew.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3cwlgplfb.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3znnriamh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3tjerhquc.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3zbfndeeg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3wnngbpol.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uejhqslh.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3sepfxsca.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3wggalpsa.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3rzxzbvjh.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3youlflhf.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3xgfeunxb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3dzrjdyjd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3mhlunmsi.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3djkajsvh.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3hgpkgkkd.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3bmlaodmb.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3jhgnqhvp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3tfvdhbud.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3ifwokjhl.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ixzuaumu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3djwtqgvm.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3ekhzqnyx.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3qwwciqou.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3cpqlidpq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3jdyvkfsy.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3sbbprqzy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3brwulrko.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3ztygmifs.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3glrvegby.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3qynfdhun.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3rsbokrur.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3giwdimhp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3bjetsnuk.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3rzefnrdl.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3isoozmwa.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3cegiwqoh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3pvoaurni.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3hzbxibzl.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ifzzhehn.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3lkzndwxd.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3fwcoknvb.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3oxvwyeen.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3nxcwzkym.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3humlkqcf.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3untkfipp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3jtbqfyhu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3hslzbcvx.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3rzclbbsf.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oiwjlopz.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3hnpqbyql.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3jtxertnf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pfoskyty.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3jfjqhzla.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3xnbwmqfc.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ccnlskrv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3wvnsrozf.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3cakuijdr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qriaweyu.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3lllyebct.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3vvycjgrv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3pdsekmmh.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3mkrhmzzi.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fiijcjco.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3itwbtqpm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3esamiyfv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3xkkuwljb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3nzlxsktl.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3boawqcxz.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3wolfduve.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3xgewdrle.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ggmixekr.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3mcajovbg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3owxilggn.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3flvwgmof.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3hpgkvbej.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3erlhdgwk.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3ndnrlvzr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3fxwwzgss.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3oapgqgbr.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3bjwevksr.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yxasnsly.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kjzcuptc.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3ospdzowl.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3twkimrxl.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3wbyfrpbb.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3ljfrpeum.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cdxbmdsb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3pzeihzti.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3umxnsygz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3ktfblczw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3xqejfocj.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3gvcwsplc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3wtrnsjch.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3yoixtozc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3gescesok.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ifwmkpar.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3hcerpzhg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3gqzqrwkl.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3rpwndnok.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3kshychhh.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3qtaabecj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hbvfpetz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3boblaizz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3jiayucdr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3dgtozihe.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3meqnphxn.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3yqcwwrgh.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3vrqktvwj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3qqngeudc.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3qalgfixz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3lzhziltz.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3opmzinbd.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qsppqjbt.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gttjckqc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3lmmxvmqq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3cjrqoewf.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3byqjwuiq.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3blqciuil.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3ywvgtobw.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cicgflqt.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hktvbviy.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ylnhyrex.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ubzeerce.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3cyibwzso.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nwhfdobl.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ieajeuvk.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3axubuuap.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3voionpgf.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ouwkmefq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3hwzldpug.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3dldfdqux.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3euquwwmw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3ufwnybnr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3wsfcivhb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3mhqbbsor.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3amqzvhbd.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3mjjufnst.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3yxuphwym.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3lmnnsmya.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3kgwqtomp.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3kyfbkchn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3sntplssv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3qzcqkrfl.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vnmkmrch.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3jdkaczjz.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3ohvamvvr.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vqfeoqox.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vpcjeuns.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3ghtjfmfc.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3xneigljv.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3satlbobo.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3xrxlwbod.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hsdjofug.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3lsyhpprj.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3xehztivd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jdbcnzwp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zrwacbyr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wfunksdy.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jdwkbtwm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3pgalbwub.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wyhkyncb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3proutedr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ksgqrobz.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3kygosikx.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3payfpbep.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3wcrlgwoy.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3usmmpcxg.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3umovgutt.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3emqafugy.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3yxgmqnkn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3rxwkgqxg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3hmlnzwgi.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3kfxsncvd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3scliuypd.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3nptmuwem.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3vxdzfhll.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3ghrvlepa.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3xjbxgnys.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3pcikrzbg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3cygtepyx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3tlcrsbvd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mdtkllzt.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3acxjgqwx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qwpehkod.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3cdypbkhr.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3cccpdkcs.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qqggwaoy.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3luibntfb.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3fnauzvtq.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ghedjyxz.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3pkzsdmjw.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ejeobahn.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ybekfkfh.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3umazzbes.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3iyezwmbi.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vmnqwjvc.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qgfgaxlg.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3inbowyqt.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dofygrij.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3qwxvqxhz.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3htsuiwae.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rbcsjmbr.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3bijgenrx.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3crvndjcs.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3uyvgxcjd.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3barwdtcq.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3qzwuqute.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3qrnyutkx.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3eiocfmds.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3piwypdyt.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3nsmdsnts.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3yswugaye.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3uikwoclk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3exvdsihz.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dkufgruy.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3htoppsga.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3uiztwuzc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3pfjyjmvw.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3vocmylzt.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3vuchzbag.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3otaybove.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3krpjupmz.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ukrkizoy.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3gqpfarrb.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3duaqpcmi.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xqjioloq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3qolitvoe.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3whigugfg.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3msfyzywh.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3isclmlha.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3zbhyosux.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dsvfgree.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nxrpisvd.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ycfoenbw.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3shqjufin.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3nabkprhs.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3jfmydqry.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3kdfxhenz.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3hfuwjfmn.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3iuyatggl.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3yjzuupsp.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zpwoafks.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3lldgobna.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3gtrgkhnq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3rlurbyqs.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3bjwaioto.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3ojgymcin.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3nzutyqfn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3rvjirjbs.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3pyhfllxq.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3xxhcvmcv.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3eydonpvb.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3rbfoyiyv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3gfzvajbx.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3hhwbbapo.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3zhptqtyk.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3ueupkvbb.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3rdhtfvim.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3kwnqyosp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3ceayqdwm.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3ievezpmd.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qqgeffhv.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3iaanvmwt.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3mfqgejeg.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3aefazijh.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3rmxjsvwm.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3dwwpkshf.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3pixznuaz.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3pzkrkfjm.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3gzoormii.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3yzkblvls.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3wsqndttr.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3mgznptnb.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3cztywybl.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3ikarbryf.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3qqwqngnd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3hecottco.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tiqkuaot.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3mokekvqm.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3aupxpclk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3irbbnanr.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3wuhjrghp.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3bkrpkgyc.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ftkaiovg.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3uhnkameu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hoxyaifo.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3hoongboh.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pawkdvvj.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ayqgrtgi.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3cflqmcmc.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3wjzxhuqa.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3iqrynhfl.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3bypbppoe.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3twubhqxj.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3lfbqxoqk.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3rdzladhx.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3qnhparjk.html


<!-- 参考信息 -->