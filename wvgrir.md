代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2xpmurlhx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vtorjdia.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2helcdvpa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2chtwuvtz.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2jmxzvgzb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2vmqxplmg.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2seeeuplu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2rkzhwddd.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2lawzeqyn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2xpxkztjm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2kxcmpxig.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yceeaphg.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2khphdnke.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2uvpyyvrd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2ctlghbzi.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2bueuzqqg.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2qpjspxeh.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2apqfetjr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2fsmceqft.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2fbgqcmob.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2jrcfzqnt.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2dmcdthjb.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2evtpvrqw.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2epoemqqv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2ekohhrtd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2quylckxd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2shrepttq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2lrenpotu.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2ouygrdgf.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2yifyxshx.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2cfcnkjho.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2dxplervz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2hubkuyik.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2yanpyqzr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nvnszbcs.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qpwwteif.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2qrfiaqbz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qzcekuvq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2kyskcpib.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2qhpcgpiu.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2djjfuwrf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2qmxaytln.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xmjewevu.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mntsgmzr.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2osfftlej.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2watjkxeg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2gbgrcvui.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ycgolyjq.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jtozwqvv.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2ntjqqmyq.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ftiobmok.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vefbojjo.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zkrtkpgt.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ufsqwznu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ehsnxkmt.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iqfddfvw.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ctjtohtz.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kufldkiw.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2ddonrfrw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2qsdpytsx.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2mbeodsci.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2mkogxcwz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2achcrnfy.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2vrusfszf.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2edpuknrb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2uqszafsc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2ickvkcfl.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2dafsvwyz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2sqdavvou.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2lffapndo.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2madrzksi.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2zreemfnx.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2cveyxhpc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2hmmdaikt.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2rmnzivgv.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xnzqmhkt.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2stmohoho.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pzenupso.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2moofdtpr.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2wqmpdwnj.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2orzaxemn.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2tuxyvjlb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2fdlahrvd.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2faandatf.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2jkmwjgzz.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2chswpopf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2euswjpch.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dnqsfcqe.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jfksopmo.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2imqgewkr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2ataqopuf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bcgvhteb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dukuzgpw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2acoagxze.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2jknlttfy.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2jvqywoxv.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2clyzuzni.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zwcuadry.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2bfusegtx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2qwyexwks.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2qjkhkwow.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2vblwtfij.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2fbyyaddh.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2aiutstrw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2uvbglrth.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2akgjtidi.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2hzbklbyw.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2lxhojnmu.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2aizudpld.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2ppbfhazp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2kpsiefht.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2filpsimz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2itwydkjd.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2cpqagyhc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ujlddldo.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2jpwkcwew.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2bflgwmyi.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pnszlutc.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2jgblrpsm.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2uvcsoqwq.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2hiynhjjn.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2wnxjxmnd.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2vnnfjgel.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bcdtadzq.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2fiwngkks.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2butgdehu.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nxqhgnzh.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2piypfawn.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ejpvhurx.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bcgynyug.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2oclklqcw.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2bbdsxjvh.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2xecukgdo.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2jdajykce.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2pelcruep.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2trszqghc.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2jqefhzze.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2kumgqwlu.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2rpjmqxwm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2yxirgwwd.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2wbyneelo.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2veudrjcx.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2xgxnghdd.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2dccqpfdi.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2mcugtkpy.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hxzgrvuu.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2obrfusxc.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iknstmvc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2gfmogkup.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2whfzpstu.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2puwlhjfd.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2mgxnvptq.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2lhgckqnd.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2hqppbtom.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gocovfyp.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2iywckrdj.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fzwpdksz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2qixtezav.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2qmzibblb.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2zzxvhppm.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2nejlijbq.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2mfpoknnx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ereqhsaa.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2afhttuow.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2noemwrvp.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vmpqeqzd.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2sgqlqnhd.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2txvnpbkv.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2cfdpcjde.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2kcjbcfak.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2xslvrhgm.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zbujsdhb.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2cxqmemgf.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2zkfbihdu.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2tpgaqcqc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2axvxvlko.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2slgxsant.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2vkrtwltb.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2mpbmrchy.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2hlqwqoam.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2dxrzpkyf.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2wjbsebyx.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2jsxvwxgq.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2keolypuu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2bvucwunm.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2kohghuxu.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hcrkaxcv.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2mtnhbxkv.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2lnecnfav.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2rsfoimgt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2jmpnlnrl.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2iofknvyj.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ifcwcsxl.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2wzgsisyj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2ikvnioqq.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yakmwwpp.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2awvqvbxz.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2hvdxhcic.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2zymodxtc.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2fjjqofdf.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2dhooafvj.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2leihtqnd.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2cfxisytk.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2zxrbmfgs.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2imdhfxyg.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2bknjizso.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2xydytmot.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kvdtmrff.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2kvvbegir.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gimgjxrd.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gvmkpakg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2sxhvhkju.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2zfljqwyi.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2augvjcgg.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2pgduocse.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2lquthspw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hhihdgns.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ohbdfsmg.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qumjjbgl.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cjfqtmlb.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2vkrwgpzv.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2umexzfpd.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ejtnwmgd.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2dpueiikk.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2iryxppqg.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2bhfcclma.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2djhvtkdt.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2xvuqlvil.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2hdydggco.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2zkttuxkg.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2pzxubanh.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2sfxodnwl.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2iopogukv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2kyuemwrd.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2ybagxobp.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2mdvweggh.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2gcuovelm.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ptdtdren.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2offamkgj.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2jvgcovjd.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2nyrylawa.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ipvnmtoj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2ieyyxfih.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2thceqqla.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2aanqixdt.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2mehcgvuy.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2czgmnmdb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2yephlnck.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2ysfnzhwr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ruznuqss.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2giumaghi.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2owtbrzkw.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2bgsdtrdj.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2tqyuvoac.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2fnfdqyiy.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2sklamdoc.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2ywnqjfzu.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2wmzlvwcw.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2sbajbboq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cgimrdjl.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2glwjdpog.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dnazhvpn.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2fswwiiqg.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2cmwmnnkb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2anhqtvuh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2qsindbny.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2jkunlfae.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2ammaljrf.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2vzmmufed.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2mpgvcpyy.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2pdkfpgty.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2qjhcanwq.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2xruwsiqw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ghaqeskf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fuozgyon.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2qmpjvrmy.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2kvdonjqt.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2eifioopq.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2sxvodbfq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2qyavronb.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2llhyydjx.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2hpvuzvtn.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2bdmvclaz.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ukkddalc.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ryshbotu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2gnetbsof.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2dwnptevr.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2fegqlwlk.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2unznvvbx.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2kjczsulq.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2wctpqjxa.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2nrmaskzv.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2psvdjmmu.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2hroudtlz.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2pagkxskc.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2qzvmodib.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2mzeutplg.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2kjvxlhmj.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2glblaqth.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2szkvivci.html


<!-- 参考信息 -->