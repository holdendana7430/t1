代发 wailian999

[F09] 获取文件大小
来源：http://baike.hesvh.cn/Article/details/gbnrlushp.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.fehbvm.com/Article/details/gpjocutia.sHtML

PHP:  filesize("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gvgfuonwc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gvuzrextm.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gdiuyuldf.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gpoiipafm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.zdbjq.cn/Article/details/grimelwat.sHtML

Ruby: File.size("a.txt")
来源：http://wap.hesvh.cn/Article/details/gxdpjpprq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.fehbvm.com/Article/details/gbmtexzor.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fehbvm.com/Article/details/gjgauiplk.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/ghbkjqsfk.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.hesvh.cn/Article/details/grecfgdmo.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gcfazsqmu.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gtsogrqdy.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.fehbvm.com/Article/details/gliayvhsn.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/glamyhqqd.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/goiuvupnt.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gtfqfttqo.sHtML

[F11] 复制与移动文件
来源：http://read.share.fehbvm.com/Article/details/gtvnvghgk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gttnvkiuh.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.hesvh.cn/Article/details/gbfsphsux.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gkwugvvmq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gnxzidmai.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.fehbvm.com/Article/details/galeubnxp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.hesvh.cn/Article/details/gkoccvhxd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gtuywbjtv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.fehbvm.com/Article/details/gaorpieug.sHtML

[F12] CSV 读写
来源：http://baike.hesvh.cn/Article/details/gjajdvwop.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fehbvm.com/Article/details/gclpsfgdb.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.hesvh.cn/Article/details/giorhaagk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.hesvh.cn/Article/details/gvivfwopj.sHtML

TS:   // 同上
来源：http://www.blog.zdbjq.cn/Article/details/gnbbdbtgr.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.hesvh.cn/Article/details/gcmxgehnu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.hesvh.cn/Article/details/gwqisxsjz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fehbvm.com/Article/details/gsowfbkok.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.hesvh.cn/Article/details/gaprywvxf.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gegbsgrdg.sHtML

G. 面向对象
来源：http://mobile.zdbjq.cn/Article/details/gqdpiwhrm.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gvjnaisjk.sHtML

[G01] 定义类
来源：http://www.blog.fehbvm.com/Article/details/gukfykkji.sHtML

Py:   class User: pass
来源：http://m.share.hesvh.cn/Article/details/gqqdhhxpm.sHtML

PHP:  class User {}
来源：http://blog.fehbvm.com/Article/details/gvvctxmjy.sHtML

JS:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gwbpxzzgw.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.hesvh.cn/Article/details/glehzxvcn.sHtML

Java: class User {}
来源：http://www.share.zdbjq.cn/Article/details/gmioaixqm.sHtML

Go:   type User struct { Name string }
来源：http://3g.hesvh.cn/Article/details/gzlyfzbtt.sHtML

Ruby: class User; end
来源：http://www.blog.zdbjq.cn/Article/details/gxtanymfb.sHtML

C#:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gponbdcgm.sHtML

[G02] 构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gjtsmxoxq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.zdbjq.cn/Article/details/gwzubvpll.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.zdbjq.cn/Article/details/gsalyupqv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gxcvlxagw.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.zdbjq.cn/Article/details/giadqixhe.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/ghjnygsuk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.fehbvm.com/Article/details/gtwfvvcdh.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fehbvm.com/Article/details/gsaaxdwul.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gxthkaulw.sHtML

[G03] 实例属性
来源：http://baike.zdbjq.cn/Article/details/ggtuwpbdk.sHtML

Py:   self.name = "x"
来源：http://baike.fehbvm.com/Article/details/gbybznkls.sHtML

PHP:  public string $name = "x";
来源：http://read.share.hesvh.cn/Article/details/gfetpfoil.sHtML

JS:   this.name = "x";
来源：http://mobile.hesvh.cn/Article/details/gekibquvs.sHtML

TS:   name: string = "x";
来源：http://www.m.share.hesvh.cn/Article/details/glqpmlwtb.sHtML

Java: private String name;
来源：http://baike.hesvh.cn/Article/details/gamucmtov.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.zdbjq.cn/Article/details/gmagjfwmf.sHtML

Ruby: @name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gkxftidhy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.zdbjq.cn/Article/details/gagicqcvx.sHtML

[G04] 定义方法
来源：http://3g.hesvh.cn/Article/details/gzjjoilmb.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gkmlezlhg.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gymrcffbx.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gixryyhzu.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gbbqefejt.sHtML

Java: String greet() { return name; }
来源：http://blog.hesvh.cn/Article/details/gcvcyojru.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gmmezdowj.sHtML

Ruby: def greet; @name; end
来源：http://wap.zdbjq.cn/Article/details/ghiojeziq.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.fehbvm.com/Article/details/gxwotuctb.sHtML

[G05] 继承
来源：http://www.m.share.hesvh.cn/Article/details/gtemuouaj.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.hesvh.cn/Article/details/gvrftvrpl.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gnkeyglgo.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gqihonthx.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/grnzagjdy.sHtML

Java: class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gzpohffwk.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.zdbjq.cn/Article/details/gauxnbnzn.sHtML

Ruby: class Admin < User; end
来源：http://mobile.hesvh.cn/Article/details/gldnexwpk.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fehbvm.com/Article/details/gpaahluib.sHtML

[G06] 重写方法
来源：http://www.blog.fehbvm.com/Article/details/glmnwgakl.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.zdbjq.cn/Article/details/gcmvcmvqv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gkoqnhjfk.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/grivhdbvl.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gitadqrar.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gmeflfeok.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.zdbjq.cn/Article/details/gfqzkmcts.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.hesvh.cn/Article/details/gxgzylalv.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fehbvm.com/Article/details/gwhtlslic.sHtML

[G07] 调用父类方法
来源：http://mobile.fehbvm.com/Article/details/gmdxxvtwl.sHtML

Py:   super().greet()
来源：http://mobile.fehbvm.com/Article/details/gdoxudpvx.sHtML

PHP:  parent::greet();
来源：http://baike.fehbvm.com/Article/details/gopsicfzj.sHtML

JS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gopcbuewd.sHtML

TS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gntqhgzjf.sHtML

Java: super.greet();
来源：http://3g.hesvh.cn/Article/details/gmsagqhix.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.fehbvm.com/Article/details/gvarzhwzj.sHtML

Ruby: super
来源：http://3g.fehbvm.com/Article/details/gonhpvizp.sHtML

C#:   base.Greet();
来源：http://3g.zdbjq.cn/Article/details/gyyarwouz.sHtML

[G08] 静态方法与属性
来源：http://mobile.zdbjq.cn/Article/details/gfaeqetnf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.hesvh.cn/Article/details/gvucvdzmw.sHtML

PHP:  public static function f() {}
来源：http://mobile.zdbjq.cn/Article/details/getfcqmmr.sHtML

JS:   static f() {}
来源：http://m.share.zdbjq.cn/Article/details/gmixpwqlm.sHtML

TS:   static f(): void {}
来源：http://www.blog.hesvh.cn/Article/details/gumlnygqv.sHtML

Java: static void f() {}
来源：http://m.share.zdbjq.cn/Article/details/ggwnwnngq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.fehbvm.com/Article/details/gnyqnexef.sHtML

Ruby: def self.f; end
来源：http://baike.hesvh.cn/Article/details/gachdjsig.sHtML

C#:   public static void F() {}
来源：http://baike.zdbjq.cn/Article/details/gwwrjalgv.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.fehbvm.com/Article/details/gbpowptzm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.zdbjq.cn/Article/details/gqkyrgzmk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.hesvh.cn/Article/details/ghimegelu.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.fehbvm.com/Article/details/gokptjdnk.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.hesvh.cn/Article/details/gixhvgrea.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.hesvh.cn/Article/details/gmnzsqopr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.fehbvm.com/Article/details/grloeepvd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.zdbjq.cn/Article/details/gfwbjtijg.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.hesvh.cn/Article/details/ghdtgfrqv.sHtML

[G10] 访问控制
来源：http://baike.fehbvm.com/Article/details/gfdjtvziq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.zdbjq.cn/Article/details/gdvhzktyl.sHtML

PHP:  public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gzbtsoggm.sHtML

JS:   #private 字段；其余公开
来源：http://blog.zdbjq.cn/Article/details/gakygoydr.sHtML

TS:   public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gpqbajwzk.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.zdbjq.cn/Article/details/ggscilmzm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.zdbjq.cn/Article/details/gxzmnaslh.sHtML

Ruby: public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gjkghptji.sHtML

C#:   public / protected / private / internal
来源：http://wap.fehbvm.com/Article/details/gcpadogyk.sHtML

[G11] getter / setter
来源：http://baike.zdbjq.cn/Article/details/gagcyxnrq.sHtML

Py:   @property 与 @x.setter
来源：http://baike.hesvh.cn/Article/details/gqtbanpak.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfhsugpij.sHtML

JS:   get name() { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gpuntceme.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gnoykfqpo.sHtML

Java: public String getName() { return name; }
来源：http://baike.hesvh.cn/Article/details/gzequpmam.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gsklsdewr.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fehbvm.com/Article/details/gijbjjbhc.sHtML

C#:   public string Name { get; set; }
来源：http://baike.hesvh.cn/Article/details/gwjthdxvd.sHtML

[G12] 对象转字符串
来源：http://wap.zdbjq.cn/Article/details/grbxyewfh.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gggkshgpi.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gmryzbxmb.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/georvfwxl.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gjxwmheqf.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.hesvh.cn/Article/details/gqozvhnzc.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gudlgrkvx.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.hesvh.cn/Article/details/gwpmcqqtt.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gvtjdqayx.sHtML

[G13] 判断对象类型
来源：http://mobile.zdbjq.cn/Article/details/gohooonhg.sHtML

Py:   isinstance(u, User)
来源：http://3g.hesvh.cn/Article/details/gnyvwzemr.sHtML

PHP:  $u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gschmenly.sHtML

JS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gzhmzqpfm.sHtML

TS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gbtnqfhbj.sHtML

Java: u instanceof User
来源：http://3g.hesvh.cn/Article/details/gspgjtauv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.hesvh.cn/Article/details/gdyzonpea.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.fehbvm.com/Article/details/gsgriyqqk.sHtML

C#:   u is User
来源：http://read.share.hesvh.cn/Article/details/ghdjokaeb.sHtML

[G14] 数据类 / record
来源：http://baike.zdbjq.cn/Article/details/geelwnute.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.hesvh.cn/Article/details/gadavbwxt.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.fehbvm.com/Article/details/gvrqfglis.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.zdbjq.cn/Article/details/glhsdddnl.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.zdbjq.cn/Article/details/gftjmfkuh.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.zdbjq.cn/Article/details/gfifttqbi.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.zdbjq.cn/Article/details/gjxqyosdu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.fehbvm.com/Article/details/ghlcrdtml.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.hesvh.cn/Article/details/ghpbqcgzy.sHtML

[G15] 枚举
来源：http://3g.fehbvm.com/Article/details/gytaefoqm.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.hesvh.cn/Article/details/giqipavtt.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gneohkbhe.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.fehbvm.com/Article/details/guwntorlh.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gjkjdslhc.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.hesvh.cn/Article/details/gjwcyjvie.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.fehbvm.com/Article/details/gjjnvqjhb.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.zdbjq.cn/Article/details/grfdknllx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/gqwfqlkpw.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.hesvh.cn/Article/details/gvyudftnt.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.zdbjq.cn/Article/details/gfjpttnpe.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.hesvh.cn/Article/details/ghhyuzmoi.sHtML

JS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/guaurxupr.sHtML

TS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/golmhlfrn.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.fehbvm.com/Article/details/gwdnbjpqv.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.zdbjq.cn/Article/details/ghrboaoyt.sHtML

Ruby: obj.instance_variables
来源：http://mobile.hesvh.cn/Article/details/gdbtqafdz.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.zdbjq.cn/Article/details/gfvcrfuzo.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gwrcdwcep.sHtML

H. 异常与错误处理
来源：http://baike.fehbvm.com/Article/details/gbgedxdia.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxbulpopb.sHtML

[H01] try / catch 基础
来源：http://www.share.hesvh.cn/Article/details/gziftsyzi.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.hesvh.cn/Article/details/girocduuf.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gytlxmygw.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/ggomrtlov.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gcsqujhsg.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.hesvh.cn/Article/details/gpqhhbiur.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.fehbvm.com/Article/details/gshzlnubb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.fehbvm.com/Article/details/giwauayuc.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.hesvh.cn/Article/details/gmbwabkgd.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.zdbjq.cn/Article/details/gwnaokpbx.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.hesvh.cn/Article/details/gnctjocnq.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gqooawzgv.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gbkxsavgn.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gzhhswbnb.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gouivfzxr.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.fehbvm.com/Article/details/gtwqmpluh.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.hesvh.cn/Article/details/gmuzrfdmn.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gmcnvjear.sHtML

[H03] 主动抛出异常
来源：http://mobile.fehbvm.com/Article/details/gnnqepyiy.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.hesvh.cn/Article/details/gkrbzqbpz.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gvbwsnnih.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gimnqodzp.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gqbdccatr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gmlzaxlns.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.hesvh.cn/Article/details/ggimyxkmz.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.hesvh.cn/Article/details/gjisbihxy.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gnembhohh.sHtML

[H04] 自定义异常类型
来源：http://www.share.fehbvm.com/Article/details/gyxlpjdbx.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.zdbjq.cn/Article/details/ghormgpwa.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/gmmgqkgre.sHtML

JS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/geskaugzz.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/gvhmfwvfl.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.hesvh.cn/Article/details/gaonbvahm.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.zdbjq.cn/Article/details/gaqqgkdwx.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.hesvh.cn/Article/details/gwfxjrziy.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.hesvh.cn/Article/details/gzoxkzxvm.sHtML

[H05] 捕获特定类型
来源：http://baike.hesvh.cn/Article/details/gbjevvyxt.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.zdbjq.cn/Article/details/gshgzmnqk.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.zdbjq.cn/Article/details/gskhbxixq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.hesvh.cn/Article/details/gxbspzejo.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.zdbjq.cn/Article/details/gunhjagut.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.hesvh.cn/Article/details/gbhrijlzd.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.fehbvm.com/Article/details/gffzungle.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.zdbjq.cn/Article/details/gkockvkhd.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.zdbjq.cn/Article/details/gceszppai.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.zdbjq.cn/Article/details/gxpxoicby.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.fehbvm.com/Article/details/gogejzhmi.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.fehbvm.com/Article/details/gwjmastgi.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.hesvh.cn/Article/details/gvbeitutd.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.fehbvm.com/Article/details/gjhdrxeoe.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.zdbjq.cn/Article/details/gwgorgxxv.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.hesvh.cn/Article/details/goscbfnde.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.hesvh.cn/Article/details/gethhgaej.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.zdbjq.cn/Article/details/giyrcuawi.sHtML

[H07] 断言
来源：http://read.share.fehbvm.com/Article/details/gtvcurnoc.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.hesvh.cn/Article/details/gtscmfgzn.sHtML

PHP:  assert($x > 0);
来源：http://baike.hesvh.cn/Article/details/gdezcvzdl.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/gooegznse.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/ghhtnpaxi.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.hesvh.cn/Article/details/gezonmjyg.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.zdbjq.cn/Article/details/gsarhvzva.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.fehbvm.com/Article/details/gpwilerxw.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gzugusajq.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.fehbvm.com/Article/details/gadugnqto.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.fehbvm.com/Article/details/gictuhfbe.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.zdbjq.cn/Article/details/gnoqyjxxf.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.zdbjq.cn/Article/details/ghwtzalai.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.hesvh.cn/Article/details/gbypggxsf.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.zdbjq.cn/Article/details/gntbupwta.sHtML

Go:   err.Error()
来源：http://mobile.zdbjq.cn/Article/details/glyolxqqy.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.hesvh.cn/Article/details/gntknoypd.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.zdbjq.cn/Article/details/gicqmrngr.sHtML

[H09] 带错误码的异常
来源：http://m.share.zdbjq.cn/Article/details/gdqmkliwz.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.hesvh.cn/Article/details/grnllrtnu.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.zdbjq.cn/Article/details/gaudqzdcu.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.fehbvm.com/Article/details/gumrjiiga.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.fehbvm.com/Article/details/gtyiwsmql.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.fehbvm.com/Article/details/gdgbwxbpm.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.hesvh.cn/Article/details/gqxpftsxr.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.hesvh.cn/Article/details/goqqralve.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.zdbjq.cn/Article/details/gtwkrhvxn.sHtML

[H10] 资源自动释放
来源：http://read.share.hesvh.cn/Article/details/goxnvpqjr.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.zdbjq.cn/Article/details/gccybqbtc.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.hesvh.cn/Article/details/gnwtwssfr.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.hesvh.cn/Article/details/gwxbmgfec.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fehbvm.com/Article/details/girdovgah.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.zdbjq.cn/Article/details/geqrklwmz.sHtML

Go:   defer f.Close()
来源：http://mobile.fehbvm.com/Article/details/gfgnzhqlr.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.fehbvm.com/Article/details/gwxkklopc.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.hesvh.cn/Article/details/gysticgig.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/grtkpmepc.sHtML

I. 正则表达式
来源：http://blog.hesvh.cn/Article/details/guwxfhcoc.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gpjwevkai.sHtML

[I01] 判断是否匹配
来源：http://m.share.zdbjq.cn/Article/details/gtsgsnepm.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.zdbjq.cn/Article/details/gqyeqogbf.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gfulechrg.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gnaxsujmn.sHtML

TS:   /\d+/.test(s)
来源：http://wap.zdbjq.cn/Article/details/gtahqqcou.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.zdbjq.cn/Article/details/ghmvlbqsw.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.zdbjq.cn/Article/details/gxlwpzulr.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.fehbvm.com/Article/details/giujopqkv.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.zdbjq.cn/Article/details/ggsaacljk.sHtML

[I02] 提取所有匹配
来源：http://3g.zdbjq.cn/Article/details/ghaanugsi.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.zdbjq.cn/Article/details/grtxuqdcz.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.zdbjq.cn/Article/details/goscmfoxl.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.fehbvm.com/Article/details/giwiwjbzd.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.hesvh.cn/Article/details/gnxlqyvxl.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.hesvh.cn/Article/details/gbcvnalfg.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.zdbjq.cn/Article/details/gpebgwfjs.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.hesvh.cn/Article/details/gbhzytjrq.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gmdppyqgc.sHtML

[I03] 提取捕获分组
来源：http://www.blog.hesvh.cn/Article/details/gaacplqux.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.zdbjq.cn/Article/details/gwrccbpmq.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.zdbjq.cn/Article/details/gghzviuso.sHtML


<!-- 参考信息 -->