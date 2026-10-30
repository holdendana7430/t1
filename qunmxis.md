代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gpxnidcwt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.hesvh.cn/Article/details/gffmdyomt.sHtML

Ruby: Dir.children("dir")
来源：http://blog.zdbjq.cn/Article/details/ghuiklqog.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.zdbjq.cn/Article/details/gjclbecgn.sHtML

[F09] 获取文件大小
来源：http://www.blog.zdbjq.cn/Article/details/gmiwndqlj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gwrlrrqqo.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gpwcqwgvg.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/guzhfgqma.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gkrngwdnn.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gtivxicwh.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.zdbjq.cn/Article/details/gqribmdtr.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gyxbkjcsa.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.fehbvm.com/Article/details/gvxzdvcot.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.hesvh.cn/Article/details/gepqglysr.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gviepgovc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.fehbvm.com/Article/details/glaguyymk.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gltabfkuu.sHtML

TS:   path.extname("a.txt")
来源：http://3g.fehbvm.com/Article/details/gmiygvqrv.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.hesvh.cn/Article/details/gojywkufe.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gchrgpjqj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gusagelhj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gdxuudmqs.sHtML

[F11] 复制与移动文件
来源：http://blog.hesvh.cn/Article/details/gjklsomuw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/goptsnldt.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.hesvh.cn/Article/details/gmizszlqg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gtgcneiow.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/glvjciavw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.zdbjq.cn/Article/details/gqzipyizv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.zdbjq.cn/Article/details/gjoooezmk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gqwbnmukw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.hesvh.cn/Article/details/gtesotfze.sHtML

[F12] CSV 读写
来源：http://www.blog.zdbjq.cn/Article/details/gemguwmfo.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.hesvh.cn/Article/details/ggfidtpqz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.fehbvm.com/Article/details/gkfropntl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.hesvh.cn/Article/details/gkzoeslqd.sHtML

TS:   // 同上
来源：http://www.blog.hesvh.cn/Article/details/glzwgdjbo.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.hesvh.cn/Article/details/glbzpyyjz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.hesvh.cn/Article/details/gaujotcag.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.hesvh.cn/Article/details/gjrdmvvqt.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.hesvh.cn/Article/details/gdihiyrho.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcheoafgf.sHtML

G. 面向对象
来源：http://www.blog.fehbvm.com/Article/details/ggeoncwpt.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/glxmiatme.sHtML

[G01] 定义类
来源：http://mobile.hesvh.cn/Article/details/gzggdrgqi.sHtML

Py:   class User: pass
来源：http://baike.fehbvm.com/Article/details/gzqmfdunl.sHtML

PHP:  class User {}
来源：http://wap.hesvh.cn/Article/details/ggbafwsxc.sHtML

JS:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gninpifob.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.hesvh.cn/Article/details/gzqzxjsne.sHtML

Java: class User {}
来源：http://www.share.fehbvm.com/Article/details/gklpmwlrw.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fehbvm.com/Article/details/gwbkoomdp.sHtML

Ruby: class User; end
来源：http://www.share.fehbvm.com/Article/details/ghcfqawdl.sHtML

C#:   class User {}
来源：http://3g.hesvh.cn/Article/details/gjereogve.sHtML

[G02] 构造函数
来源：http://read.share.zdbjq.cn/Article/details/gdojzyqcu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.zdbjq.cn/Article/details/gdyhzfkft.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.zdbjq.cn/Article/details/gxpwwhlcx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gtujdootm.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.hesvh.cn/Article/details/gjzlvxizd.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/geoauaxrv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.zdbjq.cn/Article/details/geunccaoo.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fehbvm.com/Article/details/gatefpzeo.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.fehbvm.com/Article/details/gkmsuthzk.sHtML

[G03] 实例属性
来源：http://m.share.fehbvm.com/Article/details/gqkxduegm.sHtML

Py:   self.name = "x"
来源：http://mobile.fehbvm.com/Article/details/gxcxligfl.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.hesvh.cn/Article/details/ggwjhqhho.sHtML

JS:   this.name = "x";
来源：http://wap.hesvh.cn/Article/details/ghmuqjtko.sHtML

TS:   name: string = "x";
来源：http://www.share.fehbvm.com/Article/details/gkbcrcttj.sHtML

Java: private String name;
来源：http://mobile.zdbjq.cn/Article/details/gvmpldhwr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fehbvm.com/Article/details/gbzdzebur.sHtML

Ruby: @name = "x"
来源：http://3g.hesvh.cn/Article/details/ghdbcwycq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.fehbvm.com/Article/details/gbaegpcyf.sHtML

[G04] 定义方法
来源：http://www.share.fehbvm.com/Article/details/gfbwssmpt.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gvplzeefb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/grmaikgvp.sHtML

JS:   greet() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gaozunhmr.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/ghzxntypy.sHtML

Java: String greet() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/glbykujcq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/ganavhbcs.sHtML

Ruby: def greet; @name; end
来源：http://www.share.hesvh.cn/Article/details/gbirlrvhe.sHtML

C#:   public string Greet() => Name;
来源：http://wap.zdbjq.cn/Article/details/gdzafwwjm.sHtML

[G05] 继承
来源：http://wap.zdbjq.cn/Article/details/gczsvghns.sHtML

Py:   class Admin(User): pass
来源：http://blog.hesvh.cn/Article/details/gcdncohkz.sHtML

PHP:  class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gqnswcftq.sHtML

JS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/glsujqfiy.sHtML

TS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gfvygrqci.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gffynemqt.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fehbvm.com/Article/details/gyygzpcub.sHtML

Ruby: class Admin < User; end
来源：http://blog.hesvh.cn/Article/details/gaykfckds.sHtML

C#:   class Admin : User {}
来源：http://m.share.zdbjq.cn/Article/details/gaddkskmg.sHtML

[G06] 重写方法
来源：http://www.blog.hesvh.cn/Article/details/gvxuvfqwo.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.zdbjq.cn/Article/details/gstzzkxyh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gyjsqjurd.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gtlilgftm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gxgcuxajf.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gwdnlfsed.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.hesvh.cn/Article/details/gewrodnbo.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.fehbvm.com/Article/details/gvstzfwcc.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.zdbjq.cn/Article/details/giywdxqxr.sHtML

[G07] 调用父类方法
来源：http://www.share.hesvh.cn/Article/details/gfjxdbnkp.sHtML

Py:   super().greet()
来源：http://www.blog.hesvh.cn/Article/details/gggykjcru.sHtML

PHP:  parent::greet();
来源：http://wap.zdbjq.cn/Article/details/gakeewbye.sHtML

JS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gwlxfguyz.sHtML

TS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gujihvwrp.sHtML

Java: super.greet();
来源：http://mobile.hesvh.cn/Article/details/ggnyexqhm.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.hesvh.cn/Article/details/grzjzayqa.sHtML

Ruby: super
来源：http://www.share.fehbvm.com/Article/details/gxpjjcoby.sHtML

C#:   base.Greet();
来源：http://mobile.hesvh.cn/Article/details/glazdxaip.sHtML

[G08] 静态方法与属性
来源：http://wap.hesvh.cn/Article/details/gndosyurh.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.zdbjq.cn/Article/details/ghfqhdcay.sHtML

PHP:  public static function f() {}
来源：http://read.share.hesvh.cn/Article/details/gtjglwwzl.sHtML

JS:   static f() {}
来源：http://baike.fehbvm.com/Article/details/gtylaemvl.sHtML

TS:   static f(): void {}
来源：http://www.share.fehbvm.com/Article/details/gigovmxmb.sHtML

Java: static void f() {}
来源：http://read.share.zdbjq.cn/Article/details/galvsegqd.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.zdbjq.cn/Article/details/guiwhqkqc.sHtML

Ruby: def self.f; end
来源：http://baike.zdbjq.cn/Article/details/gaiterily.sHtML

C#:   public static void F() {}
来源：http://www.share.zdbjq.cn/Article/details/gnrrcrsdf.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.zdbjq.cn/Article/details/gjcphxpij.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/gbcoyxmns.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdwlqbgmv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.hesvh.cn/Article/details/gediyjbvm.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.fehbvm.com/Article/details/gudcynejq.sHtML

Java: interface Shape { double area(); }
来源：http://3g.hesvh.cn/Article/details/gxwnmneih.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.hesvh.cn/Article/details/gcfcsvgou.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.zdbjq.cn/Article/details/gdyozjxyo.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gpodaubqj.sHtML

[G10] 访问控制
来源：http://baike.hesvh.cn/Article/details/gxnrizvzx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.hesvh.cn/Article/details/gdzqeigxu.sHtML

PHP:  public / protected / private
来源：http://blog.fehbvm.com/Article/details/gkxznjeif.sHtML

JS:   #private 字段；其余公开
来源：http://3g.hesvh.cn/Article/details/gsrpgjhdr.sHtML

TS:   public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gtldtuxay.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fehbvm.com/Article/details/gomejxbjg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.zdbjq.cn/Article/details/gkaghrhlg.sHtML

Ruby: public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gfdikjvfj.sHtML

C#:   public / protected / private / internal
来源：http://read.share.zdbjq.cn/Article/details/ghkcdufxh.sHtML

[G11] getter / setter
来源：http://www.blog.hesvh.cn/Article/details/ghwztexuo.sHtML

Py:   @property 与 @x.setter
来源：http://blog.hesvh.cn/Article/details/ggvbsvpfe.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gskqvueit.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/grwyevbyi.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.fehbvm.com/Article/details/gelkotxyt.sHtML

Java: public String getName() { return name; }
来源：http://3g.hesvh.cn/Article/details/grtkbnihr.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/goexoxtvz.sHtML

Ruby: attr_accessor :name
来源：http://m.share.zdbjq.cn/Article/details/gezndwjnc.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.hesvh.cn/Article/details/gvrueufxt.sHtML

[G12] 对象转字符串
来源：http://baike.zdbjq.cn/Article/details/gvpvorhmw.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.fehbvm.com/Article/details/gaktgrhja.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gytkjdofp.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gsdxobuib.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gxhcuvjrx.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/guruplsxu.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gyuqmduht.sHtML

Ruby: def to_s; @name; end
来源：http://3g.fehbvm.com/Article/details/giznvowfj.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/gestwyabc.sHtML

[G13] 判断对象类型
来源：http://read.share.zdbjq.cn/Article/details/gcmwpdcuo.sHtML

Py:   isinstance(u, User)
来源：http://3g.fehbvm.com/Article/details/gqfwqkzmo.sHtML

PHP:  $u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gowxphksl.sHtML

JS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gqwyhdmku.sHtML

TS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/ggrqbbtsf.sHtML

Java: u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gckfcvloe.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.fehbvm.com/Article/details/gpwgbmphn.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.hesvh.cn/Article/details/gcwuldqfn.sHtML

C#:   u is User
来源：http://baike.zdbjq.cn/Article/details/giyttkfgy.sHtML

[G14] 数据类 / record
来源：http://www.share.fehbvm.com/Article/details/gzfrjogbn.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.zdbjq.cn/Article/details/gdsccaxjb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.hesvh.cn/Article/details/gyfhatrfd.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.fehbvm.com/Article/details/gtoymzago.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.hesvh.cn/Article/details/gvyeyjiqr.sHtML

Java: record User(String name, int age) {}
来源：http://blog.zdbjq.cn/Article/details/gvqrnzxjr.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.hesvh.cn/Article/details/gefikbzic.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.zdbjq.cn/Article/details/gafbsuifv.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.fehbvm.com/Article/details/gihiqgzsy.sHtML

[G15] 枚举
来源：http://www.blog.zdbjq.cn/Article/details/gccqcfczl.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.zdbjq.cn/Article/details/gkoawzqxx.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.fehbvm.com/Article/details/gjkesmbwh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.zdbjq.cn/Article/details/gjzjxdvzw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/gnxmktwir.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.fehbvm.com/Article/details/gbpwozvlm.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.hesvh.cn/Article/details/gsbycicwk.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.fehbvm.com/Article/details/gwylnivfo.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gkamradas.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.zdbjq.cn/Article/details/gmcfkcybi.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.hesvh.cn/Article/details/gjtgixljq.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.zdbjq.cn/Article/details/gedfvxlsi.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gsnafgopd.sHtML

TS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/gvcsbhcvp.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.zdbjq.cn/Article/details/gcvjpgcrz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.zdbjq.cn/Article/details/gsdlmxdbq.sHtML

Ruby: obj.instance_variables
来源：http://blog.fehbvm.com/Article/details/gplbtyklq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.hesvh.cn/Article/details/gllwrkovu.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gmpvcdjzu.sHtML

H. 异常与错误处理
来源：http://3g.fehbvm.com/Article/details/gzeyyfrjm.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzqtqbdei.sHtML

[H01] try / catch 基础
来源：http://wap.zdbjq.cn/Article/details/gfsvxvhmp.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.zdbjq.cn/Article/details/gmpcikzon.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.fehbvm.com/Article/details/garfyttti.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gqzpafllo.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gcgegnhpd.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.hesvh.cn/Article/details/gpqagwbsi.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.hesvh.cn/Article/details/gnrjmbsel.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.hesvh.cn/Article/details/gkkwyljel.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.zdbjq.cn/Article/details/gqoxkgdod.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.hesvh.cn/Article/details/gvuhslges.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.fehbvm.com/Article/details/gjjelbzis.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gpddbvlfm.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gjfnfqgyz.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/ggrqhceoa.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gdnsmdsnx.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.zdbjq.cn/Article/details/gaekxnrja.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.fehbvm.com/Article/details/gyyollzvm.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/ghrsvrioo.sHtML

[H03] 主动抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/gzkwtjztx.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.hesvh.cn/Article/details/giwomdjbj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gakpcuaoo.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gmsruxfvf.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/gwrvxcqhm.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gnvjtiomd.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.fehbvm.com/Article/details/gplmwkvse.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.hesvh.cn/Article/details/gsreyarqr.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gkpqbbyhe.sHtML

[H04] 自定义异常类型
来源：http://3g.hesvh.cn/Article/details/gamygyckn.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.fehbvm.com/Article/details/gbspimioa.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/gurfycbfx.sHtML

JS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/gyncwqdwp.sHtML

TS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/gmhvnczzx.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/gyfwnedlr.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.fehbvm.com/Article/details/gimafzxsi.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.hesvh.cn/Article/details/gzhromvum.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.zdbjq.cn/Article/details/gtfoaideo.sHtML

[H05] 捕获特定类型
来源：http://mobile.zdbjq.cn/Article/details/gkwkvtzby.sHtML

Py:   except ValueError as e:
来源：http://www.blog.fehbvm.com/Article/details/gvtcnohqt.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.fehbvm.com/Article/details/gfdzskbnn.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.zdbjq.cn/Article/details/gjqojxkcd.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/gojjdiabi.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.zdbjq.cn/Article/details/gjlczyvhj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.zdbjq.cn/Article/details/grfarwjku.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.zdbjq.cn/Article/details/gyjklcjad.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.fehbvm.com/Article/details/gjvstveut.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.hesvh.cn/Article/details/gtxrlupzy.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.hesvh.cn/Article/details/gqykluqtn.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.fehbvm.com/Article/details/giipzsfbi.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fehbvm.com/Article/details/gypfbvcbd.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.hesvh.cn/Article/details/gjlvdvugv.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.hesvh.cn/Article/details/gqfgayuex.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.zdbjq.cn/Article/details/gzxysigcg.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.fehbvm.com/Article/details/gmupqdqgn.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.fehbvm.com/Article/details/geikwhczw.sHtML

[H07] 断言
来源：http://www.blog.hesvh.cn/Article/details/ggffjevkv.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.fehbvm.com/Article/details/gyiiyxclc.sHtML

PHP:  assert($x > 0);
来源：http://m.share.fehbvm.com/Article/details/gvbnxqhpz.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/glrvzhqkd.sHtML

TS:   console.assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gmmkdixau.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.zdbjq.cn/Article/details/gpxmkxzch.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.fehbvm.com/Article/details/gkgqwautt.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.zdbjq.cn/Article/details/gqaoltkek.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gqvbhudjs.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.fehbvm.com/Article/details/gxzbjwzit.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://wap.zdbjq.cn/Article/details/gegavdrkh.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.fehbvm.com/Article/details/gzhxbhjrf.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.zdbjq.cn/Article/details/gnksactfv.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.zdbjq.cn/Article/details/gqzbubkls.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.zdbjq.cn/Article/details/gaffduetw.sHtML

Go:   err.Error()
来源：http://read.share.hesvh.cn/Article/details/gfjkunynj.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.zdbjq.cn/Article/details/glkknmacr.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.zdbjq.cn/Article/details/gblpgwpvk.sHtML

[H09] 带错误码的异常
来源：http://www.m.share.hesvh.cn/Article/details/gtvracled.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.zdbjq.cn/Article/details/gxzemiejp.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.hesvh.cn/Article/details/gmvfzrwsl.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.fehbvm.com/Article/details/griawoapr.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.zdbjq.cn/Article/details/grywcwnfc.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.zdbjq.cn/Article/details/gotfcplcr.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.fehbvm.com/Article/details/gsaesxzxe.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.fehbvm.com/Article/details/ggvzjpahe.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.hesvh.cn/Article/details/gmxczosjc.sHtML

[H10] 资源自动释放
来源：http://www.m.share.fehbvm.com/Article/details/gmznmreha.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.zdbjq.cn/Article/details/gjhzomfxz.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.hesvh.cn/Article/details/gqeqjpqtb.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.zdbjq.cn/Article/details/gbndsafsb.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.hesvh.cn/Article/details/gygvrpmef.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.zdbjq.cn/Article/details/gsqxpougt.sHtML

Go:   defer f.Close()
来源：http://3g.fehbvm.com/Article/details/ggvrbixzi.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.fehbvm.com/Article/details/gmbwgepxs.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gpbpjmdxe.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/geczbzvly.sHtML

I. 正则表达式
来源：http://3g.fehbvm.com/Article/details/gpimfhupn.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gfysfrium.sHtML

[I01] 判断是否匹配
来源：http://3g.hesvh.cn/Article/details/gsrpgpmsh.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.hesvh.cn/Article/details/giumdeyil.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.fehbvm.com/Article/details/gzqvfpdwb.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.hesvh.cn/Article/details/gaykagsol.sHtML

TS:   /\d+/.test(s)
来源：http://baike.fehbvm.com/Article/details/gpnudjhdd.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.hesvh.cn/Article/details/gpgzgsznr.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.zdbjq.cn/Article/details/gsyvivptg.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.hesvh.cn/Article/details/gnundiovp.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.hesvh.cn/Article/details/gfnyonrtj.sHtML

[I02] 提取所有匹配
来源：http://blog.zdbjq.cn/Article/details/gjpnfaior.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.hesvh.cn/Article/details/gdlhzroid.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.hesvh.cn/Article/details/gypeifazo.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.zdbjq.cn/Article/details/gpwescuvs.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.fehbvm.com/Article/details/gfguqebtq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://blog.zdbjq.cn/Article/details/ghtofkjng.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.fehbvm.com/Article/details/gojqhuyqt.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.zdbjq.cn/Article/details/gaxguqtqz.sHtML


<!-- 参考信息 -->