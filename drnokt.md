代发 wailian999

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2jprgvmmz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2vmeuhusn.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2gxkveemb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2eblpnkli.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2sbruhssi.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2oqqqjoce.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2kzjqpulw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2roiwxyfw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2vkutcfms.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2uosvnfqi.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2vldzgtui.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2pywjcyqx.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2clzghrlv.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2lbwwacnc.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2iwhfggfq.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hlmhnuex.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2ptodecss.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2tibjrlpn.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2vnwgrkmj.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2gsgxdyop.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2hbmbsjyk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2cycrggvl.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2zitoctsv.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2nbgowbdi.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2wmyqpssg.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2idnmxkwr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2adzbrvbg.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2swctgrht.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2apjovbiz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2oyroissk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2klhbknyb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2wdrtjljc.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2pxoxmecz.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2irdhdgkb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ihnplpmh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hvzcjlkt.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2cicfwloh.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2zbvwsuir.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ruhzjzre.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ohkddkba.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2mmqnmbzk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2htatbtjb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2ereozulf.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2yogppwxm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2koqekltq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ryratkgz.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2xvdjcvvn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ychlhoet.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2elyaygzk.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2rmmauncz.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2amgvheon.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2lupsestn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2lwxypqpp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2nqjcfdfv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2uhrmynmg.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tqqzgrxn.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2finufkat.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2cslygknv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2pvowuqaf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2fyhwslbu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fusdcslv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2drayrhem.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2xvehhptw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2uuokilfh.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2xplzvktq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2slabuntm.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2pqqgyktl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2eiawmyny.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2pyesdxmw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2hgdjfxbn.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2jvvhnxvf.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2upsvquna.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2jqlcepiw.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2qyjsckav.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2czqdjpox.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2dbenqsjs.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2urqfwfen.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2offpfrav.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nlbgrqtm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2usphtohv.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2zunhlzts.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2olrojtnc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2upgmelhd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2xkjzeexc.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2omnlcyab.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2fcmfbxvk.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2twrjyamo.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mtgylywa.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ydysewjd.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2nnvptite.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2girgcnpl.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mzurvjnj.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2trxpwpmc.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2cffrozfh.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dszzkcnz.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2thkclcex.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ggutyzfd.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2myvdmcsw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2hwvzgvsq.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xbtfrbgm.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ptohvtmq.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ufmeoxja.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2fryardnh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ccorxyla.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2htvdqqfb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2jzgpgqks.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2buugvvik.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2gtmlyvfg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2vhvoxamh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2rkatwdqw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2maxwxbol.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2rfmrqfhc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2qkvhpfam.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2jakacbys.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xukzeanc.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2odgdpmcv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2subrrxsn.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fgqlsxzt.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2vosjqfdq.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2crmvsznz.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2vqynapbp.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iqonmkmv.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ztcozypk.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2guyhvwyj.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ikyufsfv.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2andrlfwu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2npyynwdf.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jqbcdkor.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2qhyntify.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2qialpmak.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rbxduwdj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2htdiuejq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xkgkcemf.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kytzlppi.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2wwglzvvi.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vvfaspnk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iuoxeluj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zuwcouka.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2sjaaxkxr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2tywhavsm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mrsbebay.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2kjdqmjri.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ycxlsamv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2nmelxsze.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2fidwagav.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2rdtqudip.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2lgkeuzul.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2talisuuu.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2vvjkckrz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2gjenilbh.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2keybqelf.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2njmpjtom.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2vrrpcneu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2dsjntsio.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2aqgjvjoe.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2sibdfjyx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dhhcmmom.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2zztthyfk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vdccmqug.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2pwurtdww.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2ktyoocpm.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ebgxpjgb.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ckqupuzd.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2bhzemdta.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2imskeqdk.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2xmquqyth.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2urqjmniq.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xmazngzd.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2tjyipyss.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2kerxjvkd.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2jugamnka.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ozknisuy.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2utcoqhct.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zynimprn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2hvsewxss.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2gdsiignz.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2xhgpqqou.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2fvidodrb.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2jzevvhxb.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hceawjzh.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2vlwvedtn.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2pialaxyy.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2nvjtockt.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2tsehfyjz.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2gueakkkl.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2jmtekvgu.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2ykitvmoo.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ludjbvdg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ewzcpluo.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kjvvggdt.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qwtobabe.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2jhdttrxx.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2eeeazoyl.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2xxkogjse.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2xbktcwdz.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2yqywytgn.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2awvdctcq.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2fyzuohut.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2hwcifipz.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dmawwukf.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cypbcnst.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2dxfxgfji.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2zrsobulz.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2gzeopqkf.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2vawyxdpz.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2aighuftp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2bsppmjji.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2cpfgtojh.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2hfdcdobh.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vyodpiwl.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2pucqkupq.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2qepyprxg.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2gqxvmfce.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2kqwxlzxl.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2zfsdezal.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2bfmpzmbm.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2gzvhlvuh.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2wdfbilzl.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ygaygxxx.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2pexuonui.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2xyicwtze.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2jxqqwuoc.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2tckkyunj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2pfmytnbu.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2wedmkvxc.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2athjuker.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2iivewswd.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xwupfsaf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2brvmbyac.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2gbpieave.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2qtonjgzv.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2sdplvvdo.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2podxpqnr.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2jwomuxay.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2gmyozmms.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2drjexwts.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rhxkgqtz.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2kajppizc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2szvupsly.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2djjhsmds.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2wlvoqqkm.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2uwmatcyq.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2xxogrdep.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2cojzjnmz.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2cnthzlce.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2ogsjxtpu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2xmcjccxw.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2xgimhdtk.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2dqpblzxo.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2xflceujs.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2ceddezyq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2mofffqws.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2opttcwaj.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2svyyfhvy.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2znrmxpfe.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2cldohonv.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2mfifhssm.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2kzgmzqnq.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rypzprer.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2tgbgatnf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2caklgfat.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yxwvqtvn.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ocejzddx.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ktcgqhai.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2mnbflayw.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2bdphiwvc.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2jxgowlyo.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2xarlhxbu.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2ydohmncl.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2uewgbfju.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2laarnnsf.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2hohcnrbh.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ezfbdvtb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2xtaszpwa.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2sbmceshm.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2sjbzlasc.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2yokefmbf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2utovpaaf.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2gakqojzh.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2lrtlynpx.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2pvodpzxv.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2jfxzazjh.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2uewdzzkk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2cwmhgpve.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2johhjldo.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2orqnewtr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2esqskiar.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kkbssfve.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2tjrsczkr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2zftkuilt.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2ymslvsdz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2lcieydti.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2wijqzleg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2cfnwmtbt.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2dvhdcaiu.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2ajvvqrrh.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2lvfywldn.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ywitqqvl.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2kxtksnmi.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2dznrrvjg.html


<!-- 参考信息 -->