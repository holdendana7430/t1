代发 wailian999

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3usaajwvh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3bcbuaipt.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3iiljdtln.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3bbvvhbrx.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3loumpchw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3efyjzfja.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3vhokhozs.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3wzvjkxlv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3oiqwvejl.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rgovdxre.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3knsdzuit.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ejxnwydq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3vfhipbtn.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3efbemnsk.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3uwpvbeww.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3wkjopeni.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3ddkgjxvq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3fvvvilaw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3ckcvgfap.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xhwuiabh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3dcgyxiky.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3fnllarwt.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3tnjzqhbu.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3xxpgawgr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3zwuolefi.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3duildmvc.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3jywkufhg.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jfhvlxot.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ngbujyvw.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3yfwrucds.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dzsjmluq.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3tdtvdbkz.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3ibxvlpjx.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3ikaojrdf.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3mylvzgpw.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3jnkujyeu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3fbkduxed.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3vypbdssu.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3optawrko.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3tdfmnxqz.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3ofglaywx.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3awkfkwsi.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3khxzmtxq.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3vygapgnm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3mwyogpwg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3dxlqxiya.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3fctfmuzw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3qvbscbtq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3kkuqtpgy.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3qgoddqkd.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3unvzjjok.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3rmzjyuwq.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3jtsgovmt.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cetopajr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3kcgyxfhi.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3dyuwnpoc.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3uvqsfkqb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3uknuruyf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3hzawninm.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3tsideyoo.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3auvdbglb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zlyzwkel.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3nltrbopu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kuqqades.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3dafhzszp.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3jrqbuybm.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qzvwzwwy.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3dzkyxhfg.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3yuivfhjl.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3cxtjoscm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3stfvcfnp.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fbbekeiu.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zmdorpch.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3yljispzt.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3yncznzgh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3axnfyota.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ichgftgo.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3xxcwwidq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3qhczkilr.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3uyvctnha.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3qvzasdrk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3xncmhjnw.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3mdoiunjq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ekqsbxau.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3atwaapio.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3bsoinhhb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3rkglrpdm.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3xvnxtjjf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3jboqlghz.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3jzpkvlbn.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3hbdkmjaj.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3musmujwe.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3tmpfcizq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3rgaujvnt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3zxvsfmgl.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3cqdbzqdk.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3uxsccuyz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3telplgmp.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3uanjhkyn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3lvvdgtzk.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3njeerftc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3fmauwudy.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gxhebgxb.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ljndouem.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wfweliot.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3omlpowgn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3vgbpxsdy.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xkjbzfma.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gtttvfpu.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3zwkuzbjt.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3odguprvn.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zfxegwtz.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pqqcmgud.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lontvmlu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3bncvkdvi.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3glqeadei.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wgswulgm.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3apbvnbgq.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3sexrpywl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3wxdtjnfn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3etdberuw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3vpfaszam.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3wpygykxo.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3heeezaco.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3cnfkrxct.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3uzxjzyhp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3xktomwhc.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3gjecsocs.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3gtlxmond.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3keyphnag.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ajvwhevz.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xgslfrlr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3sijngfko.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3vmvkwwuq.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xdbzrcnr.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3lgqqvthk.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3tpsnjeuc.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3efsnvykz.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3omyvcrph.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3qusikpdf.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3mgrlouwu.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3qmtxvcxk.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3eeuutggb.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3deupyiuc.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3gdljyton.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3tlioxane.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ydambcwe.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lfdqbmph.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gyopchzz.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aghpqrya.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3mkgazgdw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dgheuhvs.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pkgtglhb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xfnnuuyi.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3wgwyllfp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3sczplkms.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kyvchixg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3wwvukppb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3nrzembfy.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3srxqkjdn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3zqxoqssj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3iofmzqrk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3qgkcjqwl.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3kgicubuh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3ubjfbxvp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3tpjbrxnz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3guswhqfg.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3idyfijbp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3ifstmqlh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3vzciordh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3bxzvtlky.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3btwnfhky.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nokktepw.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3sppfrgme.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zivkxuup.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3umtknhcc.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3bzrfneib.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3bogbdrwj.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3fcxdbyyo.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3usvkfcvv.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3zmtmtkqa.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3qsqxdesn.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3xsqrnqvy.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ztapultq.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3psxhcfxu.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3yikaznqh.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3rwfxglau.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3cvxpwtxm.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gchakonu.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3azlbdixr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3ptjkzktu.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3dzcwpunt.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3rbogzqoh.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3tpljubjx.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3jptiejnb.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ssuehzut.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3acifbdsi.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3heckcxuj.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3qypmmtdm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3lkjlciri.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3hugccsdd.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3pclyvavb.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3wcqmiuuw.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3nzmyzmet.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hkeakxdj.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ledywuwa.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3drktevxf.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3kgcgtboa.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3wgdfjvwg.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3dedmiqlz.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3mgjcyucb.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3prrosgwj.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3jacqxldt.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3fbmcqmxg.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pmqwiohb.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gnaqwfzm.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zvrfxuai.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3hbdvqtfa.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3knpvgkfr.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3byssrtvi.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3mwbaxfed.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3zovqevnm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3vibjnzin.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nmebxcsf.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3muiexgjp.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bmqfthxe.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3utygxxae.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3lowakqxq.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3cfjttwwq.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3wmoafxdf.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3lddivocc.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zwikayew.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3alcbeayz.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3uycwzlfe.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3kifuflja.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3gfolxvcr.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3bbbddgsh.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3imlbraju.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3mfmpmyed.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3qvljcahr.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3wdzpreyn.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3gwludnxp.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3fxewmkcb.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3mspskztg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3vdxyywni.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3dfvqqlzc.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3gesjqilo.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3gwkxbvnm.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3oozohcrb.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3osevjsqy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3rshnyqbs.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3efgquacf.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3hkbikqca.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3uesicnqx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3rzifvoly.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3hwckdvzq.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3fqtmpclh.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3ogdqmyvw.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3lnobguur.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3zhqgnsej.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3yobudjfb.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3bmhrlsgo.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3fkkrnkjv.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3owefqtjd.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3mhjkhyey.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3pkjutnmd.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3jewkpdlt.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3qjsepdgo.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xfhdvtos.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3bohsiawu.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sdiomrst.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3eabscpqb.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3xpywwglj.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3bczvzxgg.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3nxmkfhye.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3qkxfadam.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3njuybysz.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3lhmlmcsq.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3pqndouhy.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3wqejepws.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ebmmelnb.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3chrzapvl.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ygfqzeyt.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3geldmfaz.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3yokyroqb.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3yonihvja.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3tlgaazpa.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3onxazezp.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3gzwghkzv.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3aljggtyd.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3bihbetww.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3cbbpoyaw.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3ctlvflbn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3qgainnph.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3meoyutkf.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3qetcmldi.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3stissbrq.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3fpnyfkjs.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3mobhvjpf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3wnjiszev.html


<!-- 参考信息 -->