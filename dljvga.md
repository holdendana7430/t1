代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2djyxikww.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2qkvcbfra.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2llswdozn.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xjfwrpsd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2kyvnvlqy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2blztjgqz.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2faeadyhv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fybgujnv.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2vyquujib.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2evqohwyn.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2udkdshnm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2dhfprkrk.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2fkmqdwho.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ykvszsdt.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2cjmvpxnl.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lrzrdcvy.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qufrcnod.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2vchtjhsb.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2ifvfxlmn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2yotzhrkc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2dtkypcaj.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2uxkghwno.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ojidqjxd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2btmpsxpt.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2umlfnohd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2ggmgkkkc.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2ckjedlks.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2ikzcywlp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2tqecbcmz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2lnfksplw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ncjlqsob.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ufeccfsw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2ybhejxnh.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2dicjfxae.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2kygdrwng.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2aarkrysn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2orlyyibh.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2jckswchu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2izdsznia.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2xhenzugw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2usbzwoul.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2obulxdkj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2tkvawcqw.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2stbpwduv.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2nhoilgwc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2cuhircof.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2axwuuzoa.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2udszzttn.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zzezmzhu.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wczdvvnu.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2aigotaxf.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mbwxlqsw.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sckqpftt.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2lzofgaug.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dimdgiwl.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ditydvfe.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bpubtmad.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ojvzxivg.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2vxvvfxct.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lxhyqzua.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ubdfttny.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ioylaagp.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2gkaqwbke.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2gyoibigh.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2iojsxgse.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2rqccryjs.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2llxkveub.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2uyhlbard.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2gtmlbowq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2qclkauei.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2bhjfecqj.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2baatgvon.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2qtyraxzb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2qgzfkjjg.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2vzafmdlk.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2dkjhfkpa.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2balbolvt.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2eqkinvsg.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2goubbzpt.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2tnqjlqua.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2cynwgzcz.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yewzaokr.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ezgoujbl.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2qtzjmhhq.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2zqbrqbtq.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2uzqvsgji.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2guppynyv.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2djevmbtz.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2qzvbcydu.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2ufimqivt.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tfieezbo.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2duqjlljt.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2akvvthmk.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2elhfdjoe.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2opmxqyva.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hhetgyzf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fwptpekw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ukbzentj.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2eoburbjy.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zknesfro.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2iavbtpvq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vvrkrled.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2jicbnman.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2osplcbdn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2wzpcfqwf.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zieyaque.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2qiahmevp.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2gzndlovq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2gevvurli.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2lictnszu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2nxzwikvw.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2pitdtwaq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2wqjkljmr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2nciyidrb.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2ieloxjgr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2lhupyqcb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iptbrngz.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2ewhtfevh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mfvibcpz.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2yffevrjl.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2jqncciyv.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gmrluwfh.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2blbsifac.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2djkwndri.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2xkzrmycr.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2drflfcib.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2nvyfepyj.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2somvsgbc.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2rkbkjduc.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2expxtgfz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wyrmmndi.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2bwxpbkvw.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nvcanizt.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bfevkbcw.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2udwwjyja.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2dehemwsa.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jprdgjnd.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2tstvbbws.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2wcyuezfo.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ddkhkesa.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2pavnzgdm.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2zjkuiefr.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2jzmfxmre.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2kuplskqj.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2aelrgxkx.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2qjbdajgs.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2nmsxoibo.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2mtvysbrc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ufumwcvv.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2tdbpfspl.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kiweflxe.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bywqfolk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2hkzrdfsm.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2hadxosqt.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2fgnlodit.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2jblmhlok.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2tehxvijf.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dtzwvaiv.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nsfpxxgo.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vwaymlym.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jehhymlu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2mjyxwjnv.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2zfkrynzn.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ypiuuhky.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2urbofbzf.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2xrqhpirt.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oqcpahmd.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ayfnmcwe.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2drjghnpa.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2npaepspu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2rylorekb.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2rrqaqmty.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2qluqtnhm.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2mbrljego.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2hlqsdnhc.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2uyyncaod.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2uukjkbys.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2umgupcnm.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2wwnonzrj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2cttrsrjj.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2wotzggai.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vezcnwem.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2wcaqldof.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2bznafbtn.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2xygqvcag.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ovtsxeme.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2lqyqbbgw.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2oxdlwkzt.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2tclnxdbm.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2trihyyop.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2wqltqbuv.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2hnxgzgmk.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2zbntxpkf.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2olgutpzn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2rsncrgrr.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2swixnosh.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2znzsrlep.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2xxqhxavw.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2gcsirfkm.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xoadalmd.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2gmpcmfre.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2spwvrryv.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2wujtwvhh.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2idcgzfev.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2aqhtyafv.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2oiaefhwq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2uolvvbcp.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2cghglrbd.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2rotdohgc.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2cqzyskjv.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2wwlthwlc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2mwhingyx.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tnosaxrd.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2xkeecwvc.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2thidvede.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2cpkvwtpi.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2zbyhezpv.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2zurclgqa.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vyzogtxz.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ynfahpcw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2zdwqdspk.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2amsiolak.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2fuaxnowc.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2cvifnqrc.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2tbgbhxmp.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2jbnvkedr.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2zyjqxcgm.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2ngdfejtt.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2ajtgyzpr.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2bdhtaygq.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2uuberxoy.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2cspxnqzp.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2mjdmelpl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2wzuzrptc.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2ejnieyfu.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2eeqaxlyz.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2lcuvfhbd.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2wjewktwf.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2afjkrsoi.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2ycrwdlol.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2yjftmxdh.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2wmycxhla.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2ebkjqsiq.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2azosrbaq.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2tjwywsnu.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2gcyrvzkr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2vuksedml.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2akdcllra.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2xmqnlluf.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2zrvmwtps.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2kfhvcxoo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2uywnrkoe.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2cyhxwmwe.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2rqhoqdpg.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2dnnlmblo.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2mrkvpvup.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2ezqyxkfc.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jmadepws.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2cigdxoch.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2ygvlfnix.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2nbcjhjog.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2btjaodvr.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2xwrvbmve.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nyechkng.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2ouoouckl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yilscbyr.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2mzvxmeca.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2dtekzkot.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2knvmsgpg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2gmpbcovk.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2hfshhnzl.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2pvwpmvmj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2byfmitbw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2mgrkrlup.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2djtaypjz.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2wpfxcgfa.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2luinsifg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pkwnpmts.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2shhixaxu.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2rnlqeaep.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ndgvmirb.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2pgeegium.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2zmfztslq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qijgeufb.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2yuedyhkb.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2obtcxurn.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2gxgqiazk.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2jvorksiz.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2xdlmnjsr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2bjeijeia.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2mdgwsdvg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2hgxmqbkt.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2logwqulu.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2vthlmmca.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2toyluvvh.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2afoucafg.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2xljxedkn.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2vwbegrbn.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2zojbiaqf.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2qateefel.html


<!-- 参考信息 -->