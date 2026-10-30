代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gstdkagpd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.fehbvm.com/Article/details/gkvhtvncs.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gtotiezpm.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.hesvh.cn/Article/details/gzyzsgmro.sHtML

[F09] 获取文件大小
来源：http://blog.zdbjq.cn/Article/details/giwldydwl.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gomgrpfec.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gkgcvbibs.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/gjizmodzq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gsvtnoqtn.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gvszpobzd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fehbvm.com/Article/details/gwiszwsdz.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gcsrprink.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.zdbjq.cn/Article/details/gxybwjqri.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.zdbjq.cn/Article/details/grrtaixuj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/geckwbbqw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.hesvh.cn/Article/details/gbwvpkidx.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gbpegzadf.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gixgbgxti.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.hesvh.cn/Article/details/govcfjupm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gtorzlbxl.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/grbnhoapx.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gljgqlmcj.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.fehbvm.com/Article/details/grdmcjuew.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gsyxzrjqq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.hesvh.cn/Article/details/gzfforpaj.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gejkfubkg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gzuislvau.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.fehbvm.com/Article/details/gbgatgtfi.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.zdbjq.cn/Article/details/gtwkpniob.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/grwdsdirw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.hesvh.cn/Article/details/gcgikwwoq.sHtML

[F12] CSV 读写
来源：http://www.m.share.zdbjq.cn/Article/details/gvbnelido.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.zdbjq.cn/Article/details/guolmltop.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.zdbjq.cn/Article/details/gphlzuypw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.zdbjq.cn/Article/details/galbuzxmr.sHtML

TS:   // 同上
来源：http://www.blog.hesvh.cn/Article/details/gafjebiqq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.fehbvm.com/Article/details/gmckxzssp.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.zdbjq.cn/Article/details/gwrufacvn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.zdbjq.cn/Article/details/gawfhmfhh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fehbvm.com/Article/details/grgjfouwj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtffxotmb.sHtML

G. 面向对象
来源：http://mobile.zdbjq.cn/Article/details/ghnadrtsk.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gkdulkfhd.sHtML

[G01] 定义类
来源：http://mobile.fehbvm.com/Article/details/gqjnxtldj.sHtML

Py:   class User: pass
来源：http://m.share.hesvh.cn/Article/details/gejjtawqz.sHtML

PHP:  class User {}
来源：http://wap.fehbvm.com/Article/details/gxymjybda.sHtML

JS:   class User {}
来源：http://read.share.fehbvm.com/Article/details/glsyirtba.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.zdbjq.cn/Article/details/giskvmgvv.sHtML

Java: class User {}
来源：http://3g.fehbvm.com/Article/details/ggqkvanva.sHtML

Go:   type User struct { Name string }
来源：http://baike.fehbvm.com/Article/details/gigoecybx.sHtML

Ruby: class User; end
来源：http://blog.fehbvm.com/Article/details/gniabaujp.sHtML

C#:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gjxwvpjid.sHtML

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/gkaqcmnkw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.fehbvm.com/Article/details/gcovdqnkl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.zdbjq.cn/Article/details/gqmabjlvo.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gsjilmexj.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fehbvm.com/Article/details/gkaorqzje.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gwexntvtc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.zdbjq.cn/Article/details/ghcsizsqx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fehbvm.com/Article/details/gkqaczwpy.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gixtfndqc.sHtML

[G03] 实例属性
来源：http://mobile.fehbvm.com/Article/details/gxzncdngq.sHtML

Py:   self.name = "x"
来源：http://wap.zdbjq.cn/Article/details/govltzclu.sHtML

PHP:  public string $name = "x";
来源：http://3g.fehbvm.com/Article/details/gdarclnzh.sHtML

JS:   this.name = "x";
来源：http://m.share.hesvh.cn/Article/details/glesmmctf.sHtML

TS:   name: string = "x";
来源：http://m.share.zdbjq.cn/Article/details/gnzoncasf.sHtML

Java: private String name;
来源：http://wap.fehbvm.com/Article/details/glnczljfx.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fehbvm.com/Article/details/gvrxvdygd.sHtML

Ruby: @name = "x"
来源：http://mobile.zdbjq.cn/Article/details/ggrjdlfag.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fehbvm.com/Article/details/gvafcsjvy.sHtML

[G04] 定义方法
来源：http://read.share.fehbvm.com/Article/details/gzyxkekcq.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gogbjswqt.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/givvyjaml.sHtML

JS:   greet() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gwyvzfapo.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gofevwuvo.sHtML

Java: String greet() { return name; }
来源：http://wap.hesvh.cn/Article/details/gcgjiyqdo.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/ghugttykx.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gfdnfbiku.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gcuvbqdhd.sHtML

[G05] 继承
来源：http://blog.zdbjq.cn/Article/details/gdszlpngp.sHtML

Py:   class Admin(User): pass
来源：http://baike.hesvh.cn/Article/details/gxnwrspvr.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gbrwfxxcv.sHtML

JS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gavwseyfr.sHtML

TS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/grqcdzsqs.sHtML

Java: class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/glytplmaw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.zdbjq.cn/Article/details/gflqztmir.sHtML

Ruby: class Admin < User; end
来源：http://blog.fehbvm.com/Article/details/ghpvfhkhk.sHtML

C#:   class Admin : User {}
来源：http://baike.hesvh.cn/Article/details/gqcimfaea.sHtML

[G06] 重写方法
来源：http://www.blog.hesvh.cn/Article/details/grhokdmgr.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.fehbvm.com/Article/details/gtewscwlz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/ggfwbvkhm.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gziwjjmnt.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gfgxnvfkx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/glouvpqgo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.zdbjq.cn/Article/details/glgryvuzb.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fehbvm.com/Article/details/gaxgrxblb.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.hesvh.cn/Article/details/gayygaphd.sHtML

[G07] 调用父类方法
来源：http://3g.hesvh.cn/Article/details/gwedtdyts.sHtML

Py:   super().greet()
来源：http://blog.zdbjq.cn/Article/details/gmnibahbp.sHtML

PHP:  parent::greet();
来源：http://3g.zdbjq.cn/Article/details/godenhuuk.sHtML

JS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gycoppwig.sHtML

TS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gqzmhxrty.sHtML

Java: super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gbjsszvea.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.fehbvm.com/Article/details/gtwjfmeob.sHtML

Ruby: super
来源：http://www.share.zdbjq.cn/Article/details/glhuuhros.sHtML

C#:   base.Greet();
来源：http://baike.zdbjq.cn/Article/details/gotufshbw.sHtML

[G08] 静态方法与属性
来源：http://www.blog.zdbjq.cn/Article/details/gacnsxork.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.fehbvm.com/Article/details/grjktwwda.sHtML

PHP:  public static function f() {}
来源：http://www.blog.hesvh.cn/Article/details/ggwbqsimw.sHtML

JS:   static f() {}
来源：http://www.share.hesvh.cn/Article/details/gyxmtougl.sHtML

TS:   static f(): void {}
来源：http://mobile.hesvh.cn/Article/details/glwrwpxbx.sHtML

Java: static void f() {}
来源：http://www.blog.fehbvm.com/Article/details/gnuciapfn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.zdbjq.cn/Article/details/gasmvhngl.sHtML

Ruby: def self.f; end
来源：http://m.share.fehbvm.com/Article/details/gvozzyalm.sHtML

C#:   public static void F() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfqeualif.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.zdbjq.cn/Article/details/gklcndwgm.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.zdbjq.cn/Article/details/gonsvihgy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.fehbvm.com/Article/details/gvjqcbjca.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.hesvh.cn/Article/details/galqhszxu.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.hesvh.cn/Article/details/gsnsitkiz.sHtML

Java: interface Shape { double area(); }
来源：http://3g.hesvh.cn/Article/details/gawlozfby.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.zdbjq.cn/Article/details/gdemddjcu.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.zdbjq.cn/Article/details/ggsmgwjsu.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.hesvh.cn/Article/details/giqfksltw.sHtML

[G10] 访问控制
来源：http://www.m.share.hesvh.cn/Article/details/gvrnyhgcd.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.zdbjq.cn/Article/details/gxcnyfkkm.sHtML

PHP:  public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gwroyazzi.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.zdbjq.cn/Article/details/ginkfcwxw.sHtML

TS:   public / protected / private
来源：http://baike.fehbvm.com/Article/details/guzyvqllf.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.zdbjq.cn/Article/details/gmhzjgidm.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.hesvh.cn/Article/details/gqafzfpfm.sHtML

Ruby: public / protected / private
来源：http://3g.fehbvm.com/Article/details/gfmkgdztq.sHtML

C#:   public / protected / private / internal
来源：http://mobile.zdbjq.cn/Article/details/gbdsigomq.sHtML

[G11] getter / setter
来源：http://read.share.fehbvm.com/Article/details/gvttdugwh.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.fehbvm.com/Article/details/gdytljktx.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gajiwpjxw.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/grwfefgue.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/guuxqoiwj.sHtML

Java: public String getName() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gswbzzoum.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gbkuvharx.sHtML

Ruby: attr_accessor :name
来源：http://3g.zdbjq.cn/Article/details/gjawxzjlb.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fehbvm.com/Article/details/geccixvsj.sHtML

[G12] 对象转字符串
来源：http://wap.fehbvm.com/Article/details/gptdqmmty.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gfgahvqqq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gcwkobejm.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gpdmmovyz.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gsbpvdznd.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gggqrjyhw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gaxupaunc.sHtML

Ruby: def to_s; @name; end
来源：http://baike.zdbjq.cn/Article/details/gyxqrqvil.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.zdbjq.cn/Article/details/gqjpeohww.sHtML

[G13] 判断对象类型
来源：http://www.m.share.fehbvm.com/Article/details/gzhuvhgmd.sHtML

Py:   isinstance(u, User)
来源：http://blog.zdbjq.cn/Article/details/gtqbhvrqe.sHtML

PHP:  $u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gyotzijqx.sHtML

JS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gngdoyqls.sHtML

TS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gictlzckk.sHtML

Java: u instanceof User
来源：http://3g.zdbjq.cn/Article/details/giwcjzdcm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.hesvh.cn/Article/details/gmflmxxcf.sHtML

Ruby: u.is_a?(User)
来源：http://blog.zdbjq.cn/Article/details/ggbqyfztj.sHtML

C#:   u is User
来源：http://read.share.hesvh.cn/Article/details/gwnpncsck.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fehbvm.com/Article/details/gpcoggeug.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.zdbjq.cn/Article/details/gjiyzcauf.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.hesvh.cn/Article/details/gukutydag.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.hesvh.cn/Article/details/gphbdprcd.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.fehbvm.com/Article/details/gdzwuvnzv.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.zdbjq.cn/Article/details/gynvwyrqm.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.fehbvm.com/Article/details/gpjzqpzrk.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.hesvh.cn/Article/details/gkpryiolj.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.zdbjq.cn/Article/details/gjduqmlle.sHtML

[G15] 枚举
来源：http://baike.hesvh.cn/Article/details/gxlyurqkv.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.fehbvm.com/Article/details/gggslrzgr.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.hesvh.cn/Article/details/gdqmfodyh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.fehbvm.com/Article/details/gpfgzktlj.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/gzugzkcxp.sHtML

Java: enum Color { RED, GREEN }
来源：http://read.share.hesvh.cn/Article/details/gzcvignsl.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.fehbvm.com/Article/details/gviwvrwcc.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.fehbvm.com/Article/details/gazxpuadt.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/ghjaeqozk.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.hesvh.cn/Article/details/gttjpndbk.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.zdbjq.cn/Article/details/gkptylezq.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.zdbjq.cn/Article/details/gtzqanpgv.sHtML

JS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/ggnwgjiaa.sHtML

TS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gqwtpjyxw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.hesvh.cn/Article/details/ghiseqblu.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.hesvh.cn/Article/details/grhlcwghk.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.fehbvm.com/Article/details/ghwnwmfpr.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.fehbvm.com/Article/details/gzhofamiy.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gunijlzgw.sHtML

H. 异常与错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gcnmgqnxm.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gvclfzxrc.sHtML

[H01] try / catch 基础
来源：http://www.share.zdbjq.cn/Article/details/gihodtkes.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.fehbvm.com/Article/details/ghcvbefxg.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.zdbjq.cn/Article/details/gokyqbkkn.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gfmaruogc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gxyvpeorh.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.fehbvm.com/Article/details/gonpgyfrh.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.zdbjq.cn/Article/details/gjbhonqgs.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.zdbjq.cn/Article/details/gjsrhksec.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.zdbjq.cn/Article/details/gwwxutltx.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.hesvh.cn/Article/details/gwrkiezec.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.fehbvm.com/Article/details/glwmmarhe.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gmdjbsyra.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gqyfqcibh.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gneuixcrn.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gxfdnvwku.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.zdbjq.cn/Article/details/guvpcmqqv.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.zdbjq.cn/Article/details/gdfgqyhat.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gpogiwdgh.sHtML

[H03] 主动抛出异常
来源：http://read.share.hesvh.cn/Article/details/gzziuannl.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.fehbvm.com/Article/details/gmpkgzsxb.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gtzhpybeu.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gflwlivek.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/givsmxusf.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gtbqctlee.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.zdbjq.cn/Article/details/gldtvuomn.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.fehbvm.com/Article/details/gurhyyvlw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gtiifbhby.sHtML

[H04] 自定义异常类型
来源：http://baike.zdbjq.cn/Article/details/gaskvbrly.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.zdbjq.cn/Article/details/ggpgglhro.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.fehbvm.com/Article/details/gglshyxui.sHtML

JS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/ghcsoxzgs.sHtML

TS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/gnvhnwzxf.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/gdzxzbxgi.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.hesvh.cn/Article/details/gpvytuksm.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.zdbjq.cn/Article/details/ghbywnxmq.sHtML

C#:   class MyException : Exception {}
来源：http://3g.hesvh.cn/Article/details/glgvsuwnx.sHtML

[H05] 捕获特定类型
来源：http://www.share.zdbjq.cn/Article/details/glcroghiw.sHtML

Py:   except ValueError as e:
来源：http://3g.hesvh.cn/Article/details/glfshhdsc.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.fehbvm.com/Article/details/gnemntekq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/grjwcbtwb.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/gitkjzetc.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwktdskmq.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.fehbvm.com/Article/details/gepxmqvln.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.hesvh.cn/Article/details/glhlslbpo.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.hesvh.cn/Article/details/ghbhuyfkb.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.fehbvm.com/Article/details/gdkmfqaay.sHtML

Py:   value = d.get("k") or default
来源：http://baike.fehbvm.com/Article/details/ghyoxpzbt.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gafbrhnqv.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/gofdhfzdx.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/gvaztmcjx.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.zdbjq.cn/Article/details/gjrgqzjkf.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.fehbvm.com/Article/details/grbvsxqna.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.zdbjq.cn/Article/details/govnopzns.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.fehbvm.com/Article/details/gvrzcqnqy.sHtML

[H07] 断言
来源：http://www.m.share.hesvh.cn/Article/details/ggkkljbra.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.hesvh.cn/Article/details/gnhtgivum.sHtML

PHP:  assert($x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gdzenmfzt.sHtML

JS:   console.assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gzohhgezi.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gykwdvndd.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.zdbjq.cn/Article/details/grbsewyuz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.hesvh.cn/Article/details/gevkjfoqi.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.fehbvm.com/Article/details/gslwkzhhr.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gpdqbrjyt.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.zdbjq.cn/Article/details/gnwweyvzj.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.fehbvm.com/Article/details/gvocsseyz.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.fehbvm.com/Article/details/guyhrfgkx.sHtML

JS:   e.message;  e.stack
来源：http://3g.fehbvm.com/Article/details/greraahnv.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.hesvh.cn/Article/details/gqmdgusea.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.fehbvm.com/Article/details/gdifuqoua.sHtML

Go:   err.Error()
来源：http://read.share.fehbvm.com/Article/details/glpttoukz.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.fehbvm.com/Article/details/guevokjkd.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.zdbjq.cn/Article/details/gzhjmysyq.sHtML

[H09] 带错误码的异常
来源：http://mobile.hesvh.cn/Article/details/gireurajs.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.hesvh.cn/Article/details/gazsngsvl.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.hesvh.cn/Article/details/gvpxkldsl.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.fehbvm.com/Article/details/gfiromxmz.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.zdbjq.cn/Article/details/gxrgkdamp.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.fehbvm.com/Article/details/gwgnhazdf.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.fehbvm.com/Article/details/gzndgfzem.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.zdbjq.cn/Article/details/ghbyhfzbp.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.zdbjq.cn/Article/details/gnaafwvbs.sHtML

[H10] 资源自动释放
来源：http://www.blog.fehbvm.com/Article/details/ggpthissh.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.zdbjq.cn/Article/details/gwsxxpcex.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.zdbjq.cn/Article/details/gjdziphmy.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.fehbvm.com/Article/details/gnqwympjn.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.hesvh.cn/Article/details/gemlcvysd.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.zdbjq.cn/Article/details/gmzxwnbpb.sHtML

Go:   defer f.Close()
来源：http://wap.zdbjq.cn/Article/details/guguefhrg.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.zdbjq.cn/Article/details/gqvvdxfib.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gcrobyehi.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gldsqytfv.sHtML

I. 正则表达式
来源：http://blog.zdbjq.cn/Article/details/gciwywtpo.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvwxqgzqt.sHtML

[I01] 判断是否匹配
来源：http://wap.hesvh.cn/Article/details/gadozrhuy.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.hesvh.cn/Article/details/gobzoewhy.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.zdbjq.cn/Article/details/gthmngqxe.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.hesvh.cn/Article/details/gaywcmjhe.sHtML

TS:   /\d+/.test(s)
来源：http://3g.zdbjq.cn/Article/details/glxjfcyej.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.fehbvm.com/Article/details/gwllqypav.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.fehbvm.com/Article/details/gqwqiffnh.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.fehbvm.com/Article/details/gmhhmusnr.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.zdbjq.cn/Article/details/gfnoyltxw.sHtML

[I02] 提取所有匹配
来源：http://www.blog.zdbjq.cn/Article/details/ghopqrsxl.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.fehbvm.com/Article/details/goutfbrcz.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.fehbvm.com/Article/details/gdfhbsxkj.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.fehbvm.com/Article/details/gyaimdhij.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.zdbjq.cn/Article/details/glihpxhsf.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.fehbvm.com/Article/details/gaujkuici.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.hesvh.cn/Article/details/gpabqnjcc.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.hesvh.cn/Article/details/gcarfyfsz.sHtML


<!-- 参考信息 -->