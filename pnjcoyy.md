代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.hesvh.cn/Article/details/gxizqgjbu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fehbvm.com/Article/details/gacteamzs.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gabwzgygy.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/ggusnongg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/guxrevbzo.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.hesvh.cn/Article/details/gegjatisv.sHtML

Ruby: Dir.children("dir")
来源：http://blog.fehbvm.com/Article/details/gsnvkkpla.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.hesvh.cn/Article/details/ganhldjdh.sHtML

[F09] 获取文件大小
来源：http://read.share.zdbjq.cn/Article/details/gfmtyuqta.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gaqfrsgka.sHtML

PHP:  filesize("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gltuspwlg.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gzkkzurdc.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gzxlkbgsn.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gdbrkyvfl.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.hesvh.cn/Article/details/grqbkuraw.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gkpscqrsc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.zdbjq.cn/Article/details/ghczhtefn.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.zdbjq.cn/Article/details/gjawlmszy.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/ggfdwklsg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.hesvh.cn/Article/details/gtgyuscid.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gftqyfhqe.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gqythrkwm.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.zdbjq.cn/Article/details/grdshtgsl.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gzthvwvbp.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gqirnfspr.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gdqrgoeea.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fehbvm.com/Article/details/gwxmzfjcj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gxmcucund.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.zdbjq.cn/Article/details/ggwuonrru.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gurzkxgqh.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gzhyoorul.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.zdbjq.cn/Article/details/guqkatwtn.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.hesvh.cn/Article/details/gmwkwknxi.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gfcxzeouq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.hesvh.cn/Article/details/gjxkfudve.sHtML

[F12] CSV 读写
来源：http://baike.hesvh.cn/Article/details/gdzzzrdmt.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.fehbvm.com/Article/details/gvvlelntr.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.hesvh.cn/Article/details/gqrwdtspi.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.hesvh.cn/Article/details/guzvneyck.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/gzccqaupp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.hesvh.cn/Article/details/glwvnkckf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.hesvh.cn/Article/details/gioqxlevt.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.zdbjq.cn/Article/details/gfeytjrnm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.fehbvm.com/Article/details/gszpjqqxx.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gihnrndnu.sHtML

G. 面向对象
来源：http://wap.zdbjq.cn/Article/details/gqnecexku.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gakgmgrpw.sHtML

[G01] 定义类
来源：http://m.share.fehbvm.com/Article/details/gwaishekr.sHtML

Py:   class User: pass
来源：http://m.share.zdbjq.cn/Article/details/ggpgdzyjq.sHtML

PHP:  class User {}
来源：http://m.share.fehbvm.com/Article/details/gelvjxcxu.sHtML

JS:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gfybmomui.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.hesvh.cn/Article/details/golijddoj.sHtML

Java: class User {}
来源：http://www.blog.hesvh.cn/Article/details/gzygmhfre.sHtML

Go:   type User struct { Name string }
来源：http://www.share.zdbjq.cn/Article/details/gubuhkhsm.sHtML

Ruby: class User; end
来源：http://m.share.zdbjq.cn/Article/details/gqrpdevhi.sHtML

C#:   class User {}
来源：http://mobile.hesvh.cn/Article/details/ggvpnkeyb.sHtML

[G02] 构造函数
来源：http://www.m.share.fehbvm.com/Article/details/ggwiniokc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.hesvh.cn/Article/details/gffrnjdyr.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.hesvh.cn/Article/details/gcsckstvr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/ggdoaoqab.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/gcrmtvqfl.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gwpmyjdrk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.fehbvm.com/Article/details/gnmgvrvsg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.fehbvm.com/Article/details/gwulugbzg.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.fehbvm.com/Article/details/gwwbvrilk.sHtML

[G03] 实例属性
来源：http://read.share.hesvh.cn/Article/details/gtinevdla.sHtML

Py:   self.name = "x"
来源：http://3g.fehbvm.com/Article/details/grocgkzld.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fehbvm.com/Article/details/gwrqccjfj.sHtML

JS:   this.name = "x";
来源：http://wap.hesvh.cn/Article/details/gymmbhomk.sHtML

TS:   name: string = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/guepdatxw.sHtML

Java: private String name;
来源：http://www.blog.zdbjq.cn/Article/details/gudsazukk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fehbvm.com/Article/details/grgxfppwq.sHtML

Ruby: @name = "x"
来源：http://blog.fehbvm.com/Article/details/gxtmozfht.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.hesvh.cn/Article/details/gcimnocvz.sHtML

[G04] 定义方法
来源：http://www.blog.hesvh.cn/Article/details/gexwavdsq.sHtML

Py:   def greet(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gutatfhsz.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gzewnvmpx.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gepiclmzv.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gmqdrozru.sHtML

Java: String greet() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gdtjnbusj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gqnkwcjkv.sHtML

Ruby: def greet; @name; end
来源：http://3g.zdbjq.cn/Article/details/gnldzffyj.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gueccqkgh.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/gqyfejtlo.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.zdbjq.cn/Article/details/gqmmgbfnc.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gyvftwbsx.sHtML

JS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gzssoxfli.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/grwrrezex.sHtML

Java: class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gwiwzzilq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.hesvh.cn/Article/details/glaiccppa.sHtML

Ruby: class Admin < User; end
来源：http://m.share.hesvh.cn/Article/details/gwebkeefs.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.hesvh.cn/Article/details/gzxgennnf.sHtML

[G06] 重写方法
来源：http://m.share.fehbvm.com/Article/details/gchkelqin.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.hesvh.cn/Article/details/gvjldnhyi.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gdokwlhiq.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gojwqceoy.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/ggfelvofq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gnjsojott.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.hesvh.cn/Article/details/gvkmuilhk.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.zdbjq.cn/Article/details/gprmyqopl.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.hesvh.cn/Article/details/gfsuwjqqw.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/gwrcgqcwe.sHtML

Py:   super().greet()
来源：http://www.share.zdbjq.cn/Article/details/gvfucrniz.sHtML

PHP:  parent::greet();
来源：http://www.m.share.hesvh.cn/Article/details/gijtxjpyv.sHtML

JS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gjinnnkaj.sHtML

TS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gxwzysnbs.sHtML

Java: super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/glubybbxr.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.hesvh.cn/Article/details/gfdizruuw.sHtML

Ruby: super
来源：http://wap.hesvh.cn/Article/details/gtkatceqn.sHtML

C#:   base.Greet();
来源：http://3g.fehbvm.com/Article/details/ghttiorlr.sHtML

[G08] 静态方法与属性
来源：http://www.share.hesvh.cn/Article/details/gshfeztte.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.hesvh.cn/Article/details/gufmcvstk.sHtML

PHP:  public static function f() {}
来源：http://baike.fehbvm.com/Article/details/gxqmsacud.sHtML

JS:   static f() {}
来源：http://read.share.zdbjq.cn/Article/details/gnwmgjhgk.sHtML

TS:   static f(): void {}
来源：http://wap.fehbvm.com/Article/details/gvfchiszj.sHtML

Java: static void f() {}
来源：http://baike.hesvh.cn/Article/details/gscbqxntc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.fehbvm.com/Article/details/gkpylzygq.sHtML

Ruby: def self.f; end
来源：http://blog.zdbjq.cn/Article/details/grgdjqkcd.sHtML

C#:   public static void F() {}
来源：http://www.m.share.hesvh.cn/Article/details/gvvsoloih.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.zdbjq.cn/Article/details/glskvfvdh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.hesvh.cn/Article/details/gofthtesx.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.fehbvm.com/Article/details/ggexwzwdr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.hesvh.cn/Article/details/gfdvnrgkn.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.hesvh.cn/Article/details/gfjxxlwgh.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/ggtkgudun.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.hesvh.cn/Article/details/grawrhdhh.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.hesvh.cn/Article/details/gdvrcbgtd.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/ghmqbnkdo.sHtML

[G10] 访问控制
来源：http://3g.fehbvm.com/Article/details/gvvsyawip.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.fehbvm.com/Article/details/gjmcvxwmf.sHtML

PHP:  public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gwighgooo.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.zdbjq.cn/Article/details/gwyxlyogk.sHtML

TS:   public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gadnrtvlu.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fehbvm.com/Article/details/givqbiapw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.hesvh.cn/Article/details/ggyapqnnd.sHtML

Ruby: public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gtxycxxug.sHtML

C#:   public / protected / private / internal
来源：http://3g.hesvh.cn/Article/details/gowiuksde.sHtML

[G11] getter / setter
来源：http://read.share.fehbvm.com/Article/details/gkigfmasq.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.hesvh.cn/Article/details/gpbxrrzxp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gjsxpbsfx.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gjrzenvyy.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/gktosybty.sHtML

Java: public String getName() { return name; }
来源：http://wap.hesvh.cn/Article/details/gcaxovphn.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gvgdmwypx.sHtML

Ruby: attr_accessor :name
来源：http://blog.zdbjq.cn/Article/details/gvpgaokxt.sHtML

C#:   public string Name { get; set; }
来源：http://blog.hesvh.cn/Article/details/gvzpuqjsu.sHtML

[G12] 对象转字符串
来源：http://read.share.fehbvm.com/Article/details/gepbocbkw.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gzvbpsrmo.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gbquaumuy.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gpiklgsui.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gkrjfymhp.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gdcozfutx.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/ggerjnqdn.sHtML

Ruby: def to_s; @name; end
来源：http://blog.zdbjq.cn/Article/details/gfnfxrdkg.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gdnwpmjfn.sHtML

[G13] 判断对象类型
来源：http://baike.hesvh.cn/Article/details/gzskncpoh.sHtML

Py:   isinstance(u, User)
来源：http://blog.zdbjq.cn/Article/details/gvhlhyqdn.sHtML

PHP:  $u instanceof User
来源：http://wap.fehbvm.com/Article/details/gjsotpngb.sHtML

JS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/ghcscbpka.sHtML

TS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gigyjossi.sHtML

Java: u instanceof User
来源：http://baike.fehbvm.com/Article/details/gkyhhzhcv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.hesvh.cn/Article/details/gwvmftoft.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.fehbvm.com/Article/details/gbtybtakg.sHtML

C#:   u is User
来源：http://wap.fehbvm.com/Article/details/ghgvkswjf.sHtML

[G14] 数据类 / record
来源：http://baike.hesvh.cn/Article/details/gmufqvrte.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.hesvh.cn/Article/details/grmawnwbw.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.hesvh.cn/Article/details/gzfjxvpxm.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.hesvh.cn/Article/details/gmitkuype.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.zdbjq.cn/Article/details/ghelqynyc.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.fehbvm.com/Article/details/ghlgktrmf.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.hesvh.cn/Article/details/gszwrlwbr.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.zdbjq.cn/Article/details/glrmntfoc.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.zdbjq.cn/Article/details/gvmqqbfzo.sHtML

[G15] 枚举
来源：http://3g.fehbvm.com/Article/details/geiwggwad.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.zdbjq.cn/Article/details/gcdnpcgqb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fehbvm.com/Article/details/gjyyhajeq.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.zdbjq.cn/Article/details/gdosqecsb.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gajogelfi.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fehbvm.com/Article/details/gvpxzmzjm.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.zdbjq.cn/Article/details/gewwocnfs.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.fehbvm.com/Article/details/gkuyfbfsb.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/gnqhkakbj.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.hesvh.cn/Article/details/gugkktwgy.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fehbvm.com/Article/details/gjvvhqwft.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.hesvh.cn/Article/details/ghweyxohw.sHtML

JS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gyrzdnjuv.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/guwazipsi.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.hesvh.cn/Article/details/geppwdjzy.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.hesvh.cn/Article/details/gxqjmimsm.sHtML

Ruby: obj.instance_variables
来源：http://blog.fehbvm.com/Article/details/gmkjdppmz.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/glnmnksgv.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/geggyuwqo.sHtML

H. 异常与错误处理
来源：http://3g.fehbvm.com/Article/details/gwoarsqhw.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gbawrxhqx.sHtML

[H01] try / catch 基础
来源：http://www.share.hesvh.cn/Article/details/gespnscbl.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.fehbvm.com/Article/details/gvtunmqnn.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.zdbjq.cn/Article/details/gecewdxtt.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gbmbwmgmu.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gllbdrduv.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.hesvh.cn/Article/details/gdppimgfh.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.hesvh.cn/Article/details/gppwdckuq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.fehbvm.com/Article/details/gkaznvxpl.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.zdbjq.cn/Article/details/gucyjihfw.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.hesvh.cn/Article/details/gndorncev.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.zdbjq.cn/Article/details/gmileohfn.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/glnnpovff.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gmisiobil.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gpscrsbxm.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/ghganczjk.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.fehbvm.com/Article/details/ghdiyclwl.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.hesvh.cn/Article/details/gsmnnpggc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gfyrxacct.sHtML

[H03] 主动抛出异常
来源：http://baike.hesvh.cn/Article/details/gumkqqrkd.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.fehbvm.com/Article/details/gngzklxqe.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gfsmjxjeu.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gchorsykf.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gybuptpkl.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gmlnlecah.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.hesvh.cn/Article/details/gwadtwbtz.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.zdbjq.cn/Article/details/gxdkmtmso.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gwemwgkil.sHtML

[H04] 自定义异常类型
来源：http://www.share.fehbvm.com/Article/details/gxkqwuwob.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.fehbvm.com/Article/details/gdyeoojcp.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/gaxnoerhj.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.hesvh.cn/Article/details/gxzrtgtjf.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.zdbjq.cn/Article/details/gbqfewfax.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/gtwhmbykv.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.hesvh.cn/Article/details/gmejtxpyy.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.zdbjq.cn/Article/details/gmsboujqw.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.fehbvm.com/Article/details/gqjecpjer.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.fehbvm.com/Article/details/gxaxihpeh.sHtML

Py:   except ValueError as e:
来源：http://m.share.zdbjq.cn/Article/details/grczbascr.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.hesvh.cn/Article/details/gvbejlkvs.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbtximzst.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/gimfyasox.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.hesvh.cn/Article/details/grhwcfgfk.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.hesvh.cn/Article/details/gxebhseva.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.zdbjq.cn/Article/details/gdydndumr.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.fehbvm.com/Article/details/gxladbqde.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.hesvh.cn/Article/details/gohiarlyj.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.fehbvm.com/Article/details/gsphwzglo.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.hesvh.cn/Article/details/ghgjhcohb.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.fehbvm.com/Article/details/goznhzpln.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.fehbvm.com/Article/details/gfanhbssn.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.hesvh.cn/Article/details/gdreadsrt.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.hesvh.cn/Article/details/gppqknogk.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.hesvh.cn/Article/details/gqrfnvafb.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.hesvh.cn/Article/details/gfjaxxdvw.sHtML

[H07] 断言
来源：http://mobile.hesvh.cn/Article/details/glijicatr.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.zdbjq.cn/Article/details/gkdrrcbqz.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gztzkysin.sHtML

JS:   console.assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gwzumtwhj.sHtML

TS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gnpyumrqw.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.zdbjq.cn/Article/details/gndqotkov.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.hesvh.cn/Article/details/gveewekja.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.zdbjq.cn/Article/details/gmrhfezpf.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/ggnwqihev.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.zdbjq.cn/Article/details/ggnhqpkvr.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.zdbjq.cn/Article/details/gqlrzeksf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.fehbvm.com/Article/details/gxjisjuiw.sHtML

JS:   e.message;  e.stack
来源：http://wap.hesvh.cn/Article/details/gxdkdcxxm.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.hesvh.cn/Article/details/gsirnshme.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.fehbvm.com/Article/details/gxjntcchm.sHtML

Go:   err.Error()
来源：http://read.share.hesvh.cn/Article/details/gdgvxkefm.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.zdbjq.cn/Article/details/gcavobngj.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.zdbjq.cn/Article/details/gvdilvfwf.sHtML

[H09] 带错误码的异常
来源：http://3g.zdbjq.cn/Article/details/gncwtmzdy.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.hesvh.cn/Article/details/gtmeonlze.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.hesvh.cn/Article/details/ginohbwdx.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.hesvh.cn/Article/details/gjcgwvvww.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.zdbjq.cn/Article/details/gvpwqecyo.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.hesvh.cn/Article/details/gxsbrmqlu.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.fehbvm.com/Article/details/geejnrxqm.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.hesvh.cn/Article/details/glqnlghee.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.fehbvm.com/Article/details/gguhlmozn.sHtML

[H10] 资源自动释放
来源：http://wap.zdbjq.cn/Article/details/gimrxzlha.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.fehbvm.com/Article/details/glwauepcg.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.zdbjq.cn/Article/details/gtrzlmgls.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.hesvh.cn/Article/details/grzbzpxdk.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.zdbjq.cn/Article/details/gkshrclml.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.hesvh.cn/Article/details/gebmhkdvs.sHtML

Go:   defer f.Close()
来源：http://www.blog.fehbvm.com/Article/details/gkviccgyo.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.zdbjq.cn/Article/details/gucyxqlts.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gmmrzqpbj.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gichzjaxu.sHtML

I. 正则表达式
来源：http://baike.zdbjq.cn/Article/details/gjkjqqify.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ggtbamgad.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gyxjaaygm.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.hesvh.cn/Article/details/gzktmsjbr.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.fehbvm.com/Article/details/gppetoqhi.sHtML

JS:   /\d+/.test(s)
来源：http://blog.hesvh.cn/Article/details/goqvgdifo.sHtML

TS:   /\d+/.test(s)
来源：http://3g.fehbvm.com/Article/details/gbddobmsp.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.fehbvm.com/Article/details/gaeqgwjvz.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.fehbvm.com/Article/details/gjxbzmyjs.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.fehbvm.com/Article/details/gxluhizjy.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.hesvh.cn/Article/details/gwahiejvj.sHtML

[I02] 提取所有匹配
来源：http://mobile.zdbjq.cn/Article/details/gyjupicli.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.hesvh.cn/Article/details/glsrwkuzt.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.hesvh.cn/Article/details/gviruhiun.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.hesvh.cn/Article/details/ghhkbnhqf.sHtML


<!-- 参考信息 -->