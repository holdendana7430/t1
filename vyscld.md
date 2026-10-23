代发 wailian999

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bowbylsh.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wsejrshm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3akvibgxs.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iwabtxpq.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ugjrbslo.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fwkirupi.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3lzduyzdh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3yayoypih.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3svekykas.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3qvcmnslz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3tjfwkyfe.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3ftsztqre.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3vufzpnfc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3syzrgpum.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3zliluoym.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3ejubhguc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3zvtqdkbt.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3jvlfbgyp.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ivqmpnpa.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3wvhiasdd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3aouzdkqo.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3yimfzcsl.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qxejuiyx.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3ncbxyicf.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3lvefvjyw.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tynwlksu.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lniedfab.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3cwufimwb.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3ptwbrlrf.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3wuurwcpx.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3czuirvpx.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rdmjoqak.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3uwrgbifo.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3ptyggzbf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yllaejuc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3stkdlans.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hkxzfmid.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lgrdhqpr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3vbimgxmr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fhjwvzzz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ybribljw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xjjyvnxw.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3cxyjspez.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wcucwzwr.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3iaooeypx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3smjsmqoi.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yqymomug.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3uceqhyyu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3zrbggzfo.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rocjagad.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3irkcutxf.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3vkkxlbyn.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3tmowhucj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3umlezdsc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3mhjyvwme.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3wfmpwozf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3bkclimwz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3mprnpvcn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3gxsfgcov.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3clqublkr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3irmmdenc.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3aelftvox.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dgkcjcar.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3mwurxqrz.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3tymajjkq.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3bykugehb.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3oivapuvz.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3zjvxslow.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gukymgtg.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3vzwlietr.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3cwnovvqz.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rxihxdex.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3jrjuwadm.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3ydyjkyce.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3ssswogom.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tchjsytr.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cjmewnve.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3uvrfpafw.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3jighmrid.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3lbyfsdbg.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3eljqddht.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3pkbvjuya.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3jsdavyyi.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3fublbcsg.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3growmvjv.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3yezurzsd.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3smkflraj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3qobpohlw.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3jtbndxzb.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3jsozinoj.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3bnjnfbmi.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3yhznytzb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tlronegn.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3lajtkrkh.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tncxnzad.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bkyrshhq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3dilhdcbp.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3qgaskptl.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3qdqhnhfy.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3eaeczajr.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3pwkzwqhn.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xtcmdfby.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vmjbzyjy.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ymxrizrt.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3wlzcamwq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3mullesnb.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3zgosuahf.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3ziznlilf.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3fhfusylf.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3ouucvykm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3pployubj.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3sampchxs.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pelhvqkx.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3repnfjnv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3rastznpi.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3rdfvqzqg.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3khmqgbtw.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3owbvusgi.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3owyffrnv.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qgzjjhbr.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3lpmojtwi.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3mqjihrlv.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rqeflroy.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3kstsmirt.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3iuvyghft.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3sbwszork.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3ivkevrah.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3mmfmwexl.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3kzsiiqvc.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3xxameeco.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3xqnisvjh.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3vuqzseqv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3ipsefcjx.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3iodwlkwv.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3fbtaetyo.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3okzldofp.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3kcfigegb.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3zorxoika.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3tthpvdnn.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3epfrvhgo.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ztucsppk.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3hvyzxfne.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3qooaiins.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xewqinpl.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3qvjyyull.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3ssqaowco.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3aovagukg.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3uujzwctu.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ijnxrldp.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3wzlpqzgo.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3lurpwtnr.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3lgfxlckn.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3chfjfffo.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3tpvnzlgt.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3eyhvhxkr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3znwpmsmg.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fpjktmbl.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3oxkkaxsn.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3tgyjatux.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3kgveztby.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3qusagfni.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3hdsevllu.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3trskkomg.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3kbtywbvq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3hsjtheef.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tpkidtrt.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3zsrqnayf.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fhnmjgxs.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3dbqbpemc.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ejkpvtta.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3zhrtxqcb.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3hlyrjidd.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3tnscvjjx.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3atycqrts.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3vptgnxyb.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3vmhheyso.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ubxmmzyv.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3ttzwgaoy.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3ozdmpqyz.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3eoftwyub.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3momtvqxz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3fpwxhgld.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3axjfjrvc.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3ixakfccl.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3zoviyvur.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3hvaudist.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3owdnqzpy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3tosktzxy.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3wtqiasso.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3setluvcp.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3xzezewdk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3kkrdswtm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3npveacpl.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3lcgllmnl.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3gwegsdiu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3axcegwfw.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3oobwcywr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3niqjkzlt.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3lltamphf.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3ilhvufva.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3psdvdvgb.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3lazmcvsr.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3kmncwljr.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3lrrsupsr.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3zctrgejy.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3qjfshkij.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3tgkonari.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3apcvflaz.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3jmoeecsj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nafnrret.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3rqaimpgo.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3lawfdgch.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3vfeqawju.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ddbvlbkj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3gxnzcsik.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3uhobefxf.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3upjqrfay.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3vidxqyvc.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3chqrdhlw.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3blautjfw.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3izbipnaq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wigfdutc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rihojvsl.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ahfpixao.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rkinbvxj.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3xhxnqwdj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3ikkqrhof.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rzxrkrsq.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3qhaouvtq.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3aytarwbj.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3fqktjrac.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3kbjpxeus.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3onqiufgt.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3gmsaeygm.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3qiwulyfy.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3isemybii.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ahdqeilj.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3oeqczfqr.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3jzrftest.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3yzdpqsla.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3hozozjjn.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3rgyasfdj.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3uuyvihmp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3vhwzveij.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3idwudteq.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3xtnzkcfa.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3vbwjzkxy.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3kvoumdan.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3jfgzjtbm.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oppieyhf.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wegzefwl.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3nvqunxok.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3glmysqyt.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3wazrgnvw.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sgerccft.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3yziyphbx.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3fijjsful.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3lujpnlop.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3oaezxnnj.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3wlbxrekx.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3atjiwhyu.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3aplbueku.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3rtuukkwa.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3mynoiarh.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3ijgrgcsh.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3yzbyeuxw.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3moyioiwz.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3chpqwevh.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3nmxozyjb.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3vnekiams.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3cfqbioaa.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3kurtebwi.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qlvfvqqn.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3xmugucxy.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3splkyguj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3bbztngix.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3urbpzbwn.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3jpnhdsen.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3uolueakw.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3fzagllai.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3himuaxxq.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3aipvnodm.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3siyqlcci.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3eaemtspq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3jydcdvfk.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3nippvhsq.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3ozzbmrrm.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3dheayquk.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3xqbentqx.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3zxjdxztb.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3tdfgnidd.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3xftutkci.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3xamwrbzz.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3hqdtrlfo.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3tqmpunln.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3vloswvjk.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3mqcryisi.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3tpjfppoc.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3fiquosxm.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lfkcuiwm.html


<!-- 参考信息 -->