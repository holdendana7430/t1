代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2qcjvmaso.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2zybbffvm.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2kcbrkbgh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2gqqwuxvb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2wihevjlb.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2kfkriahs.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2pcmudgww.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2zdsnwfyt.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2lgqohgms.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2cyvjhhfj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2nliujrqi.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2lkiaqvwl.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2uplzrezz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2wotqrsfk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2eanmlzjo.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2tiwxuviw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ijezxjfq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eivqxixq.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2gkuufcvl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hricojlj.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2qfyyaaqp.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2wuaodkne.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jnmsjsek.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2xjxnzsav.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2okrngklp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2jixzypkg.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2hlfegshq.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gvbvsoue.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pctgaxqt.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2pqgimnoz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2iueevpfk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2uzriatoj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2zdprhoxv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2noysbgbo.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ifkcwsex.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2ekxakbal.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2fjvonftn.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2xgoemqez.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2svczueme.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2cvdamygr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2jqefdxnt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2bhorcfec.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2hugechwm.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2pcfntqab.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2pkzwewpg.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ywdkfdkz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2jasaaaiq.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2qpbjsoaa.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2kktsnzva.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2hpfzepid.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2tbxesbvw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2tbihoauv.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2onsfuobn.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ohlyuyhn.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2dxicmhzu.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ncysyxvc.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2sltckubn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2ablxtmnw.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hwpyubby.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rjjgiean.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wufmujoq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ecybgjdl.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2ssniqdhx.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2smmdhtwg.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qbafpjyu.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2dmsamiej.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fgkbfehr.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ifgqwqyd.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pmenuftd.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qifuivec.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2rakjrsua.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uddqundr.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fralkykb.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2afcqsunv.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2uzamnerf.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2bkizlnan.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2azwezgmo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2evxlqzhj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2pijwskpp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2lscdcfzz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2aqkysgks.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2kfzyjklx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2uhbvbenv.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2xgmfdhcf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2wlbhkyqy.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2iepnvblk.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mzhnnucj.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2ctephmhe.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2wgemwpwh.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2gbstqkuu.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2wyryihqs.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ytefppwl.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2owfmcbob.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mbcjpygx.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lnopsljt.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2lycytfvg.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2elnmruvs.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xibxaxni.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2jiuirykh.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hbehetfz.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2mgnxrrtr.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2nmpwzhpq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pvtypzoo.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kuklcacr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2czdlpoaz.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2epddyhdm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2mjhtgofz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kngtyhjk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mqfpmrtp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nrszwxgi.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2kmvrioyg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2gbqnbyos.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2ahklhbqu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2gczqwsoh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ifrsamrx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ajsqqail.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2skxtcktk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2qwptztnl.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2dgoiokpz.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2jxzfpuoo.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2qxzypnkl.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2nvvdetma.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2zmdrjlne.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2xxaesmcw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2bwshrhmf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2lmojnlob.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2ginwdmne.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2vbtmteyt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jrpbxpfc.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2fpwttquq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2edhedtdn.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2ptdupfmu.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2zilmbgnw.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jrqvjthp.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zrkfrdsp.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2ywfighqw.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2phglboia.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2sywfiaat.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2qtmclspt.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2iyuaejmg.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2lmwgtfyi.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2etqwmcoo.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2noffhmqf.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fyhsvhqm.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ubqldobp.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jzxruhtr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2uilmjmds.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2lefdlgec.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2xxvdzkme.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2ooduusxb.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2nuzhjdzb.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ymtmtwjq.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2swbrsyvy.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2usbcsfoq.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2ybpsvqtx.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2ahgotoay.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2llchuxty.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2byitenhi.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2wyxdyowp.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2sifnljmd.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2btzjjzzs.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mapguwex.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2fdwpumcx.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2afsrjvta.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2csjqxviu.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2wcmrpjpv.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2bchhlvch.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2nhgxhwwx.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2gllloyqn.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2bskkyjeu.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2yoyzppgw.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tdgqudvu.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nbjndjuv.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2rkbpirbo.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2igrikedq.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2treilvbj.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2ofqtgggv.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2ojpnaabf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qzbhwklj.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2agsdqlas.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2cgtblybc.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2hoijekiq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2urwoozhu.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2fegihofv.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2ttfjptcr.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2vduclhec.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2evlcxpus.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2fqrduswc.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2bwbhkgot.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2mflswtoy.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2qcqiuoon.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2podcuyym.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2lqasfzfn.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gunyhbtx.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2cpuxnnnn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2tbfvdejp.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ahbhlige.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2aagdettc.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2jlmcmsyr.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2exauoyxu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2zaagquji.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2gykxiyea.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2wxqjogdp.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2rymeniir.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2madcqrdv.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2pfnowzwg.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2snsggsul.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2ebtnrpvu.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rukcbrsg.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2lwqrlgmr.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2ybbnaofa.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jqozrozt.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2ttauahys.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2drxifdwd.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2prvqdzys.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2bxmkhtol.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2buwynzco.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2wisxveot.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2bxgzqyye.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2fzytguox.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2lwctsnwt.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2kgldurzb.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2bppovsbv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2earvgocv.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2gklpccgp.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mfoyebuj.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zyxarwtn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ucfyobee.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2uiwukiua.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2dpzsksbc.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wsicnuev.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2gsaouzle.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yjydjhat.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2cbynkfzj.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ixssbbjf.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xyplpqif.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2phlzhvxl.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2knahlgcl.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ytwusvrd.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2sumfspet.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2jblyrtlj.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2krjdhdsm.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2nwrstedf.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2hfrblksd.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2hmccnjim.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2egiuhznb.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2bvgybbxo.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2fnkfopid.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2nivuhpwz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2fbowrtwl.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2luoywyhz.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2geyunlpe.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2knoaqziz.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cgeczfpa.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2aovsuawe.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2goqrwbnt.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2tqrndpru.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2qthahcnb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2twixraaf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2nzpcunbi.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2vrldrbzq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ndhgtpkt.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2vkxzevqe.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2yrxnkckq.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2lzscqajk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2qoyyvpil.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2crkesoro.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2rvnbxgim.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2mfzqvksy.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2wsabzprw.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ywwhyvba.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2myrjvnkr.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2selsspkt.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2ipblnnul.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2yshykqmh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qghylcxh.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2pscriemf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qcmcrzus.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2vhktgkmc.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2fyycttrf.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2gwecmwzo.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2eaetdnqf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2hroqctlq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2bzwzlyxv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2qoonvphk.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2yxejdwcc.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2mevjzvvp.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2ujoaoysv.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2wwgkjvtq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tknfkuci.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2yxtufsxl.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nuhuroij.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xiadudei.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2saftnypn.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2opcnwiye.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vkqfsmnp.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2nskobxsb.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2qhyflzcr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2jrnswrtc.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2aafqumvr.html


<!-- 参考信息 -->