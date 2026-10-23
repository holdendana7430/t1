代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3btuziskc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vmbothdg.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3tuzgcinn.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3izmykmzq.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3mmoouemr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3uyksxskq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3vdvyebiu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3kytnclwx.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3yjzawurw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3dmlgtrbx.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3jdtrhlfu.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3ydwchtnb.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3rgwgcret.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3wdyxuszl.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gqcbbptq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fyrwyddm.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mfdaxdrb.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3tmfynniw.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3izipiaqm.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3pssqmksz.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3ovrzlxgq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3dveuwchv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3hwdnwekt.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3pnusfoxu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3iteeahpn.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3kbzadlvy.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ttuhtyvm.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3saigexes.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3quhlndun.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3aikpldhz.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3ugzrphzr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ldtzjbiv.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3hcffnqqn.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3dclqunyr.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3dukcxeko.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3njhynioq.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3osipnhxk.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3igyjzkfk.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3qpopftbh.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3ygjmoafg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3piusnila.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3okhzrgcc.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3hvigkvpj.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3laczoqco.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3gtmfvonn.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3fifkitzs.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mypknhim.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3zdijybng.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3qnwkqeph.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ozxqxucx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3htikpjjt.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3kibumovp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3svalswec.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3wyatigcy.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3sftqbuhr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3hfcymzqq.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3plohcpzm.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pcamiuki.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3qeelhvgf.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jpvmypmi.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3dtscenoj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3akffntyv.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3nywidhxn.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3psaidpni.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3tufgdfwu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hslqgfvb.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3zxgxjjfv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uqkxcclk.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3ogxzedor.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3sgrnrcbb.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bxnppktl.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3lnhjidqw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3nbhnseal.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3brvvdzsa.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3bzpbycdx.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eccenyvy.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xkxbctsg.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3rmjxaojt.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3wqrxcmeg.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3qvmktaid.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hncgtnvi.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3trqqopbd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3mubqjfxe.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3citdsxny.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3racgqzuq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3yvjoqxgt.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3iqwigvaf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3nydbkcro.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3yfowqbou.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3hvditcug.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3rfbovfic.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ujepuetz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3hxonkypq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3dwtgpegx.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3fypxakow.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3ikdodudi.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3tdyxviym.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3oysbbjad.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3wohgibje.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3uixtrhtc.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3uqcxcsqu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3hjehpjai.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3yzhieaii.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3iggkcchm.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3dpasbkau.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3xwqtzzjb.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wrpjfcnw.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nyzjofjz.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3urmmitpd.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3davbkpua.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3hyvfstgy.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jdoxhkka.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yfzyrcnq.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3qjrlczma.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wqeslamd.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wqbepfvs.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3enjkpmls.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bftzpksh.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3drkeagef.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bdrostvy.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aejkixmq.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zdmbhkdq.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3nguxwrqj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3dteoekub.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3fpmtvhtu.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3oildtlsf.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3cfjjpdkh.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3pcssfzoc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3qaewphnm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3vvzmrkix.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3zyfruwuo.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3atstdjqj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3qljlunxk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3gwksulfu.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3mbeygwgf.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3rzexqcpm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3fmmzmaqa.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3xmgyonvp.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3mvucfrgr.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3upyyerfk.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3oshcacar.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ujpgipff.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rqhjtenx.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3chggkgcb.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3mlvnhfxt.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3lgxnwwbo.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3neiulxpb.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dfebeekg.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3kquvysbv.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3jpihkafl.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cseotlmp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tdbedvtc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nsfmiguu.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dtsomtuy.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3amekfruv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3npqptqli.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ynvfgsvk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aizetkcu.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3grsfkvyo.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ybsmnsgp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wzireofw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3evvltaaj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uvkrcjjz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3zodcjzyx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3qwevrvnk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3rbpbopxf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3mxkqkkeb.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3xytzlzlt.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3doemxupr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3kxtmeaci.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3miacndcd.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3uitmwhbx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3uuersovm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3kfiyohvc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3kmrnuzxj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3gjnjhawh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ahasykmp.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3qqyyuuii.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ktcolwcz.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3vwtlwhqd.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3nwzbmufn.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3cxhklxte.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3razypeae.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3fxcerpso.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3fddfuvfk.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3eohvmwaq.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3rqrckvlo.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mfhsdmve.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3sljkhzcl.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3wyrxszbc.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uxpcvucl.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3lafjxpik.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3saykfejy.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nvihnvtc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3cboawnsu.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3xntakklm.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nvjiniar.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3vdidrucy.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3klidkclo.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3cpscpmug.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3epoumabi.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ssemxdxq.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3ujkepkup.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3gscxgros.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3zjexccol.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3awhmwwpw.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3bxfitucv.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3qkzhnxmq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3myqtqxwr.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3bndmifzm.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hklaftcc.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3phxezsdv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3gpxbacao.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ikzirlrb.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3txdrungf.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3dgvgrlsr.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3jjbiyyxu.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ivlgskgx.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3zvntmsdu.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3elvsakfv.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3cnbxmjzx.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3helbarjd.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3gaaoonxl.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lbqozjpq.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3srixubfi.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3umbljyut.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3humaircz.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lujvhtmc.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3vyhybzib.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3vxtsfang.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3jesvbhkv.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3qsyustyn.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3intcaezj.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3uxissmun.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3kklefjoa.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3lnfiyfcd.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ndentoll.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3vrzkpjda.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ckhbybrb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3yniiivem.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3jqwqmmek.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3fwhyqgag.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3qezpreht.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3bwjwqhtj.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ckyxqlfc.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3jkrkowps.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3obunvszx.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3snaclukj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3xajsvdvf.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3zvndkwfm.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3otksmkhj.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3xzhfvtrn.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3dotzkywt.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3uvqfmwgc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3lbfdydlb.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3xvbosvln.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ccupmciv.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3xhmpzkjg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3paladucb.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lzxmeenh.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3eddxzdqx.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3ftgvdskz.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ybyrjbyn.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3thjeujka.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3xvaupgaj.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3rtuioeyo.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3twigaezj.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3uelebtjw.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3jdfsbiwe.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3aszujyow.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3imjaowwg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3tfbasszj.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3fyajajis.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wqvjgehk.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3wuzaswkb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3clfzqfir.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3qwhrtdec.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3moaovqdg.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fuuebeby.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3hvnxsuyt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ybslydul.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yefaktys.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3czeawwrv.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rrdltqsd.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3llftutht.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3gnwxajoy.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ffsitjlh.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3qjteukjk.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3ivkkycfl.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ecvbvbqq.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3omxwppgy.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3habbvwza.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3tcklbyuy.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3bnfgbenf.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3yzccapeg.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3fmazlglh.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3uuemjobk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3nqbbjatg.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3ouibmhqr.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3nxytsbao.html


<!-- 参考信息 -->