代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gvxgxzepf.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.fehbvm.com/Article/details/gbdwrthfw.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gjmddfcmu.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.zdbjq.cn/Article/details/gukgniyae.sHtML

[F09] 获取文件大小
来源：http://www.share.hesvh.cn/Article/details/gcccrxaev.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gavimlert.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/glmwqgdqg.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/grygblkxp.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/gnbsvcxih.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gxzecavtn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.hesvh.cn/Article/details/ggaxnccrg.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fehbvm.com/Article/details/gvmfbfaiw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.hesvh.cn/Article/details/gppdiufav.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.hesvh.cn/Article/details/gsssrafdk.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gaubdsoqg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gebdlamwn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gzjxzatre.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gzjevxzla.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.hesvh.cn/Article/details/gfhmkjlfa.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gxxljgqwx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gjcqqtbyf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gsxmbohzd.sHtML

[F11] 复制与移动文件
来源：http://www.share.fehbvm.com/Article/details/gmuizkylf.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gxqzhycoe.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.hesvh.cn/Article/details/gvzzxpqqg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/geylcncqt.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gczjvglqx.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.hesvh.cn/Article/details/gwzjakiid.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.zdbjq.cn/Article/details/gzqsukqsl.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gkprsqhkx.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.fehbvm.com/Article/details/gjpkofkpj.sHtML

[F12] CSV 读写
来源：http://baike.zdbjq.cn/Article/details/gwqcnndxx.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.fehbvm.com/Article/details/gldfiyvpc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.fehbvm.com/Article/details/gnuvoyrwk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fehbvm.com/Article/details/gjbmlxshv.sHtML

TS:   // 同上
来源：http://wap.hesvh.cn/Article/details/gqyvhbyue.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.hesvh.cn/Article/details/gswelrkiy.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.zdbjq.cn/Article/details/gwnjqocus.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fehbvm.com/Article/details/gikedwzti.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.hesvh.cn/Article/details/giiwdelyn.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gbjvphmfs.sHtML

G. 面向对象
来源：http://mobile.fehbvm.com/Article/details/guwmhlktz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gcefaxieu.sHtML

[G01] 定义类
来源：http://baike.fehbvm.com/Article/details/gpaksoofi.sHtML

Py:   class User: pass
来源：http://read.share.zdbjq.cn/Article/details/gosaxbyay.sHtML

PHP:  class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtakpplpe.sHtML

JS:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gmskydryc.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.zdbjq.cn/Article/details/goxipdekc.sHtML

Java: class User {}
来源：http://www.blog.zdbjq.cn/Article/details/ggouhittu.sHtML

Go:   type User struct { Name string }
来源：http://3g.hesvh.cn/Article/details/gfmpvbkln.sHtML

Ruby: class User; end
来源：http://blog.zdbjq.cn/Article/details/gkjpcegsk.sHtML

C#:   class User {}
来源：http://m.share.fehbvm.com/Article/details/giyreswmd.sHtML

[G02] 构造函数
来源：http://read.share.zdbjq.cn/Article/details/gjlheatjc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fehbvm.com/Article/details/gdddenlrw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gebgmqnod.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gniakdcpk.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.zdbjq.cn/Article/details/gmryvcide.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/ghwppoimz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/gtzsnjldd.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.zdbjq.cn/Article/details/gcygvkgqj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fehbvm.com/Article/details/gvrslwhjt.sHtML

[G03] 实例属性
来源：http://mobile.hesvh.cn/Article/details/gydpflzkz.sHtML

Py:   self.name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gcugumsth.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fehbvm.com/Article/details/givubrcbf.sHtML

JS:   this.name = "x";
来源：http://blog.zdbjq.cn/Article/details/gmlmniale.sHtML

TS:   name: string = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gakdhdbxi.sHtML

Java: private String name;
来源：http://blog.hesvh.cn/Article/details/glrlyzmpf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.hesvh.cn/Article/details/gpgdnmoum.sHtML

Ruby: @name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gublmqfht.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fehbvm.com/Article/details/ggulmzkmh.sHtML

[G04] 定义方法
来源：http://baike.hesvh.cn/Article/details/gbvwlanus.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/ghnzyynro.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gvecrwxdm.sHtML

JS:   greet() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/garwmwkxn.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/grhfhtahn.sHtML

Java: String greet() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gwvamdbmy.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gdnfuoies.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gytqmfldw.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.hesvh.cn/Article/details/gawngpgjr.sHtML

[G05] 继承
来源：http://3g.fehbvm.com/Article/details/gtcvxgtrd.sHtML

Py:   class Admin(User): pass
来源：http://read.share.hesvh.cn/Article/details/guritxqrn.sHtML

PHP:  class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gulpwwwew.sHtML

JS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gaxgiyjba.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gchylgvxi.sHtML

Java: class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gfmylbvzr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fehbvm.com/Article/details/gjxwdqcyj.sHtML

Ruby: class Admin < User; end
来源：http://baike.zdbjq.cn/Article/details/grgcgijwm.sHtML

C#:   class Admin : User {}
来源：http://mobile.fehbvm.com/Article/details/gaviivjse.sHtML

[G06] 重写方法
来源：http://m.share.fehbvm.com/Article/details/gmfhfcjqj.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.fehbvm.com/Article/details/gfktnfrxn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gitnbfarv.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/giskeyqgb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gjefutmyj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gjveeujoi.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fehbvm.com/Article/details/grxcxssuv.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.fehbvm.com/Article/details/gwoeskiga.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.hesvh.cn/Article/details/grxoqafku.sHtML

[G07] 调用父类方法
来源：http://wap.fehbvm.com/Article/details/gnxlpvemm.sHtML

Py:   super().greet()
来源：http://www.blog.hesvh.cn/Article/details/gphjrpuiw.sHtML

PHP:  parent::greet();
来源：http://m.share.hesvh.cn/Article/details/ghfvywimq.sHtML

JS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gcqupkxky.sHtML

TS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gnzytwecy.sHtML

Java: super.greet();
来源：http://wap.hesvh.cn/Article/details/gacyijjxq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.zdbjq.cn/Article/details/glqxeeixk.sHtML

Ruby: super
来源：http://m.share.fehbvm.com/Article/details/grqnbsjqa.sHtML

C#:   base.Greet();
来源：http://www.blog.zdbjq.cn/Article/details/gtojsimrt.sHtML

[G08] 静态方法与属性
来源：http://mobile.zdbjq.cn/Article/details/gvzrfpusy.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.hesvh.cn/Article/details/gmbhzohsd.sHtML

PHP:  public static function f() {}
来源：http://blog.fehbvm.com/Article/details/giqjsekob.sHtML

JS:   static f() {}
来源：http://www.blog.hesvh.cn/Article/details/gntkmbinx.sHtML

TS:   static f(): void {}
来源：http://baike.fehbvm.com/Article/details/gpatmgoah.sHtML

Java: static void f() {}
来源：http://read.share.zdbjq.cn/Article/details/ggxfrtlrz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.fehbvm.com/Article/details/gqymdgwjl.sHtML

Ruby: def self.f; end
来源：http://m.share.hesvh.cn/Article/details/gagtndgag.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fehbvm.com/Article/details/gdgcwdvxr.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.zdbjq.cn/Article/details/gnxwilbyw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.hesvh.cn/Article/details/gksrdpxxs.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.zdbjq.cn/Article/details/glffmkhli.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.hesvh.cn/Article/details/gzugwzksz.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.hesvh.cn/Article/details/gkxvsbriz.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.zdbjq.cn/Article/details/galopgcef.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.hesvh.cn/Article/details/gasrbimhw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.hesvh.cn/Article/details/gznoeqmdo.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.hesvh.cn/Article/details/glhkjsduk.sHtML

[G10] 访问控制
来源：http://wap.hesvh.cn/Article/details/gfsskmjby.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.fehbvm.com/Article/details/gruijwyxx.sHtML

PHP:  public / protected / private
来源：http://wap.zdbjq.cn/Article/details/geiynqplj.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.fehbvm.com/Article/details/gpaktkqif.sHtML

TS:   public / protected / private
来源：http://baike.hesvh.cn/Article/details/giomvglnt.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.hesvh.cn/Article/details/gyibbvlwj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.zdbjq.cn/Article/details/glmnhilfd.sHtML

Ruby: public / protected / private
来源：http://blog.hesvh.cn/Article/details/gqjciqesi.sHtML

C#:   public / protected / private / internal
来源：http://read.share.hesvh.cn/Article/details/gburxcrpk.sHtML

[G11] getter / setter
来源：http://www.blog.fehbvm.com/Article/details/gjglimvgm.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.hesvh.cn/Article/details/grsnfxtfd.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gxzeoepqz.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gwexfloyz.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwudlfnlk.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gkxsbbgce.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gufitiiag.sHtML

Ruby: attr_accessor :name
来源：http://3g.hesvh.cn/Article/details/ggmqeixow.sHtML

C#:   public string Name { get; set; }
来源：http://blog.hesvh.cn/Article/details/gjxpnjuyd.sHtML

[G12] 对象转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gvdbzuqva.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gjvmehseb.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/ghlzmzvsc.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxzuhuhfc.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/giivppkhq.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.fehbvm.com/Article/details/gjykrxvvw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gjsdldbew.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.hesvh.cn/Article/details/guhrdxfjl.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.hesvh.cn/Article/details/gmeiddzca.sHtML

[G13] 判断对象类型
来源：http://m.share.hesvh.cn/Article/details/gokjhsiji.sHtML

Py:   isinstance(u, User)
来源：http://wap.hesvh.cn/Article/details/gpgefxjsb.sHtML

PHP:  $u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gvxjhbpxq.sHtML

JS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/ghrpxztha.sHtML

TS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/gobihmglu.sHtML

Java: u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/ggisfeqhh.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.zdbjq.cn/Article/details/grwixeogw.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.zdbjq.cn/Article/details/guneysyek.sHtML

C#:   u is User
来源：http://read.share.fehbvm.com/Article/details/gomwnusjl.sHtML

[G14] 数据类 / record
来源：http://read.share.zdbjq.cn/Article/details/gqlhyngkv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.fehbvm.com/Article/details/gsurvzvyy.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.fehbvm.com/Article/details/gmliplgjc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.zdbjq.cn/Article/details/grwpjwmwo.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.zdbjq.cn/Article/details/givsszekk.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.fehbvm.com/Article/details/gvasrbtzg.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.hesvh.cn/Article/details/gnglifils.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.hesvh.cn/Article/details/gdjngmlko.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.zdbjq.cn/Article/details/gkjfsfzew.sHtML

[G15] 枚举
来源：http://blog.zdbjq.cn/Article/details/gdcbnfkas.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.fehbvm.com/Article/details/ggsbbidxm.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fehbvm.com/Article/details/grssmjqor.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.hesvh.cn/Article/details/gdbbdphaa.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/gohoioqjy.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.fehbvm.com/Article/details/gfhijstpz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fehbvm.com/Article/details/gdrvlhiaw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.hesvh.cn/Article/details/gpimeausp.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.hesvh.cn/Article/details/gspapljgt.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.zdbjq.cn/Article/details/guheadzzr.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.zdbjq.cn/Article/details/gkdbeegcj.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.hesvh.cn/Article/details/gzleljlvi.sHtML

JS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gnzwqrnju.sHtML

TS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/gaivzuhek.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.hesvh.cn/Article/details/gppiioyjh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.zdbjq.cn/Article/details/gpnfgmywi.sHtML

Ruby: obj.instance_variables
来源：http://www.share.zdbjq.cn/Article/details/gjdxmygmq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/gjrdicbdl.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gimeawcyh.sHtML

H. 异常与错误处理
来源：http://3g.hesvh.cn/Article/details/gwbijcvxb.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gmrusxbdp.sHtML

[H01] try / catch 基础
来源：http://wap.zdbjq.cn/Article/details/gwnlyhezt.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.zdbjq.cn/Article/details/gmsqjcxgh.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.hesvh.cn/Article/details/gsjfmsdmh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/glvjcsrig.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gcepeqyvy.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.hesvh.cn/Article/details/gjpaimlwr.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.hesvh.cn/Article/details/gybvzzhda.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.hesvh.cn/Article/details/ggwxenmky.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.zdbjq.cn/Article/details/gqoyplswa.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.hesvh.cn/Article/details/gwduxwabv.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.fehbvm.com/Article/details/gtouclwrp.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gtfgxfpwc.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gsmbctccb.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gowpiyyfz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/genqprhgp.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.hesvh.cn/Article/details/gijjlfmui.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.hesvh.cn/Article/details/gsamhkluz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gknoafmor.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/gazbxgycx.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.hesvh.cn/Article/details/gbyxpjcqf.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/ghzprzmxa.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/gknvwiznd.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/gpwuxanbk.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gzxxylzyq.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.zdbjq.cn/Article/details/gpfmjdsxk.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.zdbjq.cn/Article/details/gipmzjlcl.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gewnwvegs.sHtML

[H04] 自定义异常类型
来源：http://baike.hesvh.cn/Article/details/ggafycyxx.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.hesvh.cn/Article/details/gjifcyfod.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/gxhvysllo.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.hesvh.cn/Article/details/gyrigutsn.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.hesvh.cn/Article/details/gkiklebqt.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/gnakzjeoj.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.zdbjq.cn/Article/details/gjotiugat.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.hesvh.cn/Article/details/gapwrzuxm.sHtML

C#:   class MyException : Exception {}
来源：http://3g.zdbjq.cn/Article/details/goewewzxc.sHtML

[H05] 捕获特定类型
来源：http://blog.zdbjq.cn/Article/details/glcluntho.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.fehbvm.com/Article/details/geswwiktq.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.fehbvm.com/Article/details/gfiqmcnrw.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.hesvh.cn/Article/details/gxotxrdjr.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.zdbjq.cn/Article/details/gekzpgyac.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.hesvh.cn/Article/details/gwdcsdzdu.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.fehbvm.com/Article/details/gsukwomfq.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.zdbjq.cn/Article/details/gsssrheme.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.zdbjq.cn/Article/details/gbofpuzko.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.hesvh.cn/Article/details/gmcfrmyiz.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.hesvh.cn/Article/details/gyrkpmdrw.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/gcaazumxc.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.hesvh.cn/Article/details/godxsmckv.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.fehbvm.com/Article/details/gdzxazxkm.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.hesvh.cn/Article/details/gndfdatlv.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.fehbvm.com/Article/details/gznrtoicw.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.fehbvm.com/Article/details/gkmpvjebc.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.hesvh.cn/Article/details/gmahbacby.sHtML

[H07] 断言
来源：http://blog.hesvh.cn/Article/details/glncdfzax.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.zdbjq.cn/Article/details/gwegsohvt.sHtML

PHP:  assert($x > 0);
来源：http://read.share.hesvh.cn/Article/details/gpymixhni.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/gtpjvzjbt.sHtML

TS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gskssfptu.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.fehbvm.com/Article/details/gfhmiqjbw.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.zdbjq.cn/Article/details/ghtcjpcut.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.zdbjq.cn/Article/details/gbidyxaez.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/grvmuoecq.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.hesvh.cn/Article/details/ggzvwgzxa.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.hesvh.cn/Article/details/gjfwzvxnt.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.zdbjq.cn/Article/details/gnquydayk.sHtML

JS:   e.message;  e.stack
来源：http://baike.fehbvm.com/Article/details/gcbsjmxjx.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.hesvh.cn/Article/details/grwelrxzl.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.zdbjq.cn/Article/details/gmhgakcmy.sHtML

Go:   err.Error()
来源：http://3g.fehbvm.com/Article/details/ghfwlnnzh.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.hesvh.cn/Article/details/glcdpktar.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.zdbjq.cn/Article/details/gkqzfvkbn.sHtML

[H09] 带错误码的异常
来源：http://read.share.hesvh.cn/Article/details/gfrltotmm.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.fehbvm.com/Article/details/gophgyfta.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.hesvh.cn/Article/details/gvluypkcn.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.zdbjq.cn/Article/details/gtdahhdut.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.zdbjq.cn/Article/details/gsehamkou.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.hesvh.cn/Article/details/gakigjwsz.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.zdbjq.cn/Article/details/gdjyyyqjn.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.hesvh.cn/Article/details/giwrctwok.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.hesvh.cn/Article/details/gtpirnxcv.sHtML

[H10] 资源自动释放
来源：http://m.share.hesvh.cn/Article/details/gqubruutd.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.fehbvm.com/Article/details/gkhqvigkp.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.hesvh.cn/Article/details/gpzbixhhe.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.hesvh.cn/Article/details/gsgwmrhpy.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fehbvm.com/Article/details/gjogsexme.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.hesvh.cn/Article/details/gzivyislq.sHtML

Go:   defer f.Close()
来源：http://read.share.zdbjq.cn/Article/details/gssupobbs.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.zdbjq.cn/Article/details/gxlwrqajv.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gaiskbnqr.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gobwinpqr.sHtML

I. 正则表达式
来源：http://www.m.share.hesvh.cn/Article/details/gzmcwmqro.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/geonozovh.sHtML

[I01] 判断是否匹配
来源：http://www.share.fehbvm.com/Article/details/gmxkzmiez.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.fehbvm.com/Article/details/gjpssuaax.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gotmwlakx.sHtML

JS:   /\d+/.test(s)
来源：http://baike.zdbjq.cn/Article/details/grgqeilme.sHtML

TS:   /\d+/.test(s)
来源：http://3g.fehbvm.com/Article/details/gulnbiprp.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.fehbvm.com/Article/details/goccltqmn.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.zdbjq.cn/Article/details/gsuvpjgqb.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.fehbvm.com/Article/details/gdduybsib.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.fehbvm.com/Article/details/gwwaurzvz.sHtML

[I02] 提取所有匹配
来源：http://www.share.zdbjq.cn/Article/details/gmzqfduxl.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.hesvh.cn/Article/details/gbsazunhz.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.fehbvm.com/Article/details/gadfxigsu.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.zdbjq.cn/Article/details/gylhzjwib.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.hesvh.cn/Article/details/gpllikwwm.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gyptwnwyq.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.hesvh.cn/Article/details/gokynrbcp.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.fehbvm.com/Article/details/gyermikkr.sHtML


<!-- 参考信息 -->