代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/gcjqrcobf.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.hesvh.cn/Article/details/gdixmiqwz.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.zdbjq.cn/Article/details/gybkrpgax.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.fehbvm.com/Article/details/gmlaydknn.sHtML

[F09] 获取文件大小
来源：http://www.m.share.fehbvm.com/Article/details/gihxlbrgs.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/guraermhh.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gqvyvslzf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/ghayidwmn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/glhaczlvi.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gvsaxiaep.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.zdbjq.cn/Article/details/geskbepyq.sHtML

Ruby: File.size("a.txt")
来源：http://wap.zdbjq.cn/Article/details/ghwdlqyku.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.fehbvm.com/Article/details/gxdhisdqp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fehbvm.com/Article/details/ggswnwiiz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gvlugsnrq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gtxflhdfm.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/giboqkpbx.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/grilgfdym.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.fehbvm.com/Article/details/gtvwgijpe.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gxpafdymm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gtjdeuddy.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/govnctmrd.sHtML

[F11] 复制与移动文件
来源：http://blog.hesvh.cn/Article/details/gyvfhxwex.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gjltntpyh.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.fehbvm.com/Article/details/gmuccidhx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gbajyicbg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/ghpqihdig.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gmhfnripe.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.hesvh.cn/Article/details/gttttagic.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gpzjeqjnt.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fehbvm.com/Article/details/gcibmlmzl.sHtML

[F12] CSV 读写
来源：http://blog.fehbvm.com/Article/details/gjnpuvryq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.fehbvm.com/Article/details/gswpsqaut.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.zdbjq.cn/Article/details/gulqtaytg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.hesvh.cn/Article/details/gqzrxjawm.sHtML

TS:   // 同上
来源：http://www.blog.hesvh.cn/Article/details/gqtxteupw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.zdbjq.cn/Article/details/gpqbpuhqg.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.zdbjq.cn/Article/details/giuqqufso.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fehbvm.com/Article/details/ghbvnghbo.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fehbvm.com/Article/details/gfahhvbny.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gdknxrmug.sHtML

G. 面向对象
来源：http://blog.zdbjq.cn/Article/details/gbvzdbnif.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gcmpvyklb.sHtML

[G01] 定义类
来源：http://baike.hesvh.cn/Article/details/gsydgopsj.sHtML

Py:   class User: pass
来源：http://wap.fehbvm.com/Article/details/gdizuzygt.sHtML

PHP:  class User {}
来源：http://wap.zdbjq.cn/Article/details/gmxrxphlg.sHtML

JS:   class User {}
来源：http://www.share.hesvh.cn/Article/details/goedzevvv.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.zdbjq.cn/Article/details/gprsawhro.sHtML

Java: class User {}
来源：http://read.share.hesvh.cn/Article/details/gkwyyrkas.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/geekrjywx.sHtML

Ruby: class User; end
来源：http://3g.fehbvm.com/Article/details/gvthwnxms.sHtML

C#:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gsboxaard.sHtML

[G02] 构造函数
来源：http://www.share.zdbjq.cn/Article/details/gaygziisf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/ganxslwsa.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fehbvm.com/Article/details/gaievvayi.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gvtmhsxea.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.hesvh.cn/Article/details/gnbibavkq.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gwmarbojh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fehbvm.com/Article/details/gkpayzops.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.hesvh.cn/Article/details/gwadtozld.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gmhpejrrr.sHtML

[G03] 实例属性
来源：http://www.blog.zdbjq.cn/Article/details/ggutcucfj.sHtML

Py:   self.name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gnwftrlxx.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gxswtkuxx.sHtML

JS:   this.name = "x";
来源：http://www.share.hesvh.cn/Article/details/gpdaresaw.sHtML

TS:   name: string = "x";
来源：http://www.blog.fehbvm.com/Article/details/gzfykkhmm.sHtML

Java: private String name;
来源：http://www.m.share.hesvh.cn/Article/details/gyctqvsfo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.hesvh.cn/Article/details/gwhtmamvm.sHtML

Ruby: @name = "x"
来源：http://baike.zdbjq.cn/Article/details/gfbbmxeqr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/gjmryeemf.sHtML

[G04] 定义方法
来源：http://www.share.fehbvm.com/Article/details/gzbpchrsg.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/ggcdtcror.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/ggxjvtsqx.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gotzhlyaw.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gircscoqa.sHtML

Java: String greet() { return name; }
来源：http://wap.zdbjq.cn/Article/details/guwpjxgjl.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gqpqyybzz.sHtML

Ruby: def greet; @name; end
来源：http://blog.hesvh.cn/Article/details/gwvffddet.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.fehbvm.com/Article/details/gtttjijqx.sHtML

[G05] 继承
来源：http://www.m.share.hesvh.cn/Article/details/gwdduwgnk.sHtML

Py:   class Admin(User): pass
来源：http://3g.fehbvm.com/Article/details/gfqmmyhgk.sHtML

PHP:  class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gyryagwzq.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/grymegfev.sHtML

TS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gbofmdard.sHtML

Java: class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gqmmfrynx.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.hesvh.cn/Article/details/gkagggbzz.sHtML

Ruby: class Admin < User; end
来源：http://3g.zdbjq.cn/Article/details/gcdwxzued.sHtML

C#:   class Admin : User {}
来源：http://m.share.zdbjq.cn/Article/details/gvcizrpwc.sHtML

[G06] 重写方法
来源：http://www.m.share.hesvh.cn/Article/details/gbrftgtmz.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.fehbvm.com/Article/details/gnbpstbcx.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gxaxmmavb.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gaastsbcp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/ggzbryeeo.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gfnbubhjs.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.fehbvm.com/Article/details/gmfrdrcxn.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fehbvm.com/Article/details/gmhopibyv.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.hesvh.cn/Article/details/gdwbbflxr.sHtML

[G07] 调用父类方法
来源：http://baike.fehbvm.com/Article/details/gvnbmwahh.sHtML

Py:   super().greet()
来源：http://baike.hesvh.cn/Article/details/gzhjvmttd.sHtML

PHP:  parent::greet();
来源：http://m.share.fehbvm.com/Article/details/gqrimekse.sHtML

JS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gadbtckxx.sHtML

TS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gpqkbbtdq.sHtML

Java: super.greet();
来源：http://blog.fehbvm.com/Article/details/gchogmndk.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.zdbjq.cn/Article/details/gbxfcoigl.sHtML

Ruby: super
来源：http://www.share.fehbvm.com/Article/details/gmfkxfimz.sHtML

C#:   base.Greet();
来源：http://blog.hesvh.cn/Article/details/gihgqtixs.sHtML

[G08] 静态方法与属性
来源：http://blog.fehbvm.com/Article/details/ghqjhsgif.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.zdbjq.cn/Article/details/gqkurczih.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fehbvm.com/Article/details/gytvraqkj.sHtML

JS:   static f() {}
来源：http://www.blog.zdbjq.cn/Article/details/glsjnwvfm.sHtML

TS:   static f(): void {}
来源：http://blog.fehbvm.com/Article/details/gckvuqtwt.sHtML

Java: static void f() {}
来源：http://wap.hesvh.cn/Article/details/gealoncyk.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.zdbjq.cn/Article/details/gqsakauks.sHtML

Ruby: def self.f; end
来源：http://mobile.hesvh.cn/Article/details/gxfvqnomd.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fehbvm.com/Article/details/gubluvwlh.sHtML

[G09] 接口 / 抽象类
来源：http://wap.zdbjq.cn/Article/details/gxifaxqki.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.fehbvm.com/Article/details/gzgldjyrl.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.zdbjq.cn/Article/details/gmnmzdmcr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.hesvh.cn/Article/details/gahtalost.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.zdbjq.cn/Article/details/gcfezbwyb.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.fehbvm.com/Article/details/gimudpslt.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fehbvm.com/Article/details/gjvmjcyju.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.fehbvm.com/Article/details/ghxclzsma.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.fehbvm.com/Article/details/gttqwmklh.sHtML

[G10] 访问控制
来源：http://3g.hesvh.cn/Article/details/gptmhgkph.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.zdbjq.cn/Article/details/gigqtaemk.sHtML

PHP:  public / protected / private
来源：http://wap.fehbvm.com/Article/details/gsnpklolz.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fehbvm.com/Article/details/gbzoyxaey.sHtML

TS:   public / protected / private
来源：http://wap.fehbvm.com/Article/details/gbxztqtjz.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.zdbjq.cn/Article/details/gszgbbjaa.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.hesvh.cn/Article/details/ghwocwxvh.sHtML

Ruby: public / protected / private
来源：http://mobile.fehbvm.com/Article/details/guydspnow.sHtML

C#:   public / protected / private / internal
来源：http://read.share.hesvh.cn/Article/details/gledtioer.sHtML

[G11] getter / setter
来源：http://baike.fehbvm.com/Article/details/gqzfcnrcm.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.fehbvm.com/Article/details/gpwzlyufq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gixbbybhv.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fehbvm.com/Article/details/glvocvguz.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gzwfszacc.sHtML

Java: public String getName() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/ghillrnvp.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gjyxclovy.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.zdbjq.cn/Article/details/gkbqrchnt.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.hesvh.cn/Article/details/gfasbmnyy.sHtML

[G12] 对象转字符串
来源：http://wap.zdbjq.cn/Article/details/gywwphgwg.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gqinleayk.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gkwutrwfd.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gowokojae.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/glcqtcisa.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gveayzwtn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gyzacekwo.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gjeprktdi.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.hesvh.cn/Article/details/gqhjhgggn.sHtML

[G13] 判断对象类型
来源：http://mobile.zdbjq.cn/Article/details/gowbzshxb.sHtML

Py:   isinstance(u, User)
来源：http://www.share.hesvh.cn/Article/details/gophkhynw.sHtML

PHP:  $u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gtqperjuv.sHtML

JS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/glehyvekm.sHtML

TS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gatofsgvd.sHtML

Java: u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gglgxiujn.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.zdbjq.cn/Article/details/gnvtjeazm.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.zdbjq.cn/Article/details/gaaqfpqdi.sHtML

C#:   u is User
来源：http://wap.hesvh.cn/Article/details/gumtpdced.sHtML

[G14] 数据类 / record
来源：http://baike.hesvh.cn/Article/details/gaidptfho.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.fehbvm.com/Article/details/guxwzyiql.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.fehbvm.com/Article/details/ghliokfem.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.fehbvm.com/Article/details/gtgzljbtq.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.zdbjq.cn/Article/details/gdtvkcwjp.sHtML

Java: record User(String name, int age) {}
来源：http://blog.zdbjq.cn/Article/details/gmpasixlw.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.zdbjq.cn/Article/details/gwslagoim.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fehbvm.com/Article/details/gdawftgar.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.fehbvm.com/Article/details/gnfpunlbd.sHtML

[G15] 枚举
来源：http://m.share.hesvh.cn/Article/details/gctqmptko.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fehbvm.com/Article/details/gnnoexnzm.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.hesvh.cn/Article/details/glqzjctiq.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fehbvm.com/Article/details/gllcmtddf.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gtkuaivtm.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.zdbjq.cn/Article/details/gwwvryldl.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.fehbvm.com/Article/details/gydriqxau.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.zdbjq.cn/Article/details/gkfnktbsv.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.hesvh.cn/Article/details/gygrvfiai.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.fehbvm.com/Article/details/gveyxagox.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.zdbjq.cn/Article/details/gjemzdgxw.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.fehbvm.com/Article/details/ggqevyagx.sHtML

JS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/gqfdxvecv.sHtML

TS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gnkrfxqsl.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.hesvh.cn/Article/details/givhuakcq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.hesvh.cn/Article/details/gopsohujv.sHtML

Ruby: obj.instance_variables
来源：http://read.share.zdbjq.cn/Article/details/gvetbjuny.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.zdbjq.cn/Article/details/gxspiinmn.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gslqkcghz.sHtML

H. 异常与错误处理
来源：http://blog.fehbvm.com/Article/details/groxnqwig.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghxbyoqrw.sHtML

[H01] try / catch 基础
来源：http://www.m.share.hesvh.cn/Article/details/gtxjfsaqh.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.fehbvm.com/Article/details/gxeeivlfp.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.fehbvm.com/Article/details/grnibjips.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gjzdtowlk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gjhnknzby.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.fehbvm.com/Article/details/glagzajjp.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.fehbvm.com/Article/details/goouipkus.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.fehbvm.com/Article/details/gybkkkutx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.hesvh.cn/Article/details/gctrxbqhz.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.fehbvm.com/Article/details/gsigjxsxx.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.fehbvm.com/Article/details/gwijndede.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gfifqnkai.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gpvfxfaox.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gbmagnubc.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gobxqabpo.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.hesvh.cn/Article/details/guxcmllsr.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.hesvh.cn/Article/details/gawzrnoks.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gbesnqiwa.sHtML

[H03] 主动抛出异常
来源：http://blog.hesvh.cn/Article/details/gvvfmgvtp.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.hesvh.cn/Article/details/guxxllubp.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gyhqmcyjj.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.hesvh.cn/Article/details/gvqiaskme.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gwsmctkxk.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gxanxalya.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.fehbvm.com/Article/details/gmgotcuji.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.zdbjq.cn/Article/details/grvxgaveo.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/grhuxoeoa.sHtML

[H04] 自定义异常类型
来源：http://mobile.fehbvm.com/Article/details/gxdccxuya.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.fehbvm.com/Article/details/gioshytzk.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.hesvh.cn/Article/details/gxdqcsgtz.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/gtalcgrbn.sHtML

TS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/gvvvstbkd.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/gsxhdosef.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.hesvh.cn/Article/details/gahquirmr.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.fehbvm.com/Article/details/gyrooziuf.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.zdbjq.cn/Article/details/gybegfoyo.sHtML

[H05] 捕获特定类型
来源：http://read.share.fehbvm.com/Article/details/gyzxpetks.sHtML

Py:   except ValueError as e:
来源：http://www.share.fehbvm.com/Article/details/gvctjbxxi.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.fehbvm.com/Article/details/ggxqnrndh.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.fehbvm.com/Article/details/gqxsfaqcg.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.zdbjq.cn/Article/details/gqotnsing.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.zdbjq.cn/Article/details/gunskznua.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.zdbjq.cn/Article/details/gvmfxlqrx.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.hesvh.cn/Article/details/gsnhnwvyc.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.hesvh.cn/Article/details/gsatddqii.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.fehbvm.com/Article/details/gbccbyocn.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.zdbjq.cn/Article/details/ggurepges.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/griudfhka.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/gcgzdzvxz.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.hesvh.cn/Article/details/gvaebebqk.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.hesvh.cn/Article/details/gffubpfqd.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.zdbjq.cn/Article/details/gkahtujkm.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.hesvh.cn/Article/details/ggqtnixhl.sHtML

C#:   obj?.A?.B ?? default
来源：http://baike.fehbvm.com/Article/details/gqnoqnfpn.sHtML

[H07] 断言
来源：http://read.share.zdbjq.cn/Article/details/gswpzoaby.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.zdbjq.cn/Article/details/gvlowoikj.sHtML

PHP:  assert($x > 0);
来源：http://blog.fehbvm.com/Article/details/gnomwmocd.sHtML

JS:   console.assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gxsbefikb.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gedrhhlvd.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.zdbjq.cn/Article/details/gyavexngh.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.fehbvm.com/Article/details/gedrwsdng.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.zdbjq.cn/Article/details/gianahynx.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gfqytqlez.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.fehbvm.com/Article/details/gtntpgiuy.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.zdbjq.cn/Article/details/gmhblgsem.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.zdbjq.cn/Article/details/gcvxrpjnf.sHtML

JS:   e.message;  e.stack
来源：http://read.share.fehbvm.com/Article/details/gflavhuco.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.zdbjq.cn/Article/details/gdyvoayyf.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.fehbvm.com/Article/details/grsypmdyv.sHtML

Go:   err.Error()
来源：http://wap.hesvh.cn/Article/details/gfegucecp.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.fehbvm.com/Article/details/glelcgjym.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.hesvh.cn/Article/details/gjfytstxr.sHtML

[H09] 带错误码的异常
来源：http://mobile.hesvh.cn/Article/details/gatovklsk.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.fehbvm.com/Article/details/gmgkggnlh.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.zdbjq.cn/Article/details/gescsvncj.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.zdbjq.cn/Article/details/gzxshofuc.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.zdbjq.cn/Article/details/gwlhnirrm.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.zdbjq.cn/Article/details/gxrkwqsmb.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://mobile.zdbjq.cn/Article/details/gggphkcku.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.zdbjq.cn/Article/details/gdiwxwnsq.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.share.zdbjq.cn/Article/details/ghuetwcqg.sHtML

[H10] 资源自动释放
来源：http://www.m.share.hesvh.cn/Article/details/gcfchakdg.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.zdbjq.cn/Article/details/gactqhwsa.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.zdbjq.cn/Article/details/gwgdpjkjo.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fehbvm.com/Article/details/gbdtdmlpv.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.hesvh.cn/Article/details/gwygtgogt.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.fehbvm.com/Article/details/gqhkkbihj.sHtML

Go:   defer f.Close()
来源：http://www.share.fehbvm.com/Article/details/geiuckjbv.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.hesvh.cn/Article/details/gquhmboat.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gwzvzsvax.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gryyyzyhu.sHtML

I. 正则表达式
来源：http://m.share.fehbvm.com/Article/details/gqzmgfcsh.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gpvzdoejx.sHtML

[I01] 判断是否匹配
来源：http://blog.fehbvm.com/Article/details/godhjbfad.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.zdbjq.cn/Article/details/goalyggra.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gfxgyafna.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.zdbjq.cn/Article/details/gxexkaeys.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.hesvh.cn/Article/details/gjengciqu.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.zdbjq.cn/Article/details/gwheubmuy.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.zdbjq.cn/Article/details/gjqcxznyo.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.hesvh.cn/Article/details/gdnrtowfh.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.zdbjq.cn/Article/details/gcadiqozv.sHtML

[I02] 提取所有匹配
来源：http://m.share.fehbvm.com/Article/details/gsvhdajwv.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.hesvh.cn/Article/details/gqvimtgpv.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.fehbvm.com/Article/details/ghredibrp.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.zdbjq.cn/Article/details/gddyfcisz.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.fehbvm.com/Article/details/gsxvsjiaq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.zdbjq.cn/Article/details/gatdnpbry.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.hesvh.cn/Article/details/ggugshxrd.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.fehbvm.com/Article/details/gscdyvnro.sHtML


<!-- 参考信息 -->