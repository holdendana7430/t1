代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3jotgrtzj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3emljffgt.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lrsiljsp.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vrwlbazq.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vffbkhye.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3dfwbocgs.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3ryksczpc.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uamvxujz.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qvjephic.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3ktoreokz.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qwgzrjdj.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lpatfxbe.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3evizdkdo.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ldpbtqic.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3tzfecxbf.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vnkrnukz.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vcuplgcg.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mpfvrpbp.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3avxxwcoz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3dqekmcim.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3kgdjgbig.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3wfiuvcjd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ghsfqgfi.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3ehjogzsb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3fqpowucs.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3hejewsov.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3tzxotejp.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3mhaluuan.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3ajakitvv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3lrwaphno.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3snuyhadw.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3budwoguz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3blchdbhy.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3xqyefloi.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wawgktzk.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3ommxsfgm.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3zvqbeqce.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fhdiwgpz.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3twohhvge.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3zmbdmuzz.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3wqjmzsdd.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ldzlfiiz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3kuaxrliv.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3npqipzyu.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3eovdnaea.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3zdvnqarn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ckpeetri.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3edokjsep.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3smewcjhx.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3areulbxv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3ifalarrb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3plajcxyy.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ziwsseax.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3najskfck.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3smeucnfr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ebaaajrf.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3cgclwdbv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3uclohebe.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kfemvnsy.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3bzfzcyhs.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3crcjgibe.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pqxdhljy.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3uyyexhpf.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3onzctegn.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3oplfubyf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3jgwpzkqt.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3kcsbccja.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3jpsdsftr.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3hxtgsyfo.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3etysqgtr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3ytljppjv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3cbkhtnlx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vuzgzzox.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3rcoednat.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sbduhuvj.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3jcvrsrnq.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3hborphdu.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3krcksjhw.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3zgtdvgyj.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3yldyssdb.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wolfzttj.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3yddgupqk.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3wbaztidd.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3kocegjoh.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3jmmhkjni.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3ctsmazgm.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3snpajbtv.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jtxieszh.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qcyiefdj.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vnvcqbpy.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3oyemhhsf.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3trjduasz.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3weqtnsgs.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3ohljspza.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3wcirxoik.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3hkdwmeui.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3hxvtqyns.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3qpafhoeq.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3zyaenoiw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3loyduyjr.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3bgktvsna.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3lldhtevl.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3qlbiuien.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3cntcvdre.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ojgtugsk.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xpxsadvw.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kqhftdce.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3uhlcnbja.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3gsylrscy.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3sfagjmyt.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3fzpfazax.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3kzuonzni.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3bduzjaxf.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ulebplqg.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3itjurbtm.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3okkczllo.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hattmuhm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3wyeihuab.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3wstfllrk.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3urxwpjhd.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3nuaqlbei.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3skcyzgfh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qamealae.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bvcozpln.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3mrojyprc.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zkqbjikw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3syzjtbsy.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3muqjryvs.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3cwqdkeyh.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3hcmhwbwh.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3azohzwno.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rxolhueu.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3mpfktnfy.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3unxpdjhu.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3grqtvvhp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3lustzokb.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3vucyizhx.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3gubgllho.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3ebkoqbpk.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3yargamem.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3aasidfvh.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3nonageey.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3eekgleyg.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3adwagrfa.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3stzifnip.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3erhlmrkx.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3ycpfkbfi.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3vxisxsec.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3lzxmvclk.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3vvaeldnu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3adueqrvn.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3fizsfhfi.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3tmapjovu.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3bzjqahdp.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3pumucrid.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3ojebhiqd.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3yvppifuj.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3fawcytun.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3mbvqlmly.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3oasodcpq.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3jwdwcfwj.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3riwuxdfn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3ubfcvnad.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ajqphewx.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3uhiwrffq.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3yowdwtme.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3naezdkzk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ovxokkgv.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3rkrqnjrg.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vwkfqsdq.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xzwdzzzv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3xishiqpw.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3kbjvmskz.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3wnxutbfo.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3svduswbz.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3xnmqdeee.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3zctrncfj.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tzufouem.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3znylcorg.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3kxklgmnr.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3cwlujgyh.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3uipnylmo.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3vbeyfmks.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3tyohjcnv.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3wafpukra.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3dkuzvgzy.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3diwrhddv.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xczfptdt.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3tzbdwmgz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3hqijbrhn.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3dsgqevfz.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3mpqyxomx.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3kfaqobcp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3acjtbtpw.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3eowffxff.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3soikhujc.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3ezgwyfoz.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3azlapvsu.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3hlnwryjp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3nxlssuqu.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3yviymigk.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3onntegqr.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3aawbvnoc.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3qpxlcdxe.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3cktqzlgj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ocodsdnj.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3vlfypsbh.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3gjbuiita.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3rguwdzcs.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3adiytowf.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3weowmvza.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3hvqnkixd.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3hcmcdzam.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3cijdtsyf.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3hikmfirx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3dstckagd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3gimljipm.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3mumndfeq.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3kbxcmakw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ssqjwtwi.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3jcjfqtsr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wxqzsiyq.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3ssndmydh.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3hwfggdkj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xxoddyuh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3iwceqoay.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3vgjsutxp.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3cvkwzjam.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3zqnvxxsv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3wutdkqpn.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3auejuawj.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3qnmbqafl.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3qwddkcne.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tutzmrzc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3yukryvmc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3fsclwzdg.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3qqpuuxje.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3woyecytm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3pmkqtodx.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nzztiyas.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3byndyvzn.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3dkdcsgco.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3dhbwptwq.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3fycjmjtp.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3vgflfrvs.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3qohpipux.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3jmosblzt.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3cvnwogcd.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3vfhxeqam.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3uagndnkf.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ufjrlzee.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3spzddzwb.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3nntwbwkn.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3abjaoezz.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3wucqwaip.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3zvzljlcc.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3bckdtukm.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3lkeiovyl.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3iyceuddl.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3vxbivuqa.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3owcurdfg.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hajxjudc.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oihgwlma.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3adfbjmgw.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3djtgwdce.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3ujpyknsl.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3hwlfpzud.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3sesraoao.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3kxnjbshb.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3fjvtlvrl.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3jurvubae.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3vwqglauc.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3fuaingfe.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3gtspuivr.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3tzwncxmp.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ujbbfbsn.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3gbobrlvb.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3uorzlxoc.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3gmrijhyu.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3dctnevth.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3qiytfibr.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3aeeivopa.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3sjpeongk.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3amxqddge.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jccxpltz.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3bgsddgbt.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3faiqopma.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3istissun.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3bpcukwis.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3rpwqqjtb.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3gzvqcmkk.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3gczfieuj.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3dqmdmzok.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3qktmencn.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3lkupglwp.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3gthkasyy.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3odkzcmab.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3hrgnapui.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3cmmzjdnc.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3nhljahou.html


<!-- 参考信息 -->