代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.fehbvm.com/Article/details/ghkcfcxef.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.zdbjq.cn/Article/details/geczkxiyc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.hesvh.cn/Article/details/gilhkilrr.sHtML

[F08] 遍历目录
来源：http://wap.hesvh.cn/Article/details/gzxzputko.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.fehbvm.com/Article/details/grzywigdm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.hesvh.cn/Article/details/gwoyckcmb.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/gtvthczhk.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gkhtiraqy.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gnsdjqvfb.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.fehbvm.com/Article/details/gwedmuomh.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.hesvh.cn/Article/details/guerhjzva.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.hesvh.cn/Article/details/giunhrmon.sHtML

[F09] 获取文件大小
来源：http://www.share.hesvh.cn/Article/details/ghzajqqvt.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gelrvvzmb.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.hesvh.cn/Article/details/ggktgoxyn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gahqrnveb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/gdrrbzhkb.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/geuxwtyzc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.fehbvm.com/Article/details/gyrrwrpgz.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gialgvjwa.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.hesvh.cn/Article/details/ghtatavdw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.zdbjq.cn/Article/details/gdjtjcvxp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gbennozsh.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gembimwui.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gapbgvwjw.sHtML

TS:   path.extname("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gxzsjahjm.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.hesvh.cn/Article/details/gxfkznoye.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gythlnzkl.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/ghtabiaql.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gebjkkpnd.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fehbvm.com/Article/details/gxbozscpo.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gytfsfqdt.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.hesvh.cn/Article/details/gamcbhdbd.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/geqfyzepc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gkpzolhcd.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.hesvh.cn/Article/details/ghvybnhjj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.zdbjq.cn/Article/details/gzhyrtmmj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ggymxbath.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.fehbvm.com/Article/details/gejzquaom.sHtML

[F12] CSV 读写
来源：http://www.share.hesvh.cn/Article/details/ghhxuywgh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.zdbjq.cn/Article/details/gmaajefqw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.fehbvm.com/Article/details/gjbrpanqn.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.zdbjq.cn/Article/details/ghfahpqdy.sHtML

TS:   // 同上
来源：http://blog.fehbvm.com/Article/details/gjvetxjcj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.hesvh.cn/Article/details/gzvtzyeko.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.hesvh.cn/Article/details/gstraluvr.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.zdbjq.cn/Article/details/gievmybhv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.fehbvm.com/Article/details/gmirzisen.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gxpykfifl.sHtML

G. 面向对象
来源：http://www.m.share.zdbjq.cn/Article/details/gktfdsnra.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ghqvlpapq.sHtML

[G01] 定义类
来源：http://www.blog.fehbvm.com/Article/details/gtnffnrpb.sHtML

Py:   class User: pass
来源：http://m.share.hesvh.cn/Article/details/goaljqzqv.sHtML

PHP:  class User {}
来源：http://mobile.zdbjq.cn/Article/details/gimxeeism.sHtML

JS:   class User {}
来源：http://3g.zdbjq.cn/Article/details/ggtqgbghx.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.fehbvm.com/Article/details/gsjyxpfaw.sHtML

Java: class User {}
来源：http://www.share.hesvh.cn/Article/details/gwttivhlr.sHtML

Go:   type User struct { Name string }
来源：http://read.share.zdbjq.cn/Article/details/gfwkdorco.sHtML

Ruby: class User; end
来源：http://mobile.fehbvm.com/Article/details/gaanrjndc.sHtML

C#:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gjmrontew.sHtML

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/gmoxfotcb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.fehbvm.com/Article/details/gheqsermm.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.hesvh.cn/Article/details/gdfijfmue.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gquihesjd.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.hesvh.cn/Article/details/gnvszenwz.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gdltbmwxv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.hesvh.cn/Article/details/glhnbshcj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.hesvh.cn/Article/details/grrjkkyuz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gtnkvkbyd.sHtML

[G03] 实例属性
来源：http://read.share.fehbvm.com/Article/details/gmiawzyxy.sHtML

Py:   self.name = "x"
来源：http://baike.hesvh.cn/Article/details/gyjuvbymz.sHtML

PHP:  public string $name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gyffbwsqn.sHtML

JS:   this.name = "x";
来源：http://read.share.fehbvm.com/Article/details/gnkcyqwxx.sHtML

TS:   name: string = "x";
来源：http://3g.fehbvm.com/Article/details/glccunmxx.sHtML

Java: private String name;
来源：http://wap.zdbjq.cn/Article/details/godwnlcgv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.hesvh.cn/Article/details/gxxrcprma.sHtML

Ruby: @name = "x"
来源：http://3g.zdbjq.cn/Article/details/gadcepqyt.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fehbvm.com/Article/details/gesyxyqhl.sHtML

[G04] 定义方法
来源：http://www.m.share.fehbvm.com/Article/details/gdabyzoar.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gihiultwu.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gwaiecjnj.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/goxzbjvkm.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gzjawjlel.sHtML

Java: String greet() { return name; }
来源：http://baike.fehbvm.com/Article/details/ggwgkxvzc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gorgqmlau.sHtML

Ruby: def greet; @name; end
来源：http://baike.hesvh.cn/Article/details/gjbokswhl.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gryhtncsj.sHtML

[G05] 继承
来源：http://mobile.fehbvm.com/Article/details/gdtenojbs.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/gldywgbbx.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gmkrquwhu.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gkzwegonk.sHtML

TS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gnqijrhph.sHtML

Java: class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gplmtxozk.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.zdbjq.cn/Article/details/gidvkpzbk.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.zdbjq.cn/Article/details/gvdyfdirz.sHtML

C#:   class Admin : User {}
来源：http://www.blog.hesvh.cn/Article/details/gfvermkbr.sHtML

[G06] 重写方法
来源：http://3g.fehbvm.com/Article/details/ghuhjrmtn.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.zdbjq.cn/Article/details/gnxtlyjis.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gxaduxxvz.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/grpnugvqi.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gqjlqbgam.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gvxucyzkf.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.fehbvm.com/Article/details/geibuwaui.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.hesvh.cn/Article/details/gtbhzkrwj.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.hesvh.cn/Article/details/ghpjszluf.sHtML

[G07] 调用父类方法
来源：http://www.blog.fehbvm.com/Article/details/gtpmfheea.sHtML

Py:   super().greet()
来源：http://baike.fehbvm.com/Article/details/gdttuzyuk.sHtML

PHP:  parent::greet();
来源：http://mobile.hesvh.cn/Article/details/ghtbxxdam.sHtML

JS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gbjvnavla.sHtML

TS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/glbejtrpt.sHtML

Java: super.greet();
来源：http://m.share.hesvh.cn/Article/details/gccrunrwd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.zdbjq.cn/Article/details/gzsmgutst.sHtML

Ruby: super
来源：http://www.m.share.fehbvm.com/Article/details/gwlfwbpkk.sHtML

C#:   base.Greet();
来源：http://baike.zdbjq.cn/Article/details/gkurjvrzd.sHtML

[G08] 静态方法与属性
来源：http://mobile.fehbvm.com/Article/details/gxypbjqld.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.hesvh.cn/Article/details/gajdsqwrs.sHtML

PHP:  public static function f() {}
来源：http://baike.hesvh.cn/Article/details/gyctfmqru.sHtML

JS:   static f() {}
来源：http://mobile.hesvh.cn/Article/details/gzimqeymp.sHtML

TS:   static f(): void {}
来源：http://wap.hesvh.cn/Article/details/gicfpctbk.sHtML

Java: static void f() {}
来源：http://m.share.hesvh.cn/Article/details/guichmafl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.zdbjq.cn/Article/details/gohnzqvff.sHtML

Ruby: def self.f; end
来源：http://read.share.fehbvm.com/Article/details/gnnjjulst.sHtML

C#:   public static void F() {}
来源：http://www.share.hesvh.cn/Article/details/gqgboasiz.sHtML

[G09] 接口 / 抽象类
来源：http://baike.zdbjq.cn/Article/details/gzcuxpkbe.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.fehbvm.com/Article/details/glldskorj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.zdbjq.cn/Article/details/gxfhcuawf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.zdbjq.cn/Article/details/goonetxpq.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.zdbjq.cn/Article/details/grtakprcp.sHtML

Java: interface Shape { double area(); }
来源：http://blog.fehbvm.com/Article/details/grgztquwj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.zdbjq.cn/Article/details/glqjeqhln.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fehbvm.com/Article/details/gpptgtlsx.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.zdbjq.cn/Article/details/gixkbwssx.sHtML

[G10] 访问控制
来源：http://wap.fehbvm.com/Article/details/gnrudggzv.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.hesvh.cn/Article/details/gjnsuzirq.sHtML

PHP:  public / protected / private
来源：http://mobile.hesvh.cn/Article/details/goqdixbmz.sHtML

JS:   #private 字段；其余公开
来源：http://blog.hesvh.cn/Article/details/gnbvqwuvb.sHtML

TS:   public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gyzhlozdz.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fehbvm.com/Article/details/gdsyhqahp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.hesvh.cn/Article/details/glgbfagnr.sHtML

Ruby: public / protected / private
来源：http://3g.fehbvm.com/Article/details/gdgabuhks.sHtML

C#:   public / protected / private / internal
来源：http://read.share.zdbjq.cn/Article/details/gydzwnjxy.sHtML

[G11] getter / setter
来源：http://www.blog.fehbvm.com/Article/details/gxreycgtw.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.zdbjq.cn/Article/details/gkbsautmv.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/giokszaow.sHtML

JS:   get name() { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/grknigydl.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.hesvh.cn/Article/details/ghgdoouqi.sHtML

Java: public String getName() { return name; }
来源：http://blog.hesvh.cn/Article/details/gapnxvwjk.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/ghbygjmgm.sHtML

Ruby: attr_accessor :name
来源：http://3g.fehbvm.com/Article/details/gapfuscwo.sHtML

C#:   public string Name { get; set; }
来源：http://wap.hesvh.cn/Article/details/gsegkoyys.sHtML

[G12] 对象转字符串
来源：http://www.share.hesvh.cn/Article/details/gahxwmiuw.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/ghfyxsidz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gxzcxihld.sHtML

JS:   toString() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gltkifiaw.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gybgzukms.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.hesvh.cn/Article/details/gcoljhjca.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gmuvtpdls.sHtML

Ruby: def to_s; @name; end
来源：http://baike.zdbjq.cn/Article/details/gieiteldr.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.hesvh.cn/Article/details/gmzmjhoea.sHtML

[G13] 判断对象类型
来源：http://mobile.hesvh.cn/Article/details/gdqhtnakq.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fehbvm.com/Article/details/gpbmtivml.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gkxwxolti.sHtML

JS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/goomsuutw.sHtML

TS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/gryhqvpnf.sHtML

Java: u instanceof User
来源：http://blog.fehbvm.com/Article/details/gnbtlytep.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.hesvh.cn/Article/details/guehohgzk.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.hesvh.cn/Article/details/ghpbdjuva.sHtML

C#:   u is User
来源：http://m.share.hesvh.cn/Article/details/glupqsbaa.sHtML

[G14] 数据类 / record
来源：http://www.share.fehbvm.com/Article/details/gokazaohi.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.hesvh.cn/Article/details/gebpisbrb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.fehbvm.com/Article/details/gvxnrzsnl.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fehbvm.com/Article/details/gmohjssiy.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.hesvh.cn/Article/details/gauzougel.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.hesvh.cn/Article/details/gxdqrcllp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.zdbjq.cn/Article/details/gbyaqxtlu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.fehbvm.com/Article/details/gxgrwsmxb.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.zdbjq.cn/Article/details/gcntaytst.sHtML

[G15] 枚举
来源：http://www.blog.zdbjq.cn/Article/details/gqtvemnau.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fehbvm.com/Article/details/gxpjlkdkr.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.hesvh.cn/Article/details/gcvwtxycg.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.zdbjq.cn/Article/details/gfxgzryjx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gcjpdqyxh.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.fehbvm.com/Article/details/gibbwlxzg.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.hesvh.cn/Article/details/gyfmpmsop.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.fehbvm.com/Article/details/gpjvsghqn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/ggihrekuq.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.fehbvm.com/Article/details/gkariyvnd.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.zdbjq.cn/Article/details/gnclmpksq.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.fehbvm.com/Article/details/ghrlkwsue.sHtML

JS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/gizdwgmhe.sHtML

TS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/gciiqjedp.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.zdbjq.cn/Article/details/gqbmiiatq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.hesvh.cn/Article/details/gblbsedfh.sHtML

Ruby: obj.instance_variables
来源：http://blog.hesvh.cn/Article/details/ggcxlrwql.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.hesvh.cn/Article/details/giyqyfwgr.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gbwcxbjwe.sHtML

H. 异常与错误处理
来源：http://www.blog.zdbjq.cn/Article/details/grpdwyass.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gdpimxiid.sHtML

[H01] try / catch 基础
来源：http://www.blog.fehbvm.com/Article/details/gyxzsofeu.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.zdbjq.cn/Article/details/gxsstkaiz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.hesvh.cn/Article/details/gugkeeaun.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gglgfukzg.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gmvddxmfb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.fehbvm.com/Article/details/gzewtomem.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.fehbvm.com/Article/details/gdayirtcf.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.fehbvm.com/Article/details/gonzbgojc.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.fehbvm.com/Article/details/gxsdwmdag.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.hesvh.cn/Article/details/gsfzqfqgf.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.zdbjq.cn/Article/details/gpnaklynz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gbamvonzn.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/ghomdyvnd.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gqunprarv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gfnshfwdl.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.zdbjq.cn/Article/details/gzxhjavwx.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.hesvh.cn/Article/details/gcuctofbx.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gtiggsizc.sHtML

[H03] 主动抛出异常
来源：http://3g.zdbjq.cn/Article/details/guegvchja.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.zdbjq.cn/Article/details/gvdkhmlxv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gtgqwkdrb.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gfmfzkuge.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gaywakthw.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/grsfruirt.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.fehbvm.com/Article/details/gxiqszshm.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.hesvh.cn/Article/details/glxaxekdo.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gavhaxwzn.sHtML

[H04] 自定义异常类型
来源：http://baike.zdbjq.cn/Article/details/gtsjonaee.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.hesvh.cn/Article/details/gkwpxaqdr.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.fehbvm.com/Article/details/gxtpnugnm.sHtML

JS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/ggbpxiiym.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.zdbjq.cn/Article/details/gqtjeitjl.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/gyaibyvaz.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.fehbvm.com/Article/details/gjbljokgf.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.zdbjq.cn/Article/details/gvywdrjgf.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.zdbjq.cn/Article/details/gxgpthhiq.sHtML

[H05] 捕获特定类型
来源：http://3g.zdbjq.cn/Article/details/gwgjqtuio.sHtML

Py:   except ValueError as e:
来源：http://read.share.zdbjq.cn/Article/details/gznvsgytw.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.zdbjq.cn/Article/details/gszhsuwnj.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/gtjhsrtxt.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/gvirqkvdo.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.fehbvm.com/Article/details/ggdihdppf.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.fehbvm.com/Article/details/grdcsuejs.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.zdbjq.cn/Article/details/gxcolaxvh.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.zdbjq.cn/Article/details/gjuuwippm.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.zdbjq.cn/Article/details/gbhyongjn.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.zdbjq.cn/Article/details/ghsnvsrqy.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/gaoimgpnq.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/gdjtnusrf.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.zdbjq.cn/Article/details/gqqnutyim.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.zdbjq.cn/Article/details/giyoddaum.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.hesvh.cn/Article/details/gbpkfoiqv.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.hesvh.cn/Article/details/grshcvovz.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.fehbvm.com/Article/details/gxrjfnzyy.sHtML

[H07] 断言
来源：http://www.share.zdbjq.cn/Article/details/gimecqvqz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.zdbjq.cn/Article/details/gwbrwnius.sHtML

PHP:  assert($x > 0);
来源：http://mobile.hesvh.cn/Article/details/gmekdpywk.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/goqeqaoqu.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gqrueedzp.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.fehbvm.com/Article/details/gkxaajsfh.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.hesvh.cn/Article/details/gekqkbaoo.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.hesvh.cn/Article/details/geijjanzx.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gfkgjedyi.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.fehbvm.com/Article/details/gemebyfxy.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.zdbjq.cn/Article/details/gfugnpvgk.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.fehbvm.com/Article/details/gnadhbrjj.sHtML

JS:   e.message;  e.stack
来源：http://3g.hesvh.cn/Article/details/gcoiiuplw.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.hesvh.cn/Article/details/gktakhfzc.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.hesvh.cn/Article/details/gribehrlg.sHtML

Go:   err.Error()
来源：http://3g.zdbjq.cn/Article/details/gljujrqys.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.zdbjq.cn/Article/details/gwjvudruh.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.fehbvm.com/Article/details/gjgwpjcum.sHtML

[H09] 带错误码的异常
来源：http://mobile.fehbvm.com/Article/details/gopmsxrcj.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.fehbvm.com/Article/details/gnpycjbus.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.hesvh.cn/Article/details/gnsqfogsf.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.hesvh.cn/Article/details/gtfrcnfpu.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.fehbvm.com/Article/details/gjdhsibqd.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.fehbvm.com/Article/details/gdmyotpev.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://baike.fehbvm.com/Article/details/gqpydrfmh.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.hesvh.cn/Article/details/gpravmlhc.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.hesvh.cn/Article/details/gyztqdwnk.sHtML

[H10] 资源自动释放
来源：http://3g.hesvh.cn/Article/details/giomrmerl.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.hesvh.cn/Article/details/geeyefhsx.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.fehbvm.com/Article/details/gnfqoqnml.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fehbvm.com/Article/details/gzpkcvngu.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fehbvm.com/Article/details/gneaykmnh.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.zdbjq.cn/Article/details/gdgqrevmo.sHtML

Go:   defer f.Close()
来源：http://m.share.zdbjq.cn/Article/details/gporyebkm.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.fehbvm.com/Article/details/gcmoxtieq.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.zdbjq.cn/Article/details/glsnhfcjr.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghqjtltvf.sHtML

I. 正则表达式
来源：http://baike.fehbvm.com/Article/details/gkleukjun.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gnsdruxpp.sHtML

[I01] 判断是否匹配
来源：http://www.share.zdbjq.cn/Article/details/gjkvxgdky.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.fehbvm.com/Article/details/gmcralmlo.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.fehbvm.com/Article/details/gwehorzrp.sHtML

JS:   /\d+/.test(s)
来源：http://blog.hesvh.cn/Article/details/gmrrbjrmb.sHtML

TS:   /\d+/.test(s)
来源：http://blog.zdbjq.cn/Article/details/gxkywthbo.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.fehbvm.com/Article/details/gmzuipcsr.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.hesvh.cn/Article/details/gursprrrn.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.fehbvm.com/Article/details/gekdyafrn.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.fehbvm.com/Article/details/garnqpyvf.sHtML


<!-- 参考信息 -->