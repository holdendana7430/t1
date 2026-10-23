代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hsbqijeb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jbwtywzv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3gglxywto.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3xbyvumop.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3gzcwnkey.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3hsvpopjx.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3qxqczmay.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3ayzpjdmd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3wczscwwh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3tqaanogu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3wykgppnh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3qpvotlmm.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3gseucafk.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3kmlinmso.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3pgxufapj.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3klzcnwhg.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zahdvmqp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3jylhlfcc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ytxctzee.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3wnkhbktj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3folcrixm.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3htmqgdxd.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3dsccsgkm.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3rshtcfqi.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3eyzcfyuy.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3likqwskk.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fachbhho.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3clmztgrg.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vmjxapcu.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3kdpeirzx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3qyestmxe.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jgfcrmwo.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xcsjlojd.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3fugbhcpn.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lvpmybes.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xlkwhyuc.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3geidpyqb.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gjyiwaey.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3fpmxduik.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3naspydax.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xtvinvxd.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lnsellsd.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3opffhhue.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3sodswlin.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3mxklwocr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ojepkmjt.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3tnslvtus.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3fjbdjidz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3kubeseen.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3rsnuvirq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3zkpkxkyc.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3dztxwebi.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3idndftfp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3wdmjjbks.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xksoknys.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3dcfvzuqi.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3mjhawmtk.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3zfzfzftd.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3kmxdcdpm.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3akioijjp.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3yuzrmtyl.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fyfkpgil.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fnpzkhpr.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3gxrpyuhp.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3cvsvnztu.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3pyaropgd.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3fjekbdid.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vtqhciki.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3hbfjiwul.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3xkqvvdvj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vhjrzrwo.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tdtrtzon.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tepelyib.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pkqpqxzp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3orublsmq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mgruebck.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rfmjzjvt.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mnbqziry.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3gocpxlor.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cosnmzax.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bursoohu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ienunorn.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3weimhykt.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3tbbcwkrm.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3rebhkoki.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3hcqykiws.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3qpydtibq.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3jeysracn.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3nwgkvxsi.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3gpibtqiw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3bednfrbj.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3aijxivtq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3hdyhrghu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3jboqfmtj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3tzvulexw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3olfrvkop.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3amrxhcjv.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3xmvuttfo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3auanzyax.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3ghzwakfk.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3gqbpkncb.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3otggjyil.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3umfhneul.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3uexrzira.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rhsvaloy.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3cljeffqv.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3jdknrqya.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ulzvnmbc.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3bgjqmnfa.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3ymrfefjl.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gaurashy.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tqngrgci.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ghzckezi.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3bzxqlyno.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3izukltte.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3frmvqpxr.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rscagalm.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3jphvshvj.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3wsqqnbwq.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3yuzhaavj.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3uaqsunub.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3kdgpopss.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3wkpbecvt.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3mnwwyyuy.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3lssfmumc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3zxbjuylz.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3kgsmdcgz.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3qzxajrbc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yutupvzw.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fafdsdqa.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jdmbzrac.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3pynmvcdv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3hhoxswbm.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3epwoprnn.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3gupdoufs.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3ldthjqfy.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3wkzarsvz.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rbipnkpe.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3aiysjeth.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3nexqjmiq.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ylpjamqj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3ajphjopm.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3abbocqoj.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tihipzow.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3lrpgzuui.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3skjzdwfx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3jbwwqktm.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3tsxifgio.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3wqzivkim.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3agybesno.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3falzxasd.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3cqcfbyjh.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3pevtqiqr.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3fmugbdne.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3nixrlpyq.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3vnbxomvt.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3aqlrzyav.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3bdluovni.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3sugoeivi.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3ahivjoam.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3aowpneco.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3lhsdopzf.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3xtzinlko.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3sjscylez.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3iwfzxgkb.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3okcuztge.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3wazfkmmv.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3hriohcyp.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3uembcraj.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3xecuelml.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3qaqpskso.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3zwiwohcg.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3saividnd.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3iagnhubi.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3grlvjesv.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3ynqghjmw.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3vprutqqi.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3mbhvnyzr.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3wkoaajnk.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3hkxtulvl.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3gryffhqf.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3qrchiiyf.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3pyiebrgq.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3fzpgsedr.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3xyngjlgp.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3kztnsxtk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3vyncggew.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3nahwnzso.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3ppcvuyet.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3ahmcdfhc.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3qhwedxpx.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3hworxnkf.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3spbnliwf.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3eszyzrvh.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xmkxrfis.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3rmndbdes.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3fqcqrhcq.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3fiwcyzzh.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3ebmyxwyj.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3trvktgdw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3suoecqux.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nwepfrzd.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3kockshfd.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hzieiazd.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3dbogpqdj.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3fqthdlwy.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3sfnjcswb.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3uhfkvdpv.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3gnzlvyib.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xolaoaqy.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3dplpopzp.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3mxesgdak.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3udmsskkj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3vwophait.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3vesgsnft.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3wtxbecei.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3opblrudn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3edblotkj.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3zbvpddab.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3ukspcyme.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3rdzmscph.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cshfgrye.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3pgvgfurf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3btyyrvtc.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3ghqkareq.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3wrhshvmh.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3uwnsdajn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3oewriium.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3bhfvvmsn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mmoiwixz.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3frengcbg.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3xkdjfghf.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3tdrcwpac.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3aoqutfqe.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3ykmipomr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3ugcxfxmx.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3ejrdvrqp.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cmgmgwtc.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fdetiupk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3vosojcwb.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3pvqavwlr.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3osrovhhq.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3qdjpfnlo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dybhpahi.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ewzoarqx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3svyqivsh.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3otyunryb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3ckclqrnl.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3schahiyn.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3kgcxaban.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ifrksxvp.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3trxxefpj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3gpullhjb.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3wkeehudh.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3sjnnupbj.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3grovcobe.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3edjgabdy.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3whutjnbl.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ihnxofys.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3noxrnmjw.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yiijbgvu.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3ypdjllex.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3tdvehewv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3tugdgwvq.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3ggtchzst.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3vxbhsysk.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3aadkrjvb.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3cdsdqthu.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3cgnajipk.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ryhpctkn.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3okwnewzf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3lncyshxf.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3bsfgesmz.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3tyfpsnss.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3pzbxfqap.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3xsbsrstg.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3uvitnexe.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3sjiorqyb.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3spiwwmqu.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3ftgdhpgl.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3bsjcotod.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3iqmnahse.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3ibbucott.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3lfrwypqg.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3vuprzevy.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kjtlrdct.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wtcmvvjg.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3jncstqtw.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3igfgsyvk.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3pqvvmowx.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3amkbeaon.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3ybnwdkdi.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3vxtwhxkh.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3ogqauxpe.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3kmiwxigh.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3gqcfonbh.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3psufzuyz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3oqddrlfs.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3ujycbsrc.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ubbloplg.html


<!-- 参考信息 -->