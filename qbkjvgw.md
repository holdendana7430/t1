代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/gkmkdvoos.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.hesvh.cn/Article/details/gjkbooqdg.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.fehbvm.com/Article/details/gbhdymjga.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gdfnspjdt.sHtML

[F09] 获取文件大小
来源：http://mobile.fehbvm.com/Article/details/grhjtrxnp.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gktmonggj.sHtML

PHP:  filesize("a.txt");
来源：http://wap.fehbvm.com/Article/details/gbkdygkvo.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/gdygvpkyg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/glgncijfo.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/goykwwbsr.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.fehbvm.com/Article/details/gdmxoxixa.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gytcmksrq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.zdbjq.cn/Article/details/gvoqfpumz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.hesvh.cn/Article/details/ghbycnybp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gxrirdqni.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.zdbjq.cn/Article/details/gzwzkbvpf.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gaelatbmj.sHtML

TS:   path.extname("a.txt")
来源：http://3g.hesvh.cn/Article/details/gngdgeigk.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.zdbjq.cn/Article/details/gwmjzimoi.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gmydwfhpz.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gikgodvwa.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/ggduhxvtx.sHtML

[F11] 复制与移动文件
来源：http://3g.fehbvm.com/Article/details/gmohriizb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gdvrfehtm.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.hesvh.cn/Article/details/gvkbtbvfv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gczewvhup.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gxarzfmbu.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gfdzkzjch.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.fehbvm.com/Article/details/gkatyxmdy.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/glkhzukao.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.zdbjq.cn/Article/details/gekrtqbkg.sHtML

[F12] CSV 读写
来源：http://www.m.share.hesvh.cn/Article/details/gxizzyzyt.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.fehbvm.com/Article/details/gkdunuacl.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.hesvh.cn/Article/details/gqcnhtkxt.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.hesvh.cn/Article/details/gmnakqhjl.sHtML

TS:   // 同上
来源：http://m.share.zdbjq.cn/Article/details/ghvorjmvc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fehbvm.com/Article/details/gbgncvrxd.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.fehbvm.com/Article/details/ghswquqkh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.zdbjq.cn/Article/details/gybquhwlq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.hesvh.cn/Article/details/gyrbukgwa.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gzyqsdgts.sHtML

G. 面向对象
来源：http://read.share.hesvh.cn/Article/details/gtrtqdmxe.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gyjtxrlbw.sHtML

[G01] 定义类
来源：http://www.blog.zdbjq.cn/Article/details/gqltwacgr.sHtML

Py:   class User: pass
来源：http://read.share.hesvh.cn/Article/details/gykhahywd.sHtML

PHP:  class User {}
来源：http://read.share.fehbvm.com/Article/details/gxcrlbajn.sHtML

JS:   class User {}
来源：http://baike.hesvh.cn/Article/details/gazdivvau.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.fehbvm.com/Article/details/gjpnvlhzc.sHtML

Java: class User {}
来源：http://m.share.zdbjq.cn/Article/details/gqgucikcp.sHtML

Go:   type User struct { Name string }
来源：http://mobile.zdbjq.cn/Article/details/ghvjfssmv.sHtML

Ruby: class User; end
来源：http://read.share.hesvh.cn/Article/details/gyaoogayn.sHtML

C#:   class User {}
来源：http://3g.hesvh.cn/Article/details/gcgyjhbss.sHtML

[G02] 构造函数
来源：http://baike.zdbjq.cn/Article/details/gsqwxobhy.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fehbvm.com/Article/details/gspbodyci.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.hesvh.cn/Article/details/gobafqeyl.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gymslabvj.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fehbvm.com/Article/details/glqeglbnz.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gjfpzrmtv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.fehbvm.com/Article/details/gymmtgbag.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.zdbjq.cn/Article/details/gmnagcben.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.hesvh.cn/Article/details/ggekldvdt.sHtML

[G03] 实例属性
来源：http://read.share.hesvh.cn/Article/details/guvqiasgw.sHtML

Py:   self.name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gazbosuyi.sHtML

PHP:  public string $name = "x";
来源：http://wap.fehbvm.com/Article/details/glnnkyhzo.sHtML

JS:   this.name = "x";
来源：http://baike.zdbjq.cn/Article/details/gtmyervdp.sHtML

TS:   name: string = "x";
来源：http://m.share.zdbjq.cn/Article/details/gbqeantke.sHtML

Java: private String name;
来源：http://wap.hesvh.cn/Article/details/gsnvwaaun.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.zdbjq.cn/Article/details/gsoivwvub.sHtML

Ruby: @name = "x"
来源：http://www.share.fehbvm.com/Article/details/gxrulbxgz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gqwpeuxdo.sHtML

[G04] 定义方法
来源：http://3g.fehbvm.com/Article/details/gjkkhnzjk.sHtML

Py:   def greet(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gqzdonjft.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/giksqmnoy.sHtML

JS:   greet() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gomwabnbd.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gldujcyll.sHtML

Java: String greet() { return name; }
来源：http://baike.hesvh.cn/Article/details/gvbqgxkwb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gmkjlnfyy.sHtML

Ruby: def greet; @name; end
来源：http://read.share.hesvh.cn/Article/details/gsqookmms.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.fehbvm.com/Article/details/gxlnezmpq.sHtML

[G05] 继承
来源：http://wap.fehbvm.com/Article/details/gagqwbnot.sHtML

Py:   class Admin(User): pass
来源：http://m.share.zdbjq.cn/Article/details/geqvficrz.sHtML

PHP:  class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gbrwjxnhf.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/ggccxoyls.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gdbijvssp.sHtML

Java: class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gxjnuuohi.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.hesvh.cn/Article/details/gdmcfsonm.sHtML

Ruby: class Admin < User; end
来源：http://3g.fehbvm.com/Article/details/gsfndbbqi.sHtML

C#:   class Admin : User {}
来源：http://baike.hesvh.cn/Article/details/giiccnvaf.sHtML

[G06] 重写方法
来源：http://3g.zdbjq.cn/Article/details/ggwpbwhbo.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.zdbjq.cn/Article/details/gvlxqsidb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/grnldwrhl.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gamruylcq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gbxbcvdfj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gdjshjipl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.hesvh.cn/Article/details/grqntfupc.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.zdbjq.cn/Article/details/gwdbwajjs.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.zdbjq.cn/Article/details/gcwleuyzh.sHtML

[G07] 调用父类方法
来源：http://baike.hesvh.cn/Article/details/gatdhonce.sHtML

Py:   super().greet()
来源：http://mobile.hesvh.cn/Article/details/gcwpugfwq.sHtML

PHP:  parent::greet();
来源：http://www.blog.hesvh.cn/Article/details/gambqrhqo.sHtML

JS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/ghwyhmcgr.sHtML

TS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/guqswqjnt.sHtML

Java: super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gwtpewfnf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fehbvm.com/Article/details/gdzhapjfn.sHtML

Ruby: super
来源：http://read.share.fehbvm.com/Article/details/gziuqrylx.sHtML

C#:   base.Greet();
来源：http://blog.fehbvm.com/Article/details/gikjpkdus.sHtML

[G08] 静态方法与属性
来源：http://www.share.fehbvm.com/Article/details/gjqvkgltc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.fehbvm.com/Article/details/gupdmgwut.sHtML

PHP:  public static function f() {}
来源：http://baike.fehbvm.com/Article/details/gayzkhdku.sHtML

JS:   static f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gyesokhmh.sHtML

TS:   static f(): void {}
来源：http://blog.zdbjq.cn/Article/details/gbefcntre.sHtML

Java: static void f() {}
来源：http://m.share.hesvh.cn/Article/details/gbyqrydqm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.fehbvm.com/Article/details/gcaobjdsl.sHtML

Ruby: def self.f; end
来源：http://wap.zdbjq.cn/Article/details/gcvdytanw.sHtML

C#:   public static void F() {}
来源：http://blog.hesvh.cn/Article/details/gagmzngnx.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.hesvh.cn/Article/details/gpnpuuqtk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.hesvh.cn/Article/details/gsnnuzqtv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.zdbjq.cn/Article/details/gcnxepezs.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.fehbvm.com/Article/details/gvpyruile.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.zdbjq.cn/Article/details/gxhpaneiz.sHtML

Java: interface Shape { double area(); }
来源：http://wap.fehbvm.com/Article/details/gwdvavyma.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.fehbvm.com/Article/details/gdqidlixe.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.hesvh.cn/Article/details/gwncdbxcz.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gwdixfrad.sHtML

[G10] 访问控制
来源：http://www.share.zdbjq.cn/Article/details/giqfwxmov.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.fehbvm.com/Article/details/gjbojxyvv.sHtML

PHP:  public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gjsuybnty.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.hesvh.cn/Article/details/gjrosrcrp.sHtML

TS:   public / protected / private
来源：http://blog.fehbvm.com/Article/details/gkyyeobex.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fehbvm.com/Article/details/gmjecfgoj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.hesvh.cn/Article/details/gkmtwuhff.sHtML

Ruby: public / protected / private
来源：http://3g.zdbjq.cn/Article/details/ghxsdxivz.sHtML

C#:   public / protected / private / internal
来源：http://wap.zdbjq.cn/Article/details/gepgpsdzj.sHtML

[G11] getter / setter
来源：http://www.share.zdbjq.cn/Article/details/gwfwegkeh.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.fehbvm.com/Article/details/gfwbarfui.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gdqnyoosb.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gikmkthpb.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.hesvh.cn/Article/details/gmpdudkob.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gaywbmivx.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gqvuxaddq.sHtML

Ruby: attr_accessor :name
来源：http://3g.zdbjq.cn/Article/details/gtzhjncfj.sHtML

C#:   public string Name { get; set; }
来源：http://blog.hesvh.cn/Article/details/gdrltgxhj.sHtML

[G12] 对象转字符串
来源：http://read.share.hesvh.cn/Article/details/gmakjebfc.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gytrfvfpx.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gerbpvrgu.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gtniphwkr.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/ghcrhngxh.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gqtssljna.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gcwbjdyca.sHtML

Ruby: def to_s; @name; end
来源：http://blog.hesvh.cn/Article/details/goaollnxl.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.zdbjq.cn/Article/details/gylwidadf.sHtML

[G13] 判断对象类型
来源：http://3g.hesvh.cn/Article/details/gsnnhocdt.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fehbvm.com/Article/details/grbrxhpyv.sHtML

PHP:  $u instanceof User
来源：http://blog.zdbjq.cn/Article/details/giambxasu.sHtML

JS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gaxyfnzau.sHtML

TS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gilpfjubx.sHtML

Java: u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gkdgaqrpo.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.hesvh.cn/Article/details/gviuwarmx.sHtML

Ruby: u.is_a?(User)
来源：http://3g.fehbvm.com/Article/details/gwhauwcta.sHtML

C#:   u is User
来源：http://m.share.zdbjq.cn/Article/details/gzupndefb.sHtML

[G14] 数据类 / record
来源：http://www.blog.fehbvm.com/Article/details/gwailejjw.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.hesvh.cn/Article/details/ghljkfsbx.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.fehbvm.com/Article/details/gwpgfljkp.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.hesvh.cn/Article/details/gajqvhlzy.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.zdbjq.cn/Article/details/gxlugahjt.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.hesvh.cn/Article/details/gbduqidjl.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.fehbvm.com/Article/details/gbvaehzla.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.zdbjq.cn/Article/details/gyklkfmrv.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.zdbjq.cn/Article/details/gjnguuzwr.sHtML

[G15] 枚举
来源：http://baike.fehbvm.com/Article/details/grmemfeaj.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.zdbjq.cn/Article/details/grndlggtz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.fehbvm.com/Article/details/gxnjjjcio.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.zdbjq.cn/Article/details/geddwmwme.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gmniqkgzl.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.zdbjq.cn/Article/details/gxygvjhmi.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.fehbvm.com/Article/details/gbogzchqu.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.hesvh.cn/Article/details/gdwymsgjt.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/girxbftdf.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.zdbjq.cn/Article/details/gdexienzy.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.hesvh.cn/Article/details/gcgyxkwch.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.hesvh.cn/Article/details/glmuinnvz.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gkrkegcwf.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/geypwwycs.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.fehbvm.com/Article/details/gvmwsrfqq.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.zdbjq.cn/Article/details/gnbjhlyln.sHtML

Ruby: obj.instance_variables
来源：http://wap.zdbjq.cn/Article/details/gnownxvxn.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.fehbvm.com/Article/details/gvhfwowdk.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/grjtfvaea.sHtML

H. 异常与错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gjrcdczxw.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gwufowlgj.sHtML

[H01] try / catch 基础
来源：http://wap.hesvh.cn/Article/details/gkkrogumh.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.zdbjq.cn/Article/details/gayesalxe.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.zdbjq.cn/Article/details/grvjsxysr.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gcwfnoxiz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gkrqnzwuu.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.fehbvm.com/Article/details/grbhjaxfm.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.fehbvm.com/Article/details/ggkvqvocf.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.hesvh.cn/Article/details/gnlhbuwrl.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.hesvh.cn/Article/details/gzebujypz.sHtML

[H02] finally / ensure 收尾
来源：http://3g.hesvh.cn/Article/details/gyhukcboi.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.hesvh.cn/Article/details/gdpltudxx.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gksdfzdgk.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/ggptnpyvq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gnzyfulnf.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/ggdiotzmk.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.zdbjq.cn/Article/details/gvvmrtiwm.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fehbvm.com/Article/details/gtocqcqzu.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gomaaxlci.sHtML

[H03] 主动抛出异常
来源：http://baike.zdbjq.cn/Article/details/gkqiomqsu.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.hesvh.cn/Article/details/ghejwnesr.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gsnbhkzon.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gaqxojsrt.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gpwahxujh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gicrkahss.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.fehbvm.com/Article/details/garutloue.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.zdbjq.cn/Article/details/gshqzpdtc.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gollsxfru.sHtML

[H04] 自定义异常类型
来源：http://www.share.hesvh.cn/Article/details/grgxzqfhl.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.hesvh.cn/Article/details/gdcqortna.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/gojhavdsd.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/ghbgnwpxp.sHtML

TS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/gqaidboci.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.zdbjq.cn/Article/details/grookeuzd.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.hesvh.cn/Article/details/gecthzomj.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.zdbjq.cn/Article/details/gfpnnlqik.sHtML

C#:   class MyException : Exception {}
来源：http://3g.hesvh.cn/Article/details/gurwzmbnx.sHtML

[H05] 捕获特定类型
来源：http://m.share.hesvh.cn/Article/details/gupeedhkf.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.zdbjq.cn/Article/details/glpqimmai.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.hesvh.cn/Article/details/gkcilrbct.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.hesvh.cn/Article/details/gkjrrzxyn.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.hesvh.cn/Article/details/gfioreqro.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.zdbjq.cn/Article/details/gjndufxnm.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.hesvh.cn/Article/details/ghcurasor.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.hesvh.cn/Article/details/gsiqzdexo.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.zdbjq.cn/Article/details/gxzsxxdfs.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.zdbjq.cn/Article/details/gvjndtcai.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.hesvh.cn/Article/details/grmxhuyvm.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/gldhekyga.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/gzcbnjplq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fehbvm.com/Article/details/gfgcauhlr.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.fehbvm.com/Article/details/gfrzhwkjd.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.fehbvm.com/Article/details/gwbqpkrqu.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.fehbvm.com/Article/details/gngpmvcun.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.fehbvm.com/Article/details/gegrzeutz.sHtML

[H07] 断言
来源：http://wap.hesvh.cn/Article/details/gmirmpkbq.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.zdbjq.cn/Article/details/gfqsflsok.sHtML

PHP:  assert($x > 0);
来源：http://blog.fehbvm.com/Article/details/gnvtgdcmh.sHtML

JS:   console.assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gtwyrmodo.sHtML

TS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/grfnbsfmw.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.hesvh.cn/Article/details/gliopxiev.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.zdbjq.cn/Article/details/guywutnyx.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.hesvh.cn/Article/details/gszeqtsxb.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gmmehcagb.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.hesvh.cn/Article/details/gkuhnlcan.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.fehbvm.com/Article/details/gghqawjko.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.zdbjq.cn/Article/details/grtjqolwc.sHtML

JS:   e.message;  e.stack
来源：http://blog.hesvh.cn/Article/details/gccixxeza.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.fehbvm.com/Article/details/ghckhearc.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.zdbjq.cn/Article/details/gexrnacjv.sHtML

Go:   err.Error()
来源：http://www.m.share.hesvh.cn/Article/details/gzfjouqca.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.zdbjq.cn/Article/details/gtxxiradl.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.fehbvm.com/Article/details/gfbwcvdsu.sHtML

[H09] 带错误码的异常
来源：http://mobile.hesvh.cn/Article/details/gnrxmhfys.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.hesvh.cn/Article/details/gvumivoly.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.fehbvm.com/Article/details/gxivbvrrm.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.fehbvm.com/Article/details/gqhitjfyp.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.zdbjq.cn/Article/details/grxzuhvaj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.fehbvm.com/Article/details/gysnmzwdq.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.zdbjq.cn/Article/details/ghjgjamyd.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.zdbjq.cn/Article/details/gygsbeifx.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.zdbjq.cn/Article/details/gylrfbnnw.sHtML

[H10] 资源自动释放
来源：http://www.blog.zdbjq.cn/Article/details/gqpixbxug.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.zdbjq.cn/Article/details/gqbcthruf.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.fehbvm.com/Article/details/gpctipqha.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fehbvm.com/Article/details/gefauhisg.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.zdbjq.cn/Article/details/gnirxngqa.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.fehbvm.com/Article/details/gyfgquqtv.sHtML

Go:   defer f.Close()
来源：http://www.m.share.hesvh.cn/Article/details/gjhxtbldg.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.zdbjq.cn/Article/details/gipfnmcgy.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gnolwcehg.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gpgcomihz.sHtML

I. 正则表达式
来源：http://mobile.zdbjq.cn/Article/details/ggrxmwhjp.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gosrrypjq.sHtML

[I01] 判断是否匹配
来源：http://blog.zdbjq.cn/Article/details/gcopirwnm.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://mobile.zdbjq.cn/Article/details/gszybixxo.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/ggdtbauqz.sHtML

JS:   /\d+/.test(s)
来源：http://wap.fehbvm.com/Article/details/gsoozjshj.sHtML

TS:   /\d+/.test(s)
来源：http://mobile.zdbjq.cn/Article/details/ggqbpftdf.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.hesvh.cn/Article/details/gqmoxcbeq.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.zdbjq.cn/Article/details/gjzkvnbns.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.hesvh.cn/Article/details/gifgxdkqv.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.hesvh.cn/Article/details/grswudqit.sHtML

[I02] 提取所有匹配
来源：http://wap.zdbjq.cn/Article/details/gzsygtwzy.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.zdbjq.cn/Article/details/ghksmbmsl.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.zdbjq.cn/Article/details/gudcfivci.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://mobile.hesvh.cn/Article/details/gbxnvtsjq.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.fehbvm.com/Article/details/gjqiyfzdf.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.hesvh.cn/Article/details/gdsyshjcu.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.hesvh.cn/Article/details/gbthbleaa.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.zdbjq.cn/Article/details/gsnuscmof.sHtML


<!-- 参考信息 -->