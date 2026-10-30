代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gbbzuuone.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.hesvh.cn/Article/details/gchvptfpb.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.zdbjq.cn/Article/details/gfxwzaiyb.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.zdbjq.cn/Article/details/ggzywuabv.sHtML

[F09] 获取文件大小
来源：http://m.share.hesvh.cn/Article/details/gxylxtjny.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.zdbjq.cn/Article/details/ghkpjxjkt.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/guceqjguj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/gtwnleexj.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gkcvkafgo.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gynequijd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.hesvh.cn/Article/details/gwixhiydu.sHtML

Ruby: File.size("a.txt")
来源：http://blog.hesvh.cn/Article/details/gjfueielc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fehbvm.com/Article/details/gyfejjbct.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fehbvm.com/Article/details/gkujyxumu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gieydqgiz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gktxryapu.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/glplnmxro.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gbeowffns.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.zdbjq.cn/Article/details/gllammpdf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/ggagsfttc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/glsdsgbhf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gvjhemhod.sHtML

[F11] 复制与移动文件
来源：http://mobile.hesvh.cn/Article/details/gzhxzucqn.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gdhuhytjr.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.fehbvm.com/Article/details/gifczdxmq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gmyhsrrlu.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gkzanqxek.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gxmvkuyni.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fehbvm.com/Article/details/gqvqjbuli.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/geuhafcaw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.hesvh.cn/Article/details/gsvrymcil.sHtML

[F12] CSV 读写
来源：http://3g.zdbjq.cn/Article/details/gysygvruv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fehbvm.com/Article/details/ghuxiolkp.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.fehbvm.com/Article/details/ggplspzoj.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fehbvm.com/Article/details/gaxrknlnz.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/goptxfptd.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.zdbjq.cn/Article/details/gilqnlcto.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.zdbjq.cn/Article/details/gpycxldan.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.zdbjq.cn/Article/details/gelhuuhlb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.hesvh.cn/Article/details/gxnfcwate.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gwsgvjffw.sHtML

G. 面向对象
来源：http://www.m.share.zdbjq.cn/Article/details/gilotrnon.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gcifnlezh.sHtML

[G01] 定义类
来源：http://www.share.zdbjq.cn/Article/details/gdfrzwtwh.sHtML

Py:   class User: pass
来源：http://mobile.hesvh.cn/Article/details/gzgmqmyum.sHtML

PHP:  class User {}
来源：http://baike.zdbjq.cn/Article/details/gfrrdhasu.sHtML

JS:   class User {}
来源：http://www.share.fehbvm.com/Article/details/glplqsqry.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.hesvh.cn/Article/details/gkfblllcg.sHtML

Java: class User {}
来源：http://www.blog.hesvh.cn/Article/details/ghruziyjp.sHtML

Go:   type User struct { Name string }
来源：http://m.share.zdbjq.cn/Article/details/gqqdemjwa.sHtML

Ruby: class User; end
来源：http://www.m.share.zdbjq.cn/Article/details/gocinlooh.sHtML

C#:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gyvzinlte.sHtML

[G02] 构造函数
来源：http://baike.zdbjq.cn/Article/details/gblxoxnae.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.hesvh.cn/Article/details/gubwrwvws.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.fehbvm.com/Article/details/gzozocwei.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/guwflwwff.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.zdbjq.cn/Article/details/gpjtstgtg.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gszfwloqg.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.fehbvm.com/Article/details/glanockpy.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.hesvh.cn/Article/details/gzbjvaxix.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.hesvh.cn/Article/details/gkevughhb.sHtML

[G03] 实例属性
来源：http://m.share.fehbvm.com/Article/details/gbjruvdja.sHtML

Py:   self.name = "x"
来源：http://www.share.hesvh.cn/Article/details/gtmrjuprv.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gxyxaxidl.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/ghctbzvrk.sHtML

TS:   name: string = "x";
来源：http://m.share.zdbjq.cn/Article/details/gqwqimnwb.sHtML

Java: private String name;
来源：http://www.share.hesvh.cn/Article/details/ghajturlg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.zdbjq.cn/Article/details/glhmutgiv.sHtML

Ruby: @name = "x"
来源：http://www.share.zdbjq.cn/Article/details/ggikqzpfa.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gdoxlpmri.sHtML

[G04] 定义方法
来源：http://m.share.zdbjq.cn/Article/details/gacewlqqb.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gyglvvcmb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gtepzttyu.sHtML

JS:   greet() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gfqsdzmyp.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/ghapfnkaw.sHtML

Java: String greet() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gjafkjmxe.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gmulgldmm.sHtML

Ruby: def greet; @name; end
来源：http://www.share.fehbvm.com/Article/details/grdzopzed.sHtML

C#:   public string Greet() => Name;
来源：http://wap.zdbjq.cn/Article/details/gzbhtuxxd.sHtML

[G05] 继承
来源：http://mobile.zdbjq.cn/Article/details/gmxceuqtj.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fehbvm.com/Article/details/gpliflaif.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gzuwfgnmh.sHtML

JS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/ggulppbds.sHtML

TS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/giqowhlde.sHtML

Java: class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gvmupmyai.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.zdbjq.cn/Article/details/gcgohwwrh.sHtML

Ruby: class Admin < User; end
来源：http://3g.fehbvm.com/Article/details/gnxkosiwa.sHtML

C#:   class Admin : User {}
来源：http://3g.fehbvm.com/Article/details/gzlzdbaou.sHtML

[G06] 重写方法
来源：http://mobile.hesvh.cn/Article/details/gncogybts.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.zdbjq.cn/Article/details/gtynsuibi.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gupuumgpo.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gkeonivvk.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gbonzkifx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/ggngcevhc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.zdbjq.cn/Article/details/gkdqptsqe.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.zdbjq.cn/Article/details/gsgscwgma.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.zdbjq.cn/Article/details/grwtgsysr.sHtML

[G07] 调用父类方法
来源：http://baike.hesvh.cn/Article/details/gkvapwgwd.sHtML

Py:   super().greet()
来源：http://3g.zdbjq.cn/Article/details/gybxggpak.sHtML

PHP:  parent::greet();
来源：http://3g.hesvh.cn/Article/details/gxerkhyva.sHtML

JS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gmhqubtgw.sHtML

TS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gylpuzckl.sHtML

Java: super.greet();
来源：http://m.share.fehbvm.com/Article/details/ginnfdmkb.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.fehbvm.com/Article/details/gejitfvps.sHtML

Ruby: super
来源：http://read.share.zdbjq.cn/Article/details/ghncasllr.sHtML

C#:   base.Greet();
来源：http://m.share.hesvh.cn/Article/details/gqxwkpqyh.sHtML

[G08] 静态方法与属性
来源：http://read.share.zdbjq.cn/Article/details/gulefnawp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.fehbvm.com/Article/details/gnasucvmk.sHtML

PHP:  public static function f() {}
来源：http://wap.hesvh.cn/Article/details/gahpvvmyo.sHtML

JS:   static f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwfbcdwcw.sHtML

TS:   static f(): void {}
来源：http://blog.fehbvm.com/Article/details/grfgobkfl.sHtML

Java: static void f() {}
来源：http://www.blog.fehbvm.com/Article/details/gfikibajy.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.hesvh.cn/Article/details/gqopbyzsp.sHtML

Ruby: def self.f; end
来源：http://blog.hesvh.cn/Article/details/gwdvhocpw.sHtML

C#:   public static void F() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtieobbze.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.hesvh.cn/Article/details/gxyctyqwz.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fehbvm.com/Article/details/gmulmhksb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/gvdwxjzao.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.fehbvm.com/Article/details/gxonklqjw.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.fehbvm.com/Article/details/gsqztixxu.sHtML

Java: interface Shape { double area(); }
来源：http://3g.fehbvm.com/Article/details/giedzvjum.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.hesvh.cn/Article/details/gcfkzughs.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.fehbvm.com/Article/details/gjplkgtxz.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.hesvh.cn/Article/details/gjxdwxvng.sHtML

[G10] 访问控制
来源：http://blog.fehbvm.com/Article/details/gosppnewl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.zdbjq.cn/Article/details/gmtiphmsb.sHtML

PHP:  public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gbqcttitz.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.zdbjq.cn/Article/details/gxnroeten.sHtML

TS:   public / protected / private
来源：http://baike.hesvh.cn/Article/details/geblhjmdy.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.zdbjq.cn/Article/details/gmvcbpauo.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.zdbjq.cn/Article/details/gggievzkm.sHtML

Ruby: public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gwzcqjlkp.sHtML

C#:   public / protected / private / internal
来源：http://www.share.fehbvm.com/Article/details/gmrzymwpl.sHtML

[G11] getter / setter
来源：http://mobile.zdbjq.cn/Article/details/goazqxows.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fehbvm.com/Article/details/gbvfslgbv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gpnynhsgn.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gztwcinbt.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gkrrxmfkc.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gbxrdowia.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gpvmnhtgn.sHtML

Ruby: attr_accessor :name
来源：http://3g.zdbjq.cn/Article/details/ghvzbahux.sHtML

C#:   public string Name { get; set; }
来源：http://baike.fehbvm.com/Article/details/gerverknh.sHtML

[G12] 对象转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gdsuguznh.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gftbgyulr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gfvjvyxph.sHtML

JS:   toString() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gpnsxkmyl.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/grwnmmfwy.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.hesvh.cn/Article/details/guexwwnfx.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gltkvhmwn.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gzfrboxmm.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.fehbvm.com/Article/details/gzqgtzeui.sHtML

[G13] 判断对象类型
来源：http://baike.fehbvm.com/Article/details/gevoaqsks.sHtML

Py:   isinstance(u, User)
来源：http://read.share.zdbjq.cn/Article/details/gfoofcpno.sHtML

PHP:  $u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gvmmbjuem.sHtML

JS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gviwamclz.sHtML

TS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gkyxfbsef.sHtML

Java: u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gxagrnffc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.zdbjq.cn/Article/details/giksxbppl.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.hesvh.cn/Article/details/gnauqvdik.sHtML

C#:   u is User
来源：http://baike.hesvh.cn/Article/details/gqlskehbd.sHtML

[G14] 数据类 / record
来源：http://read.share.zdbjq.cn/Article/details/gtdygeolp.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fehbvm.com/Article/details/gpbmvoskh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.hesvh.cn/Article/details/ghgdutguy.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fehbvm.com/Article/details/gqsrixkfs.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.zdbjq.cn/Article/details/grzueppgj.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.hesvh.cn/Article/details/giafxkmas.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.zdbjq.cn/Article/details/gcygagphs.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.hesvh.cn/Article/details/gvqqgydoh.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.fehbvm.com/Article/details/gtfkcyixs.sHtML

[G15] 枚举
来源：http://baike.hesvh.cn/Article/details/glaxvrwlm.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.fehbvm.com/Article/details/gjfwdurid.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.zdbjq.cn/Article/details/gifkubmis.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.hesvh.cn/Article/details/genbsqikp.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/gjtwwcazm.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.zdbjq.cn/Article/details/gbegyzwko.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.zdbjq.cn/Article/details/gnhirsizz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.hesvh.cn/Article/details/gtkzqscba.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/gdfmqyklv.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.zdbjq.cn/Article/details/gmrvdceuh.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.zdbjq.cn/Article/details/gnxrsyhor.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.hesvh.cn/Article/details/gopyyzxkh.sHtML

JS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/ghilwyolr.sHtML

TS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/gxhlkroxz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.hesvh.cn/Article/details/golmbfyuo.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.zdbjq.cn/Article/details/githxetaj.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.hesvh.cn/Article/details/grrbbzkxy.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/gekrrsdeg.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gpletonrh.sHtML

H. 异常与错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gictaitqh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gsnxfuwxg.sHtML

[H01] try / catch 基础
来源：http://mobile.zdbjq.cn/Article/details/guvmflsrb.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.fehbvm.com/Article/details/gljnshtht.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.fehbvm.com/Article/details/gqdkofubt.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/glyzeindu.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gskdhvnju.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.zdbjq.cn/Article/details/glucbeqzy.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.fehbvm.com/Article/details/grpupbbpo.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.fehbvm.com/Article/details/gegcylqdx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.hesvh.cn/Article/details/gbdiypiml.sHtML

[H02] finally / ensure 收尾
来源：http://blog.fehbvm.com/Article/details/gmtufmkyc.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.fehbvm.com/Article/details/gapbwtxip.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/grtojtiyy.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/ggoomawgm.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gfqimsrux.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gqzovewkc.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.zdbjq.cn/Article/details/gjeyuczcm.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.hesvh.cn/Article/details/gzqyychmx.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/geihfpftt.sHtML

[H03] 主动抛出异常
来源：http://wap.hesvh.cn/Article/details/gnqqhpfuf.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.hesvh.cn/Article/details/gisxztaux.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/goerwgkgm.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gkoaefpje.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gjfqocowd.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gaxlmrxoc.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.hesvh.cn/Article/details/gpjxvivgk.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.hesvh.cn/Article/details/getgwrttk.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gbtytakkf.sHtML

[H04] 自定义异常类型
来源：http://blog.zdbjq.cn/Article/details/grfupnair.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.fehbvm.com/Article/details/gqapzoowq.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/gxemeulrw.sHtML

JS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/gvokuxdew.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/gocsfhadm.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/gxysmkaju.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.zdbjq.cn/Article/details/gupfqcqgc.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.hesvh.cn/Article/details/gezhindhg.sHtML

C#:   class MyException : Exception {}
来源：http://blog.zdbjq.cn/Article/details/glfsbrrnp.sHtML

[H05] 捕获特定类型
来源：http://read.share.hesvh.cn/Article/details/gouxjlksc.sHtML

Py:   except ValueError as e:
来源：http://www.share.fehbvm.com/Article/details/gqslqctuv.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.fehbvm.com/Article/details/gfrqexbla.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/ghfsllwbz.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzzxbijcv.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.fehbvm.com/Article/details/grkdgixhl.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.zdbjq.cn/Article/details/gppcbxhwu.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.zdbjq.cn/Article/details/gstdvyqsc.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fehbvm.com/Article/details/gstxcfqry.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.fehbvm.com/Article/details/gikdhwiqs.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.fehbvm.com/Article/details/grloxduyz.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gatsjidbv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/gzurkhqxk.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.zdbjq.cn/Article/details/gkwpjnyhv.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.zdbjq.cn/Article/details/gafbtqzer.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.hesvh.cn/Article/details/gynmaoati.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.zdbjq.cn/Article/details/gmnfasjyk.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.zdbjq.cn/Article/details/gcgihnofc.sHtML

[H07] 断言
来源：http://www.share.zdbjq.cn/Article/details/gpxwvwgmo.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.hesvh.cn/Article/details/gtroushax.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gytgychwh.sHtML

JS:   console.assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gpspdiclg.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gtchvsccy.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.hesvh.cn/Article/details/gpsjmmbsx.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.fehbvm.com/Article/details/gptyiirer.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.hesvh.cn/Article/details/gvkeksjop.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gwbcvmvce.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.fehbvm.com/Article/details/gewmgqvlf.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.zdbjq.cn/Article/details/gfvgdchoa.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.fehbvm.com/Article/details/gszbimqkb.sHtML

JS:   e.message;  e.stack
来源：http://m.share.hesvh.cn/Article/details/geywouxzi.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.fehbvm.com/Article/details/ghjnpdoin.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.zdbjq.cn/Article/details/gduuozobw.sHtML

Go:   err.Error()
来源：http://wap.hesvh.cn/Article/details/gnqxerivh.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.fehbvm.com/Article/details/guqlcndwd.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.fehbvm.com/Article/details/gxzmepgkz.sHtML

[H09] 带错误码的异常
来源：http://3g.hesvh.cn/Article/details/gpdcdzmwa.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.zdbjq.cn/Article/details/gopvaybik.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.fehbvm.com/Article/details/gxpzcqdca.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.hesvh.cn/Article/details/geyvkzqew.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.hesvh.cn/Article/details/gprgbsnaj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.hesvh.cn/Article/details/gpkablxiy.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.fehbvm.com/Article/details/gcqohdvvb.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.hesvh.cn/Article/details/gqsbtntjw.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.hesvh.cn/Article/details/grkdtcpmx.sHtML

[H10] 资源自动释放
来源：http://www.share.hesvh.cn/Article/details/gkdimsksk.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.hesvh.cn/Article/details/gqezfhbou.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.zdbjq.cn/Article/details/gqpfngykf.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.zdbjq.cn/Article/details/glfejawbf.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.hesvh.cn/Article/details/grkqhbsou.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.zdbjq.cn/Article/details/grfckebff.sHtML

Go:   defer f.Close()
来源：http://www.blog.zdbjq.cn/Article/details/gqznuuzme.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.fehbvm.com/Article/details/gwwdxjldr.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gujtbozgz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/guzxhwrne.sHtML

I. 正则表达式
来源：http://www.m.share.hesvh.cn/Article/details/glspfplmi.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gpdfekkll.sHtML

[I01] 判断是否匹配
来源：http://3g.hesvh.cn/Article/details/gticowniz.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.hesvh.cn/Article/details/gxwbgkfom.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.hesvh.cn/Article/details/gjezkrhpa.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.zdbjq.cn/Article/details/gdafmmkwn.sHtML

TS:   /\d+/.test(s)
来源：http://baike.hesvh.cn/Article/details/gvhkkbxhw.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.hesvh.cn/Article/details/gnpwxsify.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.zdbjq.cn/Article/details/gsjozslau.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.fehbvm.com/Article/details/gumcigbmd.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.hesvh.cn/Article/details/glodwkehs.sHtML

[I02] 提取所有匹配
来源：http://3g.zdbjq.cn/Article/details/ggkzrkhow.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.hesvh.cn/Article/details/gwenuspmf.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.zdbjq.cn/Article/details/gsxkgbqef.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.share.zdbjq.cn/Article/details/gbmrzlemy.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.fehbvm.com/Article/details/gldrsjbdb.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.zdbjq.cn/Article/details/gjquqsbtj.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.fehbvm.com/Article/details/gpxirlkfa.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.fehbvm.com/Article/details/gnlkplyfg.sHtML


<!-- 参考信息 -->