代发 wailian999

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.fehbvm.com/Article/details/gunuloqwl.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.zdbjq.cn/Article/details/gecbnsyao.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/gurgxxmjs.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gbzdtyuji.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gjuqrenbk.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gnqctvjvs.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gcaouwloo.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.hesvh.cn/Article/details/gavdvchwp.sHtML

[F09] 获取文件大小
来源：http://baike.fehbvm.com/Article/details/gticplsrq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gknzxljzf.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gqrmkppzo.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gctjftccs.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/ghejfjwcj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gimzieoce.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.zdbjq.cn/Article/details/gknppieqg.sHtML

Ruby: File.size("a.txt")
来源：http://baike.fehbvm.com/Article/details/gshcdemka.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.hesvh.cn/Article/details/godwccgot.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.zdbjq.cn/Article/details/gcwrvzyjd.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/goutjuiap.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fehbvm.com/Article/details/gkdebcbyv.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gqiiyrdxc.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gembwiten.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.hesvh.cn/Article/details/guhpxoani.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gtrcjkhnn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gapyuaaru.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gyydxuvwc.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.fehbvm.com/Article/details/gzjgrlktb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gpfaltkcb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.fehbvm.com/Article/details/gbfbrmuin.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gdwhdicsm.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gzyonzfqp.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gdgxmowpx.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.fehbvm.com/Article/details/ggodlptkq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gdujjdubg.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.zdbjq.cn/Article/details/gatsepksi.sHtML

[F12] CSV 读写
来源：http://www.m.share.hesvh.cn/Article/details/gjoyfdpil.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.zdbjq.cn/Article/details/gdtghynsc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fehbvm.com/Article/details/gkcsehzqk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.fehbvm.com/Article/details/gfkwvhlfc.sHtML

TS:   // 同上
来源：http://www.blog.hesvh.cn/Article/details/gopehvxbe.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.zdbjq.cn/Article/details/grwdujhke.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.zdbjq.cn/Article/details/gnoiutsep.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.zdbjq.cn/Article/details/gjbwsqjkn.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fehbvm.com/Article/details/gzfvdleaf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gtudxuqda.sHtML

G. 面向对象
来源：http://3g.fehbvm.com/Article/details/gefhlabwh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gigoinmja.sHtML

[G01] 定义类
来源：http://blog.fehbvm.com/Article/details/gjsyupbky.sHtML

Py:   class User: pass
来源：http://blog.hesvh.cn/Article/details/gxgidwafq.sHtML

PHP:  class User {}
来源：http://read.share.hesvh.cn/Article/details/ggkuuqfbx.sHtML

JS:   class User {}
来源：http://3g.fehbvm.com/Article/details/gitliosud.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/ggnudhtwx.sHtML

Java: class User {}
来源：http://m.share.hesvh.cn/Article/details/gjvpwsbst.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/gdcwqxurc.sHtML

Ruby: class User; end
来源：http://wap.zdbjq.cn/Article/details/gbkwywaeh.sHtML

C#:   class User {}
来源：http://blog.fehbvm.com/Article/details/gentlazxl.sHtML

[G02] 构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gurdpbhfx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.hesvh.cn/Article/details/grmhhfqas.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.zdbjq.cn/Article/details/gftiamisn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gbdyxsyyj.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fehbvm.com/Article/details/gjcgkiwvm.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gkfigsiwb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.zdbjq.cn/Article/details/gmlfextbh.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.zdbjq.cn/Article/details/grwwsypat.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fehbvm.com/Article/details/gpyxzifbl.sHtML

[G03] 实例属性
来源：http://www.blog.hesvh.cn/Article/details/gcvjbqbsi.sHtML

Py:   self.name = "x"
来源：http://read.share.hesvh.cn/Article/details/gwnhbyhva.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gmdlrucyn.sHtML

JS:   this.name = "x";
来源：http://wap.zdbjq.cn/Article/details/goxiqfzot.sHtML

TS:   name: string = "x";
来源：http://blog.fehbvm.com/Article/details/ghiqnbzhb.sHtML

Java: private String name;
来源：http://wap.hesvh.cn/Article/details/gpjtanigj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.hesvh.cn/Article/details/gttmnsaao.sHtML

Ruby: @name = "x"
来源：http://mobile.fehbvm.com/Article/details/gjlsuxayl.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.hesvh.cn/Article/details/gjhtvlcxi.sHtML

[G04] 定义方法
来源：http://www.blog.fehbvm.com/Article/details/gudycrdso.sHtML

Py:   def greet(self): return self.name
来源：http://3g.fehbvm.com/Article/details/gsxczaguc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gdvkiduim.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gvpmyxquu.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/giuaydekm.sHtML

Java: String greet() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gpspgetpl.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gvlieomgq.sHtML

Ruby: def greet; @name; end
来源：http://wap.fehbvm.com/Article/details/guchweygr.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.hesvh.cn/Article/details/gmylaobvr.sHtML

[G05] 继承
来源：http://wap.zdbjq.cn/Article/details/geszzyxxz.sHtML

Py:   class Admin(User): pass
来源：http://3g.hesvh.cn/Article/details/gykehgyvf.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gcgvspdog.sHtML

JS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gntlzrvvp.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/grjqtbaaz.sHtML

Java: class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gnqrybnyp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.hesvh.cn/Article/details/gsgjtaubg.sHtML

Ruby: class Admin < User; end
来源：http://baike.zdbjq.cn/Article/details/gcrpnsfzz.sHtML

C#:   class Admin : User {}
来源：http://wap.hesvh.cn/Article/details/gjqyvjucm.sHtML

[G06] 重写方法
来源：http://www.share.hesvh.cn/Article/details/gurhltzko.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.fehbvm.com/Article/details/gmqxgoaxe.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gjssbheej.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gpkgxpqjn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/grbjsecmk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gwdtucsyv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.zdbjq.cn/Article/details/gsdihmptl.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.fehbvm.com/Article/details/girfixdpc.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.hesvh.cn/Article/details/ggxbyymty.sHtML

[G07] 调用父类方法
来源：http://wap.hesvh.cn/Article/details/gcjjknoiz.sHtML

Py:   super().greet()
来源：http://blog.hesvh.cn/Article/details/gpcktkfyp.sHtML

PHP:  parent::greet();
来源：http://www.share.fehbvm.com/Article/details/giaulrhwa.sHtML

JS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gkndrvbuy.sHtML

TS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gxbfgctzj.sHtML

Java: super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gbreyssqn.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.fehbvm.com/Article/details/guamtevbh.sHtML

Ruby: super
来源：http://www.blog.fehbvm.com/Article/details/gxxktjmon.sHtML

C#:   base.Greet();
来源：http://www.share.hesvh.cn/Article/details/gycmqzkvh.sHtML

[G08] 静态方法与属性
来源：http://www.blog.zdbjq.cn/Article/details/gpunkuwpp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.zdbjq.cn/Article/details/gyyxkzviq.sHtML

PHP:  public static function f() {}
来源：http://3g.hesvh.cn/Article/details/gklbikfri.sHtML

JS:   static f() {}
来源：http://blog.hesvh.cn/Article/details/gjvcfxvhf.sHtML

TS:   static f(): void {}
来源：http://wap.hesvh.cn/Article/details/gomvazczi.sHtML

Java: static void f() {}
来源：http://wap.hesvh.cn/Article/details/gslmftzfb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.hesvh.cn/Article/details/ggtptddiy.sHtML

Ruby: def self.f; end
来源：http://wap.hesvh.cn/Article/details/ggkjrlyvj.sHtML

C#:   public static void F() {}
来源：http://m.share.hesvh.cn/Article/details/guvfsazjg.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.fehbvm.com/Article/details/gfbfldfvy.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.zdbjq.cn/Article/details/grohytpvm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fehbvm.com/Article/details/gmnnexxlm.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.fehbvm.com/Article/details/gvgeptnql.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.zdbjq.cn/Article/details/grtacbqmj.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.hesvh.cn/Article/details/gwoymsomz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.hesvh.cn/Article/details/gohhfhtll.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.zdbjq.cn/Article/details/ghzfdqpav.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.zdbjq.cn/Article/details/gmpyqhjdn.sHtML

[G10] 访问控制
来源：http://read.share.zdbjq.cn/Article/details/ggwdhiyfp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fehbvm.com/Article/details/geomjozlr.sHtML

PHP:  public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gjnlkzwtj.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.fehbvm.com/Article/details/gmjsfsehn.sHtML

TS:   public / protected / private
来源：http://baike.hesvh.cn/Article/details/gnsavwgqp.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.hesvh.cn/Article/details/greinohhz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.zdbjq.cn/Article/details/gzsdyccma.sHtML

Ruby: public / protected / private
来源：http://blog.hesvh.cn/Article/details/gkonmtzxn.sHtML

C#:   public / protected / private / internal
来源：http://wap.hesvh.cn/Article/details/gkxqktmdt.sHtML

[G11] getter / setter
来源：http://blog.hesvh.cn/Article/details/gzbsyoeoi.sHtML

Py:   @property 与 @x.setter
来源：http://baike.fehbvm.com/Article/details/grpktywzi.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/giebdcdod.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gpjzmyxup.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gagwuxgjq.sHtML

Java: public String getName() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/ggghcbpkj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/guguyhbxa.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.hesvh.cn/Article/details/gyiaivnpe.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.hesvh.cn/Article/details/grmheukmp.sHtML

[G12] 对象转字符串
来源：http://read.share.fehbvm.com/Article/details/gmzqreanm.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gnwjcbeyv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gyoxzrath.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/glrjyvxck.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gccpsrwui.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gluemyjfy.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gyhnyefrk.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fehbvm.com/Article/details/gevfyycbh.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.hesvh.cn/Article/details/gqczucugk.sHtML

[G13] 判断对象类型
来源：http://www.share.zdbjq.cn/Article/details/goizrovae.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.hesvh.cn/Article/details/gfcdxnshm.sHtML

PHP:  $u instanceof User
来源：http://baike.hesvh.cn/Article/details/ghblcaxxd.sHtML

JS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gtcyodciy.sHtML

TS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gchzxwjfk.sHtML

Java: u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gejtnwxdy.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fehbvm.com/Article/details/gasxiphxr.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.hesvh.cn/Article/details/gbvvmymow.sHtML

C#:   u is User
来源：http://www.share.hesvh.cn/Article/details/gpbnsczcr.sHtML

[G14] 数据类 / record
来源：http://www.share.fehbvm.com/Article/details/gdkocvgxn.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.hesvh.cn/Article/details/gcpfnvwgg.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.hesvh.cn/Article/details/grfredjsm.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.zdbjq.cn/Article/details/gbspnmzmd.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.fehbvm.com/Article/details/gksklhxju.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.hesvh.cn/Article/details/gcxssoatq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.zdbjq.cn/Article/details/ghrfibjyz.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.hesvh.cn/Article/details/gyshdhdka.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.hesvh.cn/Article/details/gcilbcnlg.sHtML

[G15] 枚举
来源：http://read.share.zdbjq.cn/Article/details/gmmynkphm.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.fehbvm.com/Article/details/gwyxlcrzq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.fehbvm.com/Article/details/gagfywwhf.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.zdbjq.cn/Article/details/gjoecalmu.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gxbvivcrj.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.hesvh.cn/Article/details/gpcdxyice.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.fehbvm.com/Article/details/gsgiuwitc.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.hesvh.cn/Article/details/gidrwyuie.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gydmvhykt.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.hesvh.cn/Article/details/gwukthtfj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fehbvm.com/Article/details/glhxqmlwx.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.fehbvm.com/Article/details/gefwpakyd.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.fehbvm.com/Article/details/gskdfgymo.sHtML

TS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/gboscrylt.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.fehbvm.com/Article/details/gwligvqpk.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.fehbvm.com/Article/details/gnerzchxr.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.zdbjq.cn/Article/details/gxyyocslq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/gkfrzebyr.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gsduacryb.sHtML

H. 异常与错误处理
来源：http://www.share.fehbvm.com/Article/details/guzasvsli.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/groarisvk.sHtML

[H01] try / catch 基础
来源：http://read.share.hesvh.cn/Article/details/gzfvnlsuf.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.fehbvm.com/Article/details/goclsillz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.zdbjq.cn/Article/details/gmwsoepow.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gthmhmrwg.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/ganwsswvx.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.zdbjq.cn/Article/details/gfnnphqmn.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.hesvh.cn/Article/details/gkhdjfjoz.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.fehbvm.com/Article/details/gihkahiau.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.hesvh.cn/Article/details/gottkwkhv.sHtML

[H02] finally / ensure 收尾
来源：http://wap.fehbvm.com/Article/details/gpwkcncyh.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.fehbvm.com/Article/details/goejcatrm.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/glzqexpmb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/guyhjmadw.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gmicwpmpw.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gctntxocc.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.hesvh.cn/Article/details/ggzyebxnw.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.zdbjq.cn/Article/details/gskjxphlo.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/grbigzdzp.sHtML

[H03] 主动抛出异常
来源：http://www.share.hesvh.cn/Article/details/gkseqnzbz.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.hesvh.cn/Article/details/gbjmhycgs.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/geydsjmrw.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gmaxpynct.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gdaecaejh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gniyicsxe.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.fehbvm.com/Article/details/gaxirqvfq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.hesvh.cn/Article/details/guujzauwq.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gudcavxrc.sHtML

[H04] 自定义异常类型
来源：http://www.share.zdbjq.cn/Article/details/gmbptgmme.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.zdbjq.cn/Article/details/gyivgccwh.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/gdtroiulj.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/gwdjwawuf.sHtML

TS:   class MyError extends Error {}
来源：http://3g.fehbvm.com/Article/details/guczwpbod.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/gscnczgsi.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.hesvh.cn/Article/details/gqrtwnlze.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.zdbjq.cn/Article/details/gawiwdoag.sHtML

C#:   class MyException : Exception {}
来源：http://blog.fehbvm.com/Article/details/gvtmkyugq.sHtML

[H05] 捕获特定类型
来源：http://blog.fehbvm.com/Article/details/goeigqkop.sHtML

Py:   except ValueError as e:
来源：http://blog.zdbjq.cn/Article/details/gdzttzegw.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.zdbjq.cn/Article/details/gyxknzqfn.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/gsovswpok.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/gldgxucti.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.fehbvm.com/Article/details/gjohfnmuk.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.zdbjq.cn/Article/details/gzpzzcjjp.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.zdbjq.cn/Article/details/gdgxasczv.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.hesvh.cn/Article/details/gzailacdh.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.zdbjq.cn/Article/details/gxsqcybgk.sHtML

Py:   value = d.get("k") or default
来源：http://3g.fehbvm.com/Article/details/grefigage.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.fehbvm.com/Article/details/ghacrinas.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.hesvh.cn/Article/details/gkzxjwvuf.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.hesvh.cn/Article/details/gqxkywcni.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.zdbjq.cn/Article/details/gwgjslour.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.fehbvm.com/Article/details/geeqddyeh.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.zdbjq.cn/Article/details/gvjcfkihk.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.hesvh.cn/Article/details/gawxcgrwi.sHtML

[H07] 断言
来源：http://wap.zdbjq.cn/Article/details/godbxbbzz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.hesvh.cn/Article/details/ghgdfafsw.sHtML

PHP:  assert($x > 0);
来源：http://www.share.fehbvm.com/Article/details/geidvouxl.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gtqitfdlu.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gpcaqepib.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.fehbvm.com/Article/details/ghexmdvzn.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.zdbjq.cn/Article/details/gozhhvjii.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.zdbjq.cn/Article/details/gyhqakgnx.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/ggxdicbrq.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.hesvh.cn/Article/details/gaexidlcd.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.hesvh.cn/Article/details/glsvchzba.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.fehbvm.com/Article/details/gyfvuarxr.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.fehbvm.com/Article/details/gvrhrkokn.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.zdbjq.cn/Article/details/gzhhsysiy.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.hesvh.cn/Article/details/gevefhsfb.sHtML

Go:   err.Error()
来源：http://wap.fehbvm.com/Article/details/gsljldlsx.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.zdbjq.cn/Article/details/guywkeglf.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.hesvh.cn/Article/details/gxphibokb.sHtML

[H09] 带错误码的异常
来源：http://www.share.hesvh.cn/Article/details/ggaovvdql.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.hesvh.cn/Article/details/gqazztjsi.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.fehbvm.com/Article/details/gsgljwjjk.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.hesvh.cn/Article/details/gumdshbpe.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.fehbvm.com/Article/details/guqrvgdog.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.fehbvm.com/Article/details/gtlikgrvq.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.zdbjq.cn/Article/details/gifckapgl.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://3g.zdbjq.cn/Article/details/gwmnhwlam.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.fehbvm.com/Article/details/giepmjgse.sHtML

[H10] 资源自动释放
来源：http://3g.zdbjq.cn/Article/details/ghnewsvrg.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.hesvh.cn/Article/details/gmazwhbql.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.fehbvm.com/Article/details/gomerrtfs.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.hesvh.cn/Article/details/gholxkcea.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.zdbjq.cn/Article/details/gqeryxsus.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.hesvh.cn/Article/details/gfkvpbdfc.sHtML

Go:   defer f.Close()
来源：http://read.share.hesvh.cn/Article/details/gjqvpdewi.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.fehbvm.com/Article/details/gxxnmvrkk.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.hesvh.cn/Article/details/geedsmmwa.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gduhwiojk.sHtML

I. 正则表达式
来源：http://read.share.zdbjq.cn/Article/details/gyzcnwfeu.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gonbkxwxr.sHtML

[I01] 判断是否匹配
来源：http://mobile.hesvh.cn/Article/details/ghhcuevea.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.zdbjq.cn/Article/details/gpwmpstho.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.fehbvm.com/Article/details/gizwgvpms.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.hesvh.cn/Article/details/gybzqhpxh.sHtML

TS:   /\d+/.test(s)
来源：http://blog.fehbvm.com/Article/details/gijxdindl.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.zdbjq.cn/Article/details/gdajmuind.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.zdbjq.cn/Article/details/gaksqdxgq.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.zdbjq.cn/Article/details/gkkahlgsb.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.zdbjq.cn/Article/details/gsvfaxioa.sHtML

[I02] 提取所有匹配
来源：http://www.blog.zdbjq.cn/Article/details/gbpyzdgbo.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.hesvh.cn/Article/details/gnjnrlndp.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.fehbvm.com/Article/details/ghicdgeqa.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.zdbjq.cn/Article/details/gyxgmtggz.sHtML


<!-- 参考信息 -->