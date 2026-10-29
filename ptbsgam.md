代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.hesvh.cn/Article/details/gszbagdff.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.hesvh.cn/Article/details/gjszvlrjr.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gdrqhozfr.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gmtifxawz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/gufaoisln.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.zdbjq.cn/Article/details/gcsplqbvv.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.zdbjq.cn/Article/details/gsinhzvja.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.zdbjq.cn/Article/details/ggksuayab.sHtML

[F09] 获取文件大小
来源：http://www.blog.hesvh.cn/Article/details/gkzbxawvh.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gkoabrgiv.sHtML

PHP:  filesize("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gugvdrliz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/gjuneqggy.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/gjqcbbeqw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gosnupeon.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.zdbjq.cn/Article/details/gwdchnohj.sHtML

Ruby: File.size("a.txt")
来源：http://baike.fehbvm.com/Article/details/gkieuejqi.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.fehbvm.com/Article/details/gqttowjzm.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.zdbjq.cn/Article/details/grrzauuom.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gpcbpysdr.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gxkekmgzo.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gjrboancu.sHtML

TS:   path.extname("a.txt")
来源：http://blog.fehbvm.com/Article/details/gssuuwfcn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.zdbjq.cn/Article/details/gcnsdhvak.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gsoxaoaue.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/ghtuifzjs.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gormhfuys.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.hesvh.cn/Article/details/gzxpnulpn.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gfyqsmxde.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.zdbjq.cn/Article/details/gpjjazhdn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gdycbhrgl.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gagsspvnn.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gerosafpj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.hesvh.cn/Article/details/gpukzorqn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gzgfkpwel.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.zdbjq.cn/Article/details/gzzzjyweh.sHtML

[F12] CSV 读写
来源：http://wap.zdbjq.cn/Article/details/gpsgbckyd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.zdbjq.cn/Article/details/gidrfafts.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.hesvh.cn/Article/details/gsprdlyqq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.zdbjq.cn/Article/details/ggbaelzuy.sHtML

TS:   // 同上
来源：http://mobile.zdbjq.cn/Article/details/gxcsdjmlq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fehbvm.com/Article/details/gyczqlasu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.fehbvm.com/Article/details/ghrftmrhp.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fehbvm.com/Article/details/ghyrdvsux.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.zdbjq.cn/Article/details/gnyruaoqz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gycouybly.sHtML

G. 面向对象
来源：http://www.m.share.fehbvm.com/Article/details/giwrrjsrf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gperljtzk.sHtML

[G01] 定义类
来源：http://www.m.share.fehbvm.com/Article/details/gwinxqhud.sHtML

Py:   class User: pass
来源：http://wap.fehbvm.com/Article/details/gsbjyetpe.sHtML

PHP:  class User {}
来源：http://baike.hesvh.cn/Article/details/gluswjlhd.sHtML

JS:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gytehbuzl.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.fehbvm.com/Article/details/gkdieeznc.sHtML

Java: class User {}
来源：http://wap.fehbvm.com/Article/details/glvjnjzmk.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/gnztztuek.sHtML

Ruby: class User; end
来源：http://baike.hesvh.cn/Article/details/gpeopejzc.sHtML

C#:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gzvcjuldt.sHtML

[G02] 构造函数
来源：http://blog.hesvh.cn/Article/details/ggauzoxho.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.zdbjq.cn/Article/details/gqxvajadi.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.zdbjq.cn/Article/details/ghhedfhwq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gswsilqsf.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.hesvh.cn/Article/details/gfgnyfies.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gbqwsuiln.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.fehbvm.com/Article/details/gypdzibgy.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fehbvm.com/Article/details/gnsoormge.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gvnjkvmem.sHtML

[G03] 实例属性
来源：http://wap.fehbvm.com/Article/details/gjznfvkhw.sHtML

Py:   self.name = "x"
来源：http://blog.fehbvm.com/Article/details/gamxfqoze.sHtML

PHP:  public string $name = "x";
来源：http://wap.zdbjq.cn/Article/details/gvbfgaoaf.sHtML

JS:   this.name = "x";
来源：http://www.blog.hesvh.cn/Article/details/glbeqwrgq.sHtML

TS:   name: string = "x";
来源：http://baike.hesvh.cn/Article/details/gtytclhfp.sHtML

Java: private String name;
来源：http://baike.hesvh.cn/Article/details/gjyylnmeq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.hesvh.cn/Article/details/gjvkgikvf.sHtML

Ruby: @name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gwtbwjjcx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.fehbvm.com/Article/details/gupjngale.sHtML

[G04] 定义方法
来源：http://wap.zdbjq.cn/Article/details/gduobuyut.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gntgisykp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gjrseahwg.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gsatgjccz.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gnlbmlgvz.sHtML

Java: String greet() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/grtnguodz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gnnunsexo.sHtML

Ruby: def greet; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gjfdewwdq.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gaufudeby.sHtML

[G05] 继承
来源：http://3g.hesvh.cn/Article/details/gmkmzqqdp.sHtML

Py:   class Admin(User): pass
来源：http://read.share.zdbjq.cn/Article/details/gaivndbrg.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvjcpaycm.sHtML

JS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gpcflgond.sHtML

TS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/giqjwicws.sHtML

Java: class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gctumiuup.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.zdbjq.cn/Article/details/glulscxfh.sHtML

Ruby: class Admin < User; end
来源：http://3g.hesvh.cn/Article/details/gsdambqwf.sHtML

C#:   class Admin : User {}
来源：http://blog.zdbjq.cn/Article/details/gwildbzty.sHtML

[G06] 重写方法
来源：http://www.m.share.hesvh.cn/Article/details/gaseqczem.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.hesvh.cn/Article/details/gssuxhpik.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gctwuelzl.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gfhemugbw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gzshbhtfu.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/ggxnzsnvy.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fehbvm.com/Article/details/gzarbuuec.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.fehbvm.com/Article/details/gkdmfwdxh.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.zdbjq.cn/Article/details/gozbuwdcq.sHtML

[G07] 调用父类方法
来源：http://baike.zdbjq.cn/Article/details/guvnspypc.sHtML

Py:   super().greet()
来源：http://baike.fehbvm.com/Article/details/guamoujmc.sHtML

PHP:  parent::greet();
来源：http://www.share.fehbvm.com/Article/details/gbfawwldg.sHtML

JS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gisdntqtf.sHtML

TS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gvofbcneu.sHtML

Java: super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gtrnelpud.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.zdbjq.cn/Article/details/gfaknpoha.sHtML

Ruby: super
来源：http://www.share.hesvh.cn/Article/details/gkjmogxpi.sHtML

C#:   base.Greet();
来源：http://mobile.fehbvm.com/Article/details/ggwyplxhx.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.zdbjq.cn/Article/details/gboygktfr.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fehbvm.com/Article/details/gboykejvs.sHtML

PHP:  public static function f() {}
来源：http://mobile.zdbjq.cn/Article/details/gwovjxzhb.sHtML

JS:   static f() {}
来源：http://blog.hesvh.cn/Article/details/gdwnestin.sHtML

TS:   static f(): void {}
来源：http://baike.fehbvm.com/Article/details/githokdeh.sHtML

Java: static void f() {}
来源：http://www.share.zdbjq.cn/Article/details/gkbdartan.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.fehbvm.com/Article/details/gxakiuvpi.sHtML

Ruby: def self.f; end
来源：http://www.blog.zdbjq.cn/Article/details/geiklcjcc.sHtML

C#:   public static void F() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjdhnrotz.sHtML

[G09] 接口 / 抽象类
来源：http://baike.hesvh.cn/Article/details/guyvfluqp.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.zdbjq.cn/Article/details/grzyvkvjy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.zdbjq.cn/Article/details/glexnduxp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.hesvh.cn/Article/details/gxzyupveo.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.zdbjq.cn/Article/details/ginsckxvr.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.fehbvm.com/Article/details/gtfmnzojq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fehbvm.com/Article/details/gibvnbqxk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.hesvh.cn/Article/details/gichabjbb.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fehbvm.com/Article/details/ghsokpdge.sHtML

[G10] 访问控制
来源：http://read.share.fehbvm.com/Article/details/gaftsxktl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.hesvh.cn/Article/details/gdjvgoaxy.sHtML

PHP:  public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gpcaqxxeo.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.fehbvm.com/Article/details/gfqstbnwk.sHtML

TS:   public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gldpsmshp.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fehbvm.com/Article/details/gmhkdzlvc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fehbvm.com/Article/details/gdycdotrp.sHtML

Ruby: public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gotiqwurc.sHtML

C#:   public / protected / private / internal
来源：http://www.share.zdbjq.cn/Article/details/ghvwmqkss.sHtML

[G11] getter / setter
来源：http://m.share.fehbvm.com/Article/details/gnbbtsthj.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.fehbvm.com/Article/details/gaqejhrwu.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gfehxdbqi.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/gflznkjls.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gqiebqrca.sHtML

Java: public String getName() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gayysvorm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gzbbqccrn.sHtML

Ruby: attr_accessor :name
来源：http://www.share.zdbjq.cn/Article/details/guixuvkoz.sHtML

C#:   public string Name { get; set; }
来源：http://blog.zdbjq.cn/Article/details/goeohqodc.sHtML

[G12] 对象转字符串
来源：http://wap.zdbjq.cn/Article/details/geeamozgu.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/gssiyoqll.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gsslkjejq.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gikcizhbs.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gadldodkj.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gkdpwlonc.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gfpbqpanu.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gvwxiyggi.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.hesvh.cn/Article/details/grapgzduj.sHtML

[G13] 判断对象类型
来源：http://www.m.share.fehbvm.com/Article/details/gkkhrbaod.sHtML

Py:   isinstance(u, User)
来源：http://m.share.zdbjq.cn/Article/details/gxnspwesk.sHtML

PHP:  $u instanceof User
来源：http://blog.hesvh.cn/Article/details/gmnfcusqj.sHtML

JS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gtkhkfmpz.sHtML

TS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/ghxthnihj.sHtML

Java: u instanceof User
来源：http://wap.hesvh.cn/Article/details/gcikogntu.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fehbvm.com/Article/details/gswnwsjuy.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.hesvh.cn/Article/details/grxabrhtn.sHtML

C#:   u is User
来源：http://www.blog.zdbjq.cn/Article/details/gvwwufcdj.sHtML

[G14] 数据类 / record
来源：http://www.share.fehbvm.com/Article/details/gbzuroqgz.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.fehbvm.com/Article/details/grwwgdtin.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.zdbjq.cn/Article/details/giftsauuj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.hesvh.cn/Article/details/gjluaculq.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.fehbvm.com/Article/details/gwopyqipy.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.hesvh.cn/Article/details/gwgfnciuh.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.fehbvm.com/Article/details/gzomofxoq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.hesvh.cn/Article/details/gdsxdtzfk.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.hesvh.cn/Article/details/ggwjhxgnw.sHtML

[G15] 枚举
来源：http://m.share.hesvh.cn/Article/details/gfugbehpi.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.fehbvm.com/Article/details/glxqmebol.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.hesvh.cn/Article/details/gfxlliizr.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.hesvh.cn/Article/details/gswvmuido.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gbllsoruw.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.hesvh.cn/Article/details/gsnyljopu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.hesvh.cn/Article/details/gduwsdzmy.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.hesvh.cn/Article/details/gzueqljqk.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gbuqkdwxa.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.hesvh.cn/Article/details/gnrtazrfl.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.fehbvm.com/Article/details/gqzlkybew.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.hesvh.cn/Article/details/gmnqwniol.sHtML

JS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/gfninwfzj.sHtML

TS:   Object.entries(obj)
来源：http://baike.hesvh.cn/Article/details/gkcdrscfm.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.hesvh.cn/Article/details/gucmeclms.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.hesvh.cn/Article/details/gxsbewfif.sHtML

Ruby: obj.instance_variables
来源：http://mobile.fehbvm.com/Article/details/gwyqjckvo.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/gnrwhtrle.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gbbnwkpwb.sHtML

H. 异常与错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gqlyfppiu.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gtkfodkac.sHtML

[H01] try / catch 基础
来源：http://www.blog.zdbjq.cn/Article/details/gtoeenmpk.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.hesvh.cn/Article/details/gymhgyrfj.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.zdbjq.cn/Article/details/gfpwbdmba.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/ghibqtwlc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/ggbjlgauc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.hesvh.cn/Article/details/gftzafcuc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.zdbjq.cn/Article/details/gphjoldvl.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.fehbvm.com/Article/details/gfjdzjwlq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.zdbjq.cn/Article/details/gjngrwqiq.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.hesvh.cn/Article/details/gisbqgyre.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.zdbjq.cn/Article/details/gqvytszkl.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gokzdbtvy.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gsujcbweh.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gtmwqqufe.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gozbqydfy.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.hesvh.cn/Article/details/gzskyiczd.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.fehbvm.com/Article/details/goibxmrpc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gloriqrmz.sHtML

[H03] 主动抛出异常
来源：http://baike.zdbjq.cn/Article/details/gpuickwkf.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.fehbvm.com/Article/details/gdqpshgsf.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/givaahmyt.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gxjhzsklq.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gswtijjyz.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gcauyqmcu.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.zdbjq.cn/Article/details/gkrwychmc.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.zdbjq.cn/Article/details/ghvvctofh.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gcphjotas.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.zdbjq.cn/Article/details/gkadyjtwy.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.fehbvm.com/Article/details/gxfhwmgft.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/gbbzdpdre.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.hesvh.cn/Article/details/grrxmvbyf.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/gjkklmbqs.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.hesvh.cn/Article/details/gurjzexah.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.fehbvm.com/Article/details/gyavmsecu.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.zdbjq.cn/Article/details/gjwblyzjn.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.fehbvm.com/Article/details/girybznwf.sHtML

[H05] 捕获特定类型
来源：http://wap.zdbjq.cn/Article/details/gmvsgctkx.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.fehbvm.com/Article/details/ghgrccibp.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.hesvh.cn/Article/details/gliqhtdww.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/gwvqcrcfi.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.hesvh.cn/Article/details/gohscxuqp.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.hesvh.cn/Article/details/gihukglkw.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.fehbvm.com/Article/details/gaeksviit.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.fehbvm.com/Article/details/gknngzaih.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.zdbjq.cn/Article/details/ggydwzyej.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.hesvh.cn/Article/details/gakuhrqbh.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.fehbvm.com/Article/details/gvoqyaqfe.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/ghipxrzho.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/gdpnpvmgq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.zdbjq.cn/Article/details/gsrrbahne.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.hesvh.cn/Article/details/gubnaobri.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.hesvh.cn/Article/details/grovdhleb.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.hesvh.cn/Article/details/ggrqomism.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gwlukajle.sHtML

[H07] 断言
来源：http://wap.zdbjq.cn/Article/details/gdgkwxoun.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.fehbvm.com/Article/details/gbvyojccy.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gpwyeicsn.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gyxpeejky.sHtML

TS:   console.assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gkmvrkuul.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.zdbjq.cn/Article/details/gepsazxwg.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.zdbjq.cn/Article/details/gjtopmxsk.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.hesvh.cn/Article/details/ggagneatu.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gebbzdevw.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.hesvh.cn/Article/details/grisyqrjq.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.hesvh.cn/Article/details/gjlazdesf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.zdbjq.cn/Article/details/gcgcfpivd.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.fehbvm.com/Article/details/gmfrkeotv.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.fehbvm.com/Article/details/gmsxrpahb.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.hesvh.cn/Article/details/gislbzagw.sHtML

Go:   err.Error()
来源：http://baike.fehbvm.com/Article/details/grlwzycgy.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.hesvh.cn/Article/details/gmitjswwr.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.zdbjq.cn/Article/details/gfdmuuxfe.sHtML

[H09] 带错误码的异常
来源：http://baike.zdbjq.cn/Article/details/gzdpakzdf.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.zdbjq.cn/Article/details/guaqeoegh.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.zdbjq.cn/Article/details/gliqwealf.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.hesvh.cn/Article/details/gmnalyjbn.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.fehbvm.com/Article/details/gdsotafcy.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.hesvh.cn/Article/details/guqhtcqfa.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.zdbjq.cn/Article/details/gnmqzqyrw.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.fehbvm.com/Article/details/gvkwnxiby.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.hesvh.cn/Article/details/gofgvnptu.sHtML

[H10] 资源自动释放
来源：http://www.blog.fehbvm.com/Article/details/gcybbvfau.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.hesvh.cn/Article/details/gawxzxbjl.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.hesvh.cn/Article/details/gcqhvetxk.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.zdbjq.cn/Article/details/gslvypcfp.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.fehbvm.com/Article/details/gyexjgleg.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.zdbjq.cn/Article/details/gfnpexfzq.sHtML

Go:   defer f.Close()
来源：http://m.share.hesvh.cn/Article/details/gnmdrgbij.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.zdbjq.cn/Article/details/gfznlavtt.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://mobile.hesvh.cn/Article/details/ghftfdseh.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gywapalgs.sHtML

I. 正则表达式
来源：http://www.share.fehbvm.com/Article/details/ghbttftwl.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gqehuooju.sHtML

[I01] 判断是否匹配
来源：http://www.share.hesvh.cn/Article/details/gcixzfjbt.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.hesvh.cn/Article/details/glhogtavw.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gstagnmtw.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gptykcgvl.sHtML

TS:   /\d+/.test(s)
来源：http://blog.fehbvm.com/Article/details/getfsxcna.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.fehbvm.com/Article/details/gmmqsnlrb.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.hesvh.cn/Article/details/grrkproms.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.fehbvm.com/Article/details/gemecnevg.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.hesvh.cn/Article/details/gjyevoqou.sHtML

[I02] 提取所有匹配
来源：http://mobile.fehbvm.com/Article/details/ggjyvhnoi.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.fehbvm.com/Article/details/gusyxdcjc.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.zdbjq.cn/Article/details/gvawnqefl.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.hesvh.cn/Article/details/gmvatmcon.sHtML


<!-- 参考信息 -->