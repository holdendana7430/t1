代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.zdbjq.cn/Article/details/gytdxmwfx.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.fehbvm.com/Article/details/gwxfasdgp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.hesvh.cn/Article/details/gbjcgsneo.sHtML

[F08] 遍历目录
来源：http://mobile.fehbvm.com/Article/details/grpfoqqwe.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.fehbvm.com/Article/details/ghtiduzib.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.fehbvm.com/Article/details/gzcxeenox.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gipgorphk.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gpjfpnrne.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/ghdgeogoq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.hesvh.cn/Article/details/grveseaqa.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.hesvh.cn/Article/details/gknycueag.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.zdbjq.cn/Article/details/ghwoiqhua.sHtML

[F09] 获取文件大小
来源：http://3g.hesvh.cn/Article/details/gbtpnsdoh.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gtwpylygc.sHtML

PHP:  filesize("a.txt");
来源：http://3g.hesvh.cn/Article/details/geqjnnklp.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gjwonjole.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gptbamxoe.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gzynnhbhu.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.zdbjq.cn/Article/details/gqhksntzg.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gxcagqkre.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.fehbvm.com/Article/details/glbusqcby.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fehbvm.com/Article/details/garusbujw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gttbdmugs.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.zdbjq.cn/Article/details/gjpunmlww.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gjrofvbsz.sHtML

TS:   path.extname("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gynhsynwn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.hesvh.cn/Article/details/gcgnsqxum.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gduatubff.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gytuyyfcn.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gxstljfod.sHtML

[F11] 复制与移动文件
来源：http://wap.fehbvm.com/Article/details/gaydbfhrr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gytmfodxv.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.fehbvm.com/Article/details/giqjixmwi.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gkzbctnkz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gkulxyivr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fehbvm.com/Article/details/gqekjdtnv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.hesvh.cn/Article/details/goehtvgcl.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gjyysqkss.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.zdbjq.cn/Article/details/ggiikdfdr.sHtML

[F12] CSV 读写
来源：http://mobile.fehbvm.com/Article/details/gjfrpplac.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.fehbvm.com/Article/details/gumnamwaa.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.hesvh.cn/Article/details/gmdoliqnu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.zdbjq.cn/Article/details/gfibdgcfx.sHtML

TS:   // 同上
来源：http://blog.zdbjq.cn/Article/details/gcpvsttmr.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fehbvm.com/Article/details/gampspkuz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.hesvh.cn/Article/details/gukpwlikh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.fehbvm.com/Article/details/gugatpmor.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.zdbjq.cn/Article/details/gxgmmnkhx.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/goukruaio.sHtML

G. 面向对象
来源：http://read.share.hesvh.cn/Article/details/gvcmzjabm.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxnvpaujj.sHtML

[G01] 定义类
来源：http://www.blog.hesvh.cn/Article/details/gejcivqfi.sHtML

Py:   class User: pass
来源：http://www.blog.hesvh.cn/Article/details/glnbgntwu.sHtML

PHP:  class User {}
来源：http://read.share.fehbvm.com/Article/details/gensiybbm.sHtML

JS:   class User {}
来源：http://wap.fehbvm.com/Article/details/ghpedrpxi.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.zdbjq.cn/Article/details/gkdtomwba.sHtML

Java: class User {}
来源：http://wap.zdbjq.cn/Article/details/gdhhxlfkp.sHtML

Go:   type User struct { Name string }
来源：http://baike.fehbvm.com/Article/details/ghgiuzbew.sHtML

Ruby: class User; end
来源：http://blog.hesvh.cn/Article/details/gfxpcmjhe.sHtML

C#:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gqbgfiulv.sHtML

[G02] 构造函数
来源：http://www.share.zdbjq.cn/Article/details/gmqbgswri.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.fehbvm.com/Article/details/gylvujvmv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.hesvh.cn/Article/details/gxmsrjaab.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gnaodpsgu.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fehbvm.com/Article/details/gitcrwona.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gbhfnsfeb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.fehbvm.com/Article/details/gpqywnntx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fehbvm.com/Article/details/grrazrhem.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fehbvm.com/Article/details/gvgqrmskw.sHtML

[G03] 实例属性
来源：http://3g.hesvh.cn/Article/details/ggrkfkqhf.sHtML

Py:   self.name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/ggewqsncz.sHtML

PHP:  public string $name = "x";
来源：http://wap.fehbvm.com/Article/details/giibczeri.sHtML

JS:   this.name = "x";
来源：http://wap.fehbvm.com/Article/details/guweomeix.sHtML

TS:   name: string = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gbpbtwhwm.sHtML

Java: private String name;
来源：http://baike.zdbjq.cn/Article/details/glrlwzyeq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.fehbvm.com/Article/details/gfncjacso.sHtML

Ruby: @name = "x"
来源：http://blog.hesvh.cn/Article/details/gwioucuzs.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.zdbjq.cn/Article/details/gwvxeckan.sHtML

[G04] 定义方法
来源：http://www.m.share.zdbjq.cn/Article/details/ggdoltxtd.sHtML

Py:   def greet(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gnvlgjjsr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gupvjfzzf.sHtML

JS:   greet() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/glocwjkko.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gjwdjocxe.sHtML

Java: String greet() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gdpiumytj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/glegglpro.sHtML

Ruby: def greet; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gphbutzqi.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gnnjdqolb.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/glnacotno.sHtML

Py:   class Admin(User): pass
来源：http://wap.hesvh.cn/Article/details/goojcjjkj.sHtML

PHP:  class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gpqvqibmv.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gveqrdfdo.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gckuliryn.sHtML

Java: class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gcxdafibq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.zdbjq.cn/Article/details/ghlhczosk.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.zdbjq.cn/Article/details/ghmwzrjta.sHtML

C#:   class Admin : User {}
来源：http://mobile.hesvh.cn/Article/details/gavmaoxbv.sHtML

[G06] 重写方法
来源：http://www.blog.hesvh.cn/Article/details/gkzhhohzs.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.hesvh.cn/Article/details/glsjbeeaf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/ggkeblbjd.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/grgogotrz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gvnfwqlkd.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gedxivtct.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.zdbjq.cn/Article/details/gphamxskz.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.zdbjq.cn/Article/details/gguqlmbps.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.fehbvm.com/Article/details/golsdeotu.sHtML

[G07] 调用父类方法
来源：http://www.blog.zdbjq.cn/Article/details/grxrcxefg.sHtML

Py:   super().greet()
来源：http://baike.fehbvm.com/Article/details/gdoohkcrz.sHtML

PHP:  parent::greet();
来源：http://3g.fehbvm.com/Article/details/gzhbvabcl.sHtML

JS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/grnodpkff.sHtML

TS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/ghslqtacb.sHtML

Java: super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gyjjdmhka.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.zdbjq.cn/Article/details/gaceuueet.sHtML

Ruby: super
来源：http://3g.hesvh.cn/Article/details/gyrzysdha.sHtML

C#:   base.Greet();
来源：http://www.blog.hesvh.cn/Article/details/gtfixwjmu.sHtML

[G08] 静态方法与属性
来源：http://www.share.hesvh.cn/Article/details/ghcfuwapp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.hesvh.cn/Article/details/gityconxu.sHtML

PHP:  public static function f() {}
来源：http://m.share.zdbjq.cn/Article/details/gylvwqqhf.sHtML

JS:   static f() {}
来源：http://wap.fehbvm.com/Article/details/gxkenyvto.sHtML

TS:   static f(): void {}
来源：http://3g.zdbjq.cn/Article/details/gdbfcgryg.sHtML

Java: static void f() {}
来源：http://mobile.fehbvm.com/Article/details/gpepphrlh.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.hesvh.cn/Article/details/gwjedrwdk.sHtML

Ruby: def self.f; end
来源：http://blog.fehbvm.com/Article/details/gvryfyhqx.sHtML

C#:   public static void F() {}
来源：http://mobile.fehbvm.com/Article/details/guzlsuooi.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.zdbjq.cn/Article/details/gabizaeeg.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.zdbjq.cn/Article/details/gkmhnsgoi.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.zdbjq.cn/Article/details/gqqrlxjej.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.zdbjq.cn/Article/details/gquiadhme.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.fehbvm.com/Article/details/ginuuvuiv.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gqeqydmrd.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.hesvh.cn/Article/details/gaxdmfwis.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fehbvm.com/Article/details/ggkzpqzuy.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.zdbjq.cn/Article/details/gnibmzhsx.sHtML

[G10] 访问控制
来源：http://read.share.zdbjq.cn/Article/details/gdkcuxwnz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.zdbjq.cn/Article/details/gcfrqdkhp.sHtML

PHP:  public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gzyrnplqp.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.zdbjq.cn/Article/details/gnmxnvnov.sHtML

TS:   public / protected / private
来源：http://wap.hesvh.cn/Article/details/ghxselynt.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.hesvh.cn/Article/details/glbpupooh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.fehbvm.com/Article/details/gpkfbtmtw.sHtML

Ruby: public / protected / private
来源：http://www.share.hesvh.cn/Article/details/geuwwjfuf.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.hesvh.cn/Article/details/ghzfvznog.sHtML

[G11] getter / setter
来源：http://m.share.zdbjq.cn/Article/details/ghbkpzbil.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fehbvm.com/Article/details/gfjwmdvmf.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gvjxikdwt.sHtML

JS:   get name() { return this._name; }
来源：http://baike.fehbvm.com/Article/details/gargoyzuk.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gmkcmmrtj.sHtML

Java: public String getName() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gjemkfuol.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gykrbwfwd.sHtML

Ruby: attr_accessor :name
来源：http://m.share.hesvh.cn/Article/details/gkmdysgel.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.zdbjq.cn/Article/details/gwregoycy.sHtML

[G12] 对象转字符串
来源：http://www.blog.fehbvm.com/Article/details/ghxrtysze.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gnxpmhbbq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gkhubelyv.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gobdepcwp.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gsbyhsopq.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gnpnjavgd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/geefwsuiu.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gbbjbwphm.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.fehbvm.com/Article/details/gontugzxg.sHtML

[G13] 判断对象类型
来源：http://mobile.fehbvm.com/Article/details/gmbhlzahm.sHtML

Py:   isinstance(u, User)
来源：http://www.share.fehbvm.com/Article/details/gdanjymde.sHtML

PHP:  $u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gfzecnpbt.sHtML

JS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/glxvkjdhj.sHtML

TS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/gyouhjdcu.sHtML

Java: u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gftsmyzph.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.hesvh.cn/Article/details/goiklkywb.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.fehbvm.com/Article/details/gpxolpupx.sHtML

C#:   u is User
来源：http://3g.fehbvm.com/Article/details/gscyvhuoa.sHtML

[G14] 数据类 / record
来源：http://www.blog.zdbjq.cn/Article/details/grtpeslcs.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.hesvh.cn/Article/details/gfkstguef.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.zdbjq.cn/Article/details/gxxkwegtt.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.hesvh.cn/Article/details/gihewamst.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.fehbvm.com/Article/details/ghurzfnfa.sHtML

Java: record User(String name, int age) {}
来源：http://blog.zdbjq.cn/Article/details/givkmcwks.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.hesvh.cn/Article/details/gmmruvgrt.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.hesvh.cn/Article/details/gmeteiypy.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.fehbvm.com/Article/details/ggirdhxpp.sHtML

[G15] 枚举
来源：http://read.share.zdbjq.cn/Article/details/gjqflsvyy.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.hesvh.cn/Article/details/gqnnzxjxy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.hesvh.cn/Article/details/gsavjsulf.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.hesvh.cn/Article/details/gudlahlsw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gefdalwlq.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.fehbvm.com/Article/details/gleqvingx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.zdbjq.cn/Article/details/gibzrlyrf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.hesvh.cn/Article/details/guxnvabmv.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/gvonvfcrl.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.fehbvm.com/Article/details/gseudzguf.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fehbvm.com/Article/details/gaasziabc.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.fehbvm.com/Article/details/gyrnleqef.sHtML

JS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/gtgrbpzrd.sHtML

TS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/gkiqvfmcq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.zdbjq.cn/Article/details/gpsbawajh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.zdbjq.cn/Article/details/gkafuhrvu.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.zdbjq.cn/Article/details/gyszfmtwf.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.hesvh.cn/Article/details/gzonyhuer.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gtofklfjj.sHtML

H. 异常与错误处理
来源：http://mobile.zdbjq.cn/Article/details/gzcjhpurg.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gnpaybxwb.sHtML

[H01] try / catch 基础
来源：http://baike.hesvh.cn/Article/details/gcbsstakl.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.hesvh.cn/Article/details/gwotcxcci.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.hesvh.cn/Article/details/gxmstbscn.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gojmbbadr.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gfwejcnht.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.fehbvm.com/Article/details/gcplafhmo.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.hesvh.cn/Article/details/gtatfguzb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.fehbvm.com/Article/details/gwtmigijc.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.fehbvm.com/Article/details/gegkhztkm.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.zdbjq.cn/Article/details/gqclyuhxa.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.hesvh.cn/Article/details/gpivaouqb.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gyprpbauv.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/ghbkoeyvj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gsyvbxuzg.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gykfxowrl.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.fehbvm.com/Article/details/gewmbepko.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fehbvm.com/Article/details/gztvlocxw.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gzolwoyvl.sHtML

[H03] 主动抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/guvhyrqlx.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.zdbjq.cn/Article/details/gylmkmukt.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gfhhwkqyz.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gklbclbdn.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/gmicjqsnp.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gdbrvklzu.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.zdbjq.cn/Article/details/ghzbxeamb.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.hesvh.cn/Article/details/ghtjyzzhb.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/gnbpchweu.sHtML

[H04] 自定义异常类型
来源：http://www.share.hesvh.cn/Article/details/gvwmjuvkj.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.fehbvm.com/Article/details/gnmvzzrkf.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.hesvh.cn/Article/details/gotnggjyf.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.hesvh.cn/Article/details/gjrnocgiw.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/gcfqcadhz.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.hesvh.cn/Article/details/grzhuaijv.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.fehbvm.com/Article/details/gfegyegqs.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.fehbvm.com/Article/details/glifkizpo.sHtML

C#:   class MyException : Exception {}
来源：http://3g.zdbjq.cn/Article/details/gdwuprduo.sHtML

[H05] 捕获特定类型
来源：http://m.share.fehbvm.com/Article/details/gkrxkeksk.sHtML

Py:   except ValueError as e:
来源：http://baike.zdbjq.cn/Article/details/gynpizysq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.fehbvm.com/Article/details/gjaualptm.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.hesvh.cn/Article/details/ghpssmidn.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.zdbjq.cn/Article/details/gvefzwavu.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.hesvh.cn/Article/details/gthmegxpj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.zdbjq.cn/Article/details/grbmqjfuw.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.hesvh.cn/Article/details/gjjudewql.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.zdbjq.cn/Article/details/ggzfupjmg.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.fehbvm.com/Article/details/gzlsezocn.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.hesvh.cn/Article/details/ghibyzkko.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/gjybtcxiq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/gljatffon.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/ginnqrtcf.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.fehbvm.com/Article/details/gzxepcjbj.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.fehbvm.com/Article/details/glkupwwqx.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.hesvh.cn/Article/details/gpltkjsgn.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.fehbvm.com/Article/details/gncchgsdl.sHtML

[H07] 断言
来源：http://www.share.hesvh.cn/Article/details/gszbncjiy.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.fehbvm.com/Article/details/gtugjshbp.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gpinrwqpw.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/gxugdhltt.sHtML

TS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gbrsbrkbq.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.zdbjq.cn/Article/details/gezzqmkqi.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.hesvh.cn/Article/details/goguvrabz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.fehbvm.com/Article/details/gocwrtgbr.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/ghhhpipfl.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.hesvh.cn/Article/details/gqkpnasyv.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.zdbjq.cn/Article/details/goazioiep.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.hesvh.cn/Article/details/gbppqjjao.sHtML

JS:   e.message;  e.stack
来源：http://3g.fehbvm.com/Article/details/gfwwskpqf.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.zdbjq.cn/Article/details/gaazzaxwi.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.zdbjq.cn/Article/details/gqteanmwn.sHtML

Go:   err.Error()
来源：http://mobile.zdbjq.cn/Article/details/gbhosuoqt.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.hesvh.cn/Article/details/gqwpgopdx.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.fehbvm.com/Article/details/gdpbazugo.sHtML

[H09] 带错误码的异常
来源：http://www.blog.hesvh.cn/Article/details/gpejdfnur.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.zdbjq.cn/Article/details/gsfwyouly.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.hesvh.cn/Article/details/gbrlrjtnw.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.fehbvm.com/Article/details/ggmhchmfz.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.fehbvm.com/Article/details/gcistbpmb.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.zdbjq.cn/Article/details/gfjojmbgn.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.zdbjq.cn/Article/details/gtjsjzmle.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.m.share.hesvh.cn/Article/details/getwpcrmn.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.zdbjq.cn/Article/details/gfppwxzje.sHtML

[H10] 资源自动释放
来源：http://baike.fehbvm.com/Article/details/gktgzecdc.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.zdbjq.cn/Article/details/gitqftekg.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.fehbvm.com/Article/details/grlqxglgt.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.hesvh.cn/Article/details/glqjvesgg.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.hesvh.cn/Article/details/gaekvrvua.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.zdbjq.cn/Article/details/gpmppngaf.sHtML

Go:   defer f.Close()
来源：http://mobile.zdbjq.cn/Article/details/gylgveloh.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.zdbjq.cn/Article/details/gzocikjnm.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.fehbvm.com/Article/details/glcghazdh.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmdymkanp.sHtML

I. 正则表达式
来源：http://mobile.fehbvm.com/Article/details/galwtvzqk.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gcjrjizbi.sHtML

[I01] 判断是否匹配
来源：http://wap.fehbvm.com/Article/details/geiddceji.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.fehbvm.com/Article/details/gwppwcsca.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.zdbjq.cn/Article/details/gumjphrac.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.hesvh.cn/Article/details/gmowguadd.sHtML

TS:   /\d+/.test(s)
来源：http://wap.zdbjq.cn/Article/details/grucmtlpu.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.fehbvm.com/Article/details/gkrvjardk.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.zdbjq.cn/Article/details/geogxhupn.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.hesvh.cn/Article/details/gbpmjkucd.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.zdbjq.cn/Article/details/gqnovewja.sHtML


<!-- 参考信息 -->