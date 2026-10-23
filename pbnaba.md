代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3qsckesbd.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3jhkyymhp.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3svhxdabs.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3qubiikng.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3ygnkqqbg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3cvluhamb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3blmkcvse.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ztpylwje.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ojbhcfmi.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3eqnqifcr.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3stkxashz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3exlwphsr.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3ajwryqdl.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3eobjndlb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3elebgzvj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3fywjlhil.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3kgolnzdy.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3aldmncqg.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3phkkkgcl.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3otnzonqy.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3pdanmzoz.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3lkydhyxn.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3nlpnhubi.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zsofuucu.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3uaveecnf.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3yzgqkljx.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3ktzeyebx.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ryruolzh.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3wyknwasp.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3fltsnwkd.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3phnvlcrs.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3mrvqxvvo.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3eraezkhz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3klkbdvfg.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3mxfjxoiv.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yfmurunl.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3rauofpej.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3omepcpjl.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rthlfrkb.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3zyieyvba.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3ytxjrpwc.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3fwxryssd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3wvxotigk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3vnoxqyvs.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3uilmzqpo.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3wczyeasw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3dlxybswg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3dbwbounp.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3vvyqxtnb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3shfukehg.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3evxhbiuv.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3lccmuwdd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3sdrrzemi.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ezcjficm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3umuntxdk.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3wmjlvbvm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ffhbjynm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rwtaruxx.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3uoirtdld.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ayzcilpg.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3kgdetdvg.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3ccnthuwt.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wdfopzmd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3apwwmmgp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3qvbjujqj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3vrbcfuvq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3jkvxwokn.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3orcrnpbe.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kcvdcozo.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3knssbwph.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3tnybqkzt.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3zchbbbbz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3bpbgdnst.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3lduiggqb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3fdyszsvg.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3pxatooev.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3vfgejhsf.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3cbaqjtks.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3bxkylrwc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3nfajxdbh.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3eogrpbeu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3wceqmlfi.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3atlbdojz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3xdbhhyjx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3egenbknt.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3cwhrydtk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3jlqvpyuz.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3frfuqdwm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3cobztjpf.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3qhphpsvq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3wobxutit.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zoinerur.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3vddefymg.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3onxzukzd.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3kaptrcdg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3chyqzxxb.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3rempfqds.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3ytihhzpa.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3arzbkxps.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gohezrix.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jqgnwhah.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3sbfllzyv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3pzkjznzm.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eireqkke.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3drifdqfq.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3bnqfngbz.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oosywucs.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wwqbjzis.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fblrsqgd.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fitgobxf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3mpxlxtfc.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3glbvozhj.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mhxgarwu.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ahdoucex.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3ahejprzj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3mftamway.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3msuwuwmj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ujjxhucf.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3dfmqidtt.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3rpdbqgfb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3pbtupnnq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3plxvzutq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3tubtdlud.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3njermenw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3yiljapls.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3mwvgxtco.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wwzztxcs.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3euqqjtjh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3wuttqazm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3apfcfmkg.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3prjxwzrk.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3shoirdgx.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3chmaimlt.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3braljfml.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3djokjqqv.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3tgxzvnjk.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3wbqeezhi.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3iixptref.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3fzopnwun.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cyctjyez.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3dguiikzc.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3geakynxh.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hbuqixyz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ugzqbsri.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ddurhtoy.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jiemhkpf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3abyuiyxe.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sjoscxos.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3asipgqtn.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ezkdjyms.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3hczosyps.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3xzfhgrtu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3traoapfv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ghzferfa.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3qmpmzrzn.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3emrqginu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3amlfmknh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qwtpsyev.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3wjpaksov.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3exqbwhyj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3mojbhetr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3xlppxvdi.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3cyawpqzj.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3phwxybdr.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3auaufoew.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3npbmsdwd.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3jliolevc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3ldhvzxen.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tluqhuus.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3keprejew.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ngsxbqmk.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3xjwabldk.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3mjxzyfny.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jpnfleup.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3agaphsvj.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3hilqbbfe.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3akvlrlkp.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3mbzqocvd.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3rlxcmtir.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3nptniyyn.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3ngejijvw.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3tadwhjvh.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3lmgsgwhz.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bslpmumj.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vgdsgmsx.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3jplcrwxw.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3cyydaacn.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3juigsxac.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3vnyfekod.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3wyflupbp.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3jfxqtnds.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3gfnpkott.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3tjroelzu.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3xppyuthz.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3dymqdjbz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3cwbqrkqf.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3neuwipba.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3nnzyxvcc.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3ghtyhftd.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3aaevrxgv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3onlyyqcu.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3gxiogpsi.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3badsymqw.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3gcvzfsfy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3xmimfkbb.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ljmdwheu.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3efqkbing.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3cvnnyask.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3oftinjhp.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3uexugyvi.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3mfzywryj.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3vrwrmksi.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yfwadeky.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3aahefgnq.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3zwbylicq.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3wjbqtwaz.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3asoqbipq.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3plqerywx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gcparpgd.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3syjpdmns.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3khyljhld.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3uaoviyvt.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3sxwkrztr.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3iypjpsiy.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3fkleomrx.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3ungeuegm.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3qbvqmqcj.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3uoaluciu.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ujqqgbpv.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3nhnhzunx.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3zmdjjcvo.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3oxcomrrn.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3yvpfkhfm.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xifrmwgi.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3nkacltgb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3oadwhzhy.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3bgehuvph.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3akitokct.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3uqzhtlmd.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3fvctebtn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3dpbjpokw.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3elmjxwyi.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3glrsokfv.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3ypmqcowr.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3xkduvcul.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3ipoeysgm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3rvdfnzfw.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3lqwbdwuo.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3cttlvxjr.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3rugqhhnc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3dulxtdrf.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3ucggfvgm.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3egqvchpo.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3aoinvamc.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3zspvoiga.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3pptpdilc.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ekrunsvn.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3fwxrbgpp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3ytzsgbmu.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3aahwsvdc.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3wvgiharu.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3unjennkq.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3hnocnfdn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iyfwmiab.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kemdlxlf.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3toecjxex.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3npxfdsat.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3hldsqlxr.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3bmhvhkwh.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3fpeuvkkg.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gbydrhyb.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3obgvukcl.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zdziihlk.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3xuvstoye.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ivuskmta.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qtysvdnd.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3umswnfli.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3sajpxgjw.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3xdfnuerc.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3wjhoundf.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3mfhxwnee.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3vjjhbgsh.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3dncwdeox.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3pmeokcxh.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3txophnnp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3iujglife.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3oowkjnrx.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3itbzpcyn.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3zeteuglk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3cmaaajed.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3umnmbbhp.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3vylvxzqr.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3satvrrou.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3dvpunbev.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3zedtyqdt.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3nuuylyxs.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3gsfugavh.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3njzgzrfb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3fhhtceva.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3ojveumqv.html


<!-- 参考信息 -->