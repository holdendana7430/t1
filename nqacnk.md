代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ribybzcr.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3vysxryqf.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3giwmktpx.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3oifoxjan.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3qkxbszfd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3snabjsbe.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3bktxpbhi.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3bchuycaf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3fesxynhq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3chjdmorn.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3nnojciec.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3lhnrrcua.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3frfhkwdv.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3reyaqnqw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3kssdmydt.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3pmsvychc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3sesbvlgm.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3vwdpaebn.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3vmcvwafo.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3inrjggeq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3huemkkkz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3jwrolnyl.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3sdzgyhgh.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3aoroixhv.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3zowkpgyp.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3eusarmjw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3ixtapeoj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3honltcqn.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ucnrtglh.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3aofzrnnn.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cvzvtbqp.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ouoekwbf.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ztuqsigt.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3detiyqdy.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3zzimscxt.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fiqdmbdg.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ahsmqszy.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3pozgtums.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ottalhre.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lvbhehkl.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3neckwixd.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dabkrefa.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3mdcknhwh.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3okfkjudr.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uhoiazej.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vzdgtohd.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3pjuassru.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3swrabzil.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3kjaeeqey.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ozjkkfce.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3nontahai.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3tijepshp.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3hckhggun.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3dmuizvjn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3wsaabfbf.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3edcuythh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3cifyebnj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3jepbuali.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3sirqjoky.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ahnknigl.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3kglaiaxm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3haiuccgj.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3vnuwtstw.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3vfqlznga.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3rainhcvt.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hdrbhyye.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hgnkzkzb.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3gzeuzkiu.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3akrfuepb.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3rdjyzhca.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3fdfbzxbu.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ybrhbyhc.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3wxorzoip.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3slbnxvsv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3koogxooh.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3aeersxnn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3insikwvv.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3llpwalzl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3kvttozpu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rcunrwlz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ldwhjgtf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ijwdeslt.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3mzilpptk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hsxdhrly.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tmqdqogi.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3jfgkrwjg.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3gozhhern.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3wxrlrorx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3gjbhjomw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fhdvbegf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3juuzgvij.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3beprnfdl.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3eroumuiv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3lwcstohe.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3myiwalzh.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3jwrtrtnn.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3lasnfski.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3qiaoizyg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3bndkoaod.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3zubindpd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nalnkkps.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3qaayvpqg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3slqfoibo.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3whhkclrl.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3ffybwiyo.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3vyqlckat.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3sqdgygoo.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3dbdmapdl.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3uxfohfal.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3alzjwcez.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3qjnqabzk.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3hghpvzla.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ehckbnmo.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3litnpwnt.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hpmogjbm.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kawjyojb.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fhpenztp.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3popyaycc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3jfgeyzox.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3zkbfoezd.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cwybepcw.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3lbzlqets.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3exjvawgw.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3krhaxbkb.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3dijsztqt.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3vfmkvbsp.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3zskyjfnv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3opesncgt.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3awklspix.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3fvqgjwof.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3grqgjtgk.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3lvikplhn.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3klavubmk.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gkiptvph.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zxteeons.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3gmgwkuwf.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3qtsxgbwd.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ypjgorjf.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3uopgohac.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3iwtfhzfc.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3iczhmbii.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hymgzyrw.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3opstwlzj.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bkmexsly.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3eowapowa.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3eclfzsml.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3lawbzgzg.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3dvaouesw.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3nakaevpo.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3kydbzkiu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3quntjjmt.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ohuonbyh.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3opjonung.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xmdscsup.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3lftvfrdu.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3lpoxcalu.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3ljdkqmqb.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3oxdjbjor.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3bxljckvj.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3dpwzkuqq.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3vtcbhnfm.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3voumfezk.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ckxfqxjx.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3erygecvr.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3rjbpqyhi.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3nnwzsdcl.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3njsbuiwv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3exoupfcc.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3kjzhdugw.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3kqppeaji.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3jualgxsy.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3hbsfuxsm.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3oeqmrsyb.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3aukovoyf.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3kimskbdu.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3vkgpvnbp.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3nsqllzke.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3kqkuysop.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3pmzhpsnv.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3aowwgopt.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3pttsdjdf.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3rkrnzjbq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3ahbdcfgr.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3ydisjeia.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3zdqcrzdp.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3zvakoaic.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3oekxvpal.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3hogjbshu.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3gquxpjvr.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3hzbicjzy.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3mtuqnvry.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3xtjcpgin.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3glnohfsm.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3xvxzjfuu.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3bhwfgxyi.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3vedrqrlc.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3hqxwfkpw.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ierikwso.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3kazfmjzu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3drouauaw.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3ksmqvnxg.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3ydxqwpmo.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zkdixqeq.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3uvfnnkkr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3owrrtjlm.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jjjcymvq.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nrkjikco.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3iaitsaxu.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3zrnopzbl.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3avegepjt.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ryyftggg.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3xyeovgxp.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3qprhktsa.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3hiiycqab.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3jgyarkxh.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xcywsvps.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3egixercl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3vlxxetbo.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3vviodwhe.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3ygqtjvra.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3jecppxja.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3ihkwhelk.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3ligxlzkb.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3ratlleph.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3zqtbkazg.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dtyiiueg.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3aengdmaw.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3gxfdlznl.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3qkmieedh.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3llkuzzyl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3advamxej.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3tjgnumiz.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3uztsiqoo.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3vgwkwswv.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3fhjfpyfz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3dheahkxg.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3ynnxrrrd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3fzlgfqpy.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3bploobnl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3juazlxtt.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3ujeuckzd.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3rwyhkani.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3fabezjmk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3ntmjirol.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3irtujbyb.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3pkuwnntd.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3lgmomvdu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vpbyctlr.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3giowklew.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lnempfpo.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3mcopylrq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3tkkrotzd.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3akfaxblc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3yxyhraof.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3peiugfkx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3idgnxgud.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3bvrbvgjb.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3mbakeyli.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3nsqshkfv.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3dfktdhaq.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3xmssstrf.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zkbfgcak.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3nztafoqc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3qdoxpqxe.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ongpevfn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3xcbybmfa.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3higxcnfh.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3twpvrjkf.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3shvjvbfu.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3nthdbalp.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3hgihlylq.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ayxpbffc.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3teuzfajb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3rcrplsxb.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3ulhgmdrl.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3cdchaxuv.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3nkkcalgw.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3ugkyumak.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3wbhnddqo.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3ltpntjfo.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3okcgaatq.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3zqoqniue.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3soazscet.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3cqrzvlzn.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3zkbmpgjh.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3onuxrtis.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3orlcuiop.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3shxbogym.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3lmpemptl.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zsstpwyu.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3swanlwhz.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3zdebtsdm.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3glaowrlt.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3zvwyxcvf.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3puqnkaez.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3ogijywsf.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3rcpxkqsy.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3krqkfhpj.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3powlkivn.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3tjhfdvuy.html


<!-- 参考信息 -->