代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zndtvxqm.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2pxnqqxvo.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2cozgfjoo.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hpbxayqj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2iedeskpf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2siklgkta.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2olsnnqvm.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2czmxsjiv.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2zyhnpghw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2qvznkuuh.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2vjuptgje.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2fvqqmdeu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2ufyfkaku.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2jkikskcp.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2viojjadl.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2mkartgbu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2jylqohxw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zwhfqsog.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2eecwllsg.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2bzgbqvag.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2prfvoyuq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2oofpxjvg.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2uliiwtak.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2swapwirj.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2ueicewfs.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2hvmaadyk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2fsxtbckj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2rlgtgzue.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2noywkkes.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hpdjwnxp.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2djzucsvy.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2sdqskfxi.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2ffsustwo.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2pobkmxob.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2rxbazxwb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2iqozzuul.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2yoloomfr.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2pxhjlkoj.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wmlwlkou.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2npqbgxnn.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2qxfxnqvg.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2vjrumqrm.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2bcoaepqj.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2ruroldvw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2yjwkqgut.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2zmlwejbs.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2jblwlwac.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ozsehyzq.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2xzneghna.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2uakdxpha.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2smimkytq.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2wgawmvvx.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2pqjgfraw.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2vkhvppsk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ecjqnwip.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gvsseexa.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zrcmnzap.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2msforqny.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nzgsbvxh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2okzrhhit.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2jshxkoll.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mhhrasaz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ekakwleb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2lrgpwmyb.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2kmnvopkm.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2jdyeapgi.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2xqkxtclu.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2knkhwvhr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2fxryimce.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fdltprvr.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2rosnkuum.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fjjphmkj.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2xkrvocet.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2gmskrgsx.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wulgsnqk.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2xitslcno.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2wbgnqrbz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2fcjcjigu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2qaxxvthc.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dvgvpzxu.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2esnmwidk.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2dowzhwch.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2peoirtjh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ygajlcin.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2vjmnsruh.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2nwxswxgt.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2uqbleyls.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2xhgztnnk.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2uzpvmuiz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2zdhugvex.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2xdaxvwin.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2nildapqu.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2hrynrbed.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2tcwzdjnx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2nhskmdrt.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2fdwmqxfm.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2sawzihcg.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2cgrqhzko.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2lcceitob.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2yijnurhw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hddymmjg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2wyrhlrsf.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2visuuppc.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rqnivdmv.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2kvhyaxly.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2smqjkcly.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2ozqbwebq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2sthdqsae.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2dysvdave.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2xavayzuq.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hydsucsc.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mzlpemmh.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hykkxpjn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2xlmajsmj.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2ydyrkcvl.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xrmbzdyj.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xrottsol.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2ibqeuabo.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iapdbely.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2perkkmjd.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lujflppx.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hymqfiud.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2iipllaoa.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bnnjjwli.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nkldtwsc.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lruxiurg.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2ykyaykeo.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wodgvtkj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2gscqvosd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2qujqgjyx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2kbooiori.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2pnxaukyj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2futykvmq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2aykyrpiu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2yxmtclbc.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2fpkjfwpd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2plectjrt.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2qdxcdatr.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2nmcqvbfw.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2tfthntpd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2mrpjkqca.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bujyqrfe.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2iiqslhik.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2kcgugbnd.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2rwkjsllt.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2motawfhc.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wrfychux.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2mvinnbww.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2cmmomzio.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2qsuixsqw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2vwbnfpwi.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hmgfxame.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2ypfuwrkx.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2gkgzwbqp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2miznwbrx.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jfjimcxo.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hnkczcor.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xhrnnrdo.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2vlxspttm.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bdzadhfk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dlgqlmqg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gsgvhfsx.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2kbidfbzh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fbaniqff.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2zzontyco.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jcnrashh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2mmuqfgoy.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2jzhefitk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2irfrxxht.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bjndtrwo.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2rlqjupmc.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2pkbhtoes.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2esfwqoei.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2letrmpvq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2gnjxxgds.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2dkwghyrx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2ahwaltct.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2ghstbujh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2fxanpnew.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2shaxptaf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bhlqqrry.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2yvzopnvc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wlenjisu.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2nxdrhdmh.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2gseyjoeh.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2fytuxsvp.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2dtnytktm.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2uiqinytx.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2dyjjjkgy.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2cnwhbnzw.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2adcmxcoa.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2hqnljrhf.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2jsblbvza.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2bbulxwqo.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2qlgumzcx.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eecnvhmm.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dqezpzzp.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xntwfcge.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2xuoqguup.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2zwapnbci.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2wilqfzrz.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2rnrfvvnt.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2wemtvsca.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2knctfzvs.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2engyjaqr.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2pecbewqq.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2uovsxelz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2typvvqit.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2irfgortz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2hrphjlcw.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2zfeqrybf.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ikvwhmky.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rqkkscww.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2xwtzerwy.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cpnolibm.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2spmokoit.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2kgxavybh.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2oelvojrx.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2abhntlba.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2iycacwxt.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2fyyswisw.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2makcvayt.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hrtmorme.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2npdgbxll.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vnblpjto.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2mnmxlyoe.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2heraoflg.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ejgzyuiw.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2voajpcsx.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2dxygveev.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2zhpflfbp.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kibgwtqc.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zvaehiby.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2jhayimfs.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2rsrasspx.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2kpcsleea.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2dopryden.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2bmtcpona.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2nedtqyeh.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ldejxktm.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2exesofrf.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2hgddkggw.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zdonflnv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2ucawbfmu.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2xukrceuw.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2ozugasfh.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2znqusals.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2ihrcebtp.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2kiijhpqv.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2rtalcshh.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2lfwpcrts.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2tkedarxp.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2oqrdpuvw.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2vwdffmpo.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2imgfbawl.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2lpzimvpw.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2wgerqsnm.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2bquokbvn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2gqzeyvwg.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2ahhcmzwo.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2wxqdjyvh.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2svofuunj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2xqpfkvur.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2mzsaekqf.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2zhjcwell.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2quqnkmrr.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2uydbwulx.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2tejuetyo.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2rebgakfi.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2qcdicdov.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2rlfihjfo.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2rndpqfue.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2rfflyqya.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2yfmefulb.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2lwkpefoh.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2bywpkdet.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2jioyiyet.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2elhubczf.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bpxzrctp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2teluvule.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2jjekojli.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2qiclxqcq.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ubsuxkrx.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2rmavnjsk.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2zphcopgc.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ihkdocjk.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fjfvgdid.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ihipytzl.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2qfrdxnyt.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2qthsftee.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2fpxokgdv.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2hrgeruit.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2nnqzrcnn.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2amltfpth.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ubnsusuo.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2wqewxfpr.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ryhrffqt.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2bawhjncb.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2hvrpmlhq.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2poadkoim.html


<!-- 参考信息 -->