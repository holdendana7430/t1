代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobnawrvu.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fanxiaobao.xyz/Article/details/ghnwprwwz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gdcdoxwbi.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.fanxiaobao.xyz/Article/details/gujpoahmo.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gjutdhcsm.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwdlkxte.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.fanxiaobao.xyz/Article/details/gjvsgrxxu.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gjypnadck.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxzmwuem.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gnykiiqep.sHtML

[F11] 复制与移动文件
来源：http://3g.fanxiaobao.xyz/Article/details/gqjeiyhjk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcoiqdpb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkcmhsazj.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gfttcgyhy.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gqdzdsegl.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fanxiaobao.xyz/Article/details/gtqhagzbl.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.fanxiaobao.xyz/Article/details/gloogpvfx.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/ggxrihtfe.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fanxiaobao.xyz/Article/details/gtlygsosp.sHtML

[F12] CSV 读写
来源：http://3g.fanxiaobao.xyz/Article/details/guqbnwiyp.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbcaxsdau.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.fanxiaobao.xyz/Article/details/gswnllnvb.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpblussy.sHtML

TS:   // 同上
来源：http://wap.fanxiaobao.xyz/Article/details/gigxhvvlu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fanxiaobao.xyz/Article/details/gicwwzohb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fanxiaobao.xyz/Article/details/gsqsajvbg.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.fanxiaobao.xyz/Article/details/gabjifanl.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fanxiaobao.xyz/Article/details/glrakhfyq.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gsdvgejmd.sHtML

G. 面向对象
来源：http://wap.fanxiaobao.xyz/Article/details/gnhgitrfq.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gwchpwojp.sHtML

[G01] 定义类
来源：http://blog.fanxiaobao.xyz/Article/details/giqiuphez.sHtML

Py:   class User: pass
来源：http://mobile.fanxiaobao.xyz/Article/details/gfcszzmcr.sHtML

PHP:  class User {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknuworyi.sHtML

JS:   class User {}
来源：http://wap.fanxiaobao.xyz/Article/details/gzxsrgvks.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfrouryd.sHtML

Java: class User {}
来源：http://3g.fanxiaobao.xyz/Article/details/gstaphvts.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugguvkph.sHtML

Ruby: class User; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqgcayig.sHtML

C#:   class User {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtosyhie.sHtML

[G02] 构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gduxrqmtk.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfewmfit.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggptahjgv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzswcuntv.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvjkidxc.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gozbmwudv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxvlrmgu.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyygqbfyt.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsguubamj.sHtML

[G03] 实例属性
来源：http://3g.fanxiaobao.xyz/Article/details/geratjhbu.sHtML

Py:   self.name = "x"
来源：http://baike.fanxiaobao.xyz/Article/details/gkdqybqzm.sHtML

PHP:  public string $name = "x";
来源：http://wap.fanxiaobao.xyz/Article/details/gtmfgcsob.sHtML

JS:   this.name = "x";
来源：http://mobile.fanxiaobao.xyz/Article/details/glszbqqfk.sHtML

TS:   name: string = "x";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpecxnbnn.sHtML

Java: private String name;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmpupilo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.fanxiaobao.xyz/Article/details/ghysfnevc.sHtML

Ruby: @name = "x"
来源：http://wap.fanxiaobao.xyz/Article/details/gfjoiwymg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fanxiaobao.xyz/Article/details/gdrjuuxgy.sHtML

[G04] 定义方法
来源：http://wap.fanxiaobao.xyz/Article/details/gongrlfkb.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fanxiaobao.xyz/Article/details/gfseiuhuy.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gomqzfqtv.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fanxiaobao.xyz/Article/details/grmdztwra.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gfhptypwa.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdzvkmml.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fanxiaobao.xyz/Article/details/ghifcqvit.sHtML

Ruby: def greet; @name; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmxmtviu.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fanxiaobao.xyz/Article/details/ghbqiqhfn.sHtML

[G05] 继承
来源：http://baike.fanxiaobao.xyz/Article/details/gtdxmmxgh.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fanxiaobao.xyz/Article/details/gdoaduqak.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gllrmsaqh.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxiewdgn.sHtML

TS:   class Admin extends User {}
来源：http://3g.fanxiaobao.xyz/Article/details/gqmfyauwa.sHtML

Java: class Admin extends User {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gvekgdgcl.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghngqedua.sHtML

Ruby: class Admin < User; end
来源：http://baike.fanxiaobao.xyz/Article/details/gcxusrmky.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gilimmpwj.sHtML

[G06] 重写方法
来源：http://m.share.fanxiaobao.xyz/Article/details/gghstdfzc.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.fanxiaobao.xyz/Article/details/gotnowzgt.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzldrihb.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwulexexl.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgieszuk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gpuarotye.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fanxiaobao.xyz/Article/details/gymphawvm.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gxjdsltnk.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fanxiaobao.xyz/Article/details/gcwcjsfwc.sHtML

[G07] 调用父类方法
来源：http://wap.fanxiaobao.xyz/Article/details/gfceysaaw.sHtML

Py:   super().greet()
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgcfvbgx.sHtML

PHP:  parent::greet();
来源：http://3g.fanxiaobao.xyz/Article/details/gogyrqddu.sHtML

JS:   super.greet();
来源：http://wap.fanxiaobao.xyz/Article/details/ghlnlstca.sHtML

TS:   super.greet();
来源：http://mobile.fanxiaobao.xyz/Article/details/gylpbonai.sHtML

Java: super.greet();
来源：http://wap.fanxiaobao.xyz/Article/details/gxyqntoej.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.fanxiaobao.xyz/Article/details/guetwqgrt.sHtML

Ruby: super
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gafwruckn.sHtML

C#:   base.Greet();
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnbadkpy.sHtML

[G08] 静态方法与属性
来源：http://read.share.fanxiaobao.xyz/Article/details/gimbwkbsq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.fanxiaobao.xyz/Article/details/gyshkpuwr.sHtML

PHP:  public static function f() {}
来源：http://m.share.fanxiaobao.xyz/Article/details/goiryjjrw.sHtML

JS:   static f() {}
来源：http://mobile.fanxiaobao.xyz/Article/details/glfjmbjtt.sHtML

TS:   static f(): void {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwrxgxeh.sHtML

Java: static void f() {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gbgpbwuzi.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fanxiaobao.xyz/Article/details/grgqllnik.sHtML

Ruby: def self.f; end
来源：http://blog.fanxiaobao.xyz/Article/details/gngqrdond.sHtML

C#:   public static void F() {}
来源：http://3g.fanxiaobao.xyz/Article/details/gpygrmpaj.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fanxiaobao.xyz/Article/details/gyihtssqs.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fanxiaobao.xyz/Article/details/giaahgwnf.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gijyqiyxi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.fanxiaobao.xyz/Article/details/gthmbkakq.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtctnbmlh.sHtML

Java: interface Shape { double area(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gzluomsvj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbfhatib.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.fanxiaobao.xyz/Article/details/gjifudheo.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fanxiaobao.xyz/Article/details/ghaskeebp.sHtML

[G10] 访问控制
来源：http://3g.fanxiaobao.xyz/Article/details/gsqepcccn.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkbbqech.sHtML

PHP:  public / protected / private
来源：http://www.share.fanxiaobao.xyz/Article/details/gisrwwpsz.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fanxiaobao.xyz/Article/details/govhhyfgj.sHtML

TS:   public / protected / private
来源：http://3g.fanxiaobao.xyz/Article/details/gpcezoqrk.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fanxiaobao.xyz/Article/details/guglfgkbb.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fanxiaobao.xyz/Article/details/glylzpedj.sHtML

Ruby: public / protected / private
来源：http://3g.fanxiaobao.xyz/Article/details/gaaiytoav.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdfnqgof.sHtML

[G11] getter / setter
来源：http://www.share.fanxiaobao.xyz/Article/details/glowvuukt.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqnaxiaj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/goxwnzhsz.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdlfllte.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gxblvnamj.sHtML

Java: public String getName() { return name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/giggspxqz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.fanxiaobao.xyz/Article/details/geqxldyoj.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fanxiaobao.xyz/Article/details/gufmotuvx.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gceowuvpz.sHtML

[G12] 对象转字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gxtjaveuq.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.fanxiaobao.xyz/Article/details/gftgdavln.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvoslcax.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnrkinkdf.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdefrcvub.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.fanxiaobao.xyz/Article/details/geswgkdzy.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.fanxiaobao.xyz/Article/details/gkldhtyeq.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqeladna.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqzszypp.sHtML

[G13] 判断对象类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowpwnfuk.sHtML

Py:   isinstance(u, User)
来源：http://read.share.fanxiaobao.xyz/Article/details/gajckjxbz.sHtML

PHP:  $u instanceof User
来源：http://mobile.fanxiaobao.xyz/Article/details/gsnjyopab.sHtML

JS:   u instanceof User
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwrikhgr.sHtML

TS:   u instanceof User
来源：http://blog.fanxiaobao.xyz/Article/details/gcinbfxxr.sHtML

Java: u instanceof User
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbfxlpoct.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.fanxiaobao.xyz/Article/details/gznlddofw.sHtML

Ruby: u.is_a?(User)
来源：http://blog.fanxiaobao.xyz/Article/details/gqoqjrejd.sHtML

C#:   u is User
来源：http://m.share.fanxiaobao.xyz/Article/details/gcsfbsjcm.sHtML

[G14] 数据类 / record
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrwdiyal.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.fanxiaobao.xyz/Article/details/gspudceqc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfujomwqd.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.fanxiaobao.xyz/Article/details/ganrxoeps.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.fanxiaobao.xyz/Article/details/gudaxieyz.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzuwbhjm.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.fanxiaobao.xyz/Article/details/gbmrsgzwg.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.fanxiaobao.xyz/Article/details/gzpvikkvn.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.fanxiaobao.xyz/Article/details/gsngnfmpk.sHtML

[G15] 枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gnwnuxnrg.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.fanxiaobao.xyz/Article/details/guzuyeuiz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.fanxiaobao.xyz/Article/details/ghegdossc.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxmxokgl.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/grngqngvz.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgvqzbrb.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grcgrwpyh.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.fanxiaobao.xyz/Article/details/gncapmdca.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gfdxniucj.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gtsoaaggq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fanxiaobao.xyz/Article/details/gfvodgood.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqxeycoj.sHtML

JS:   Object.entries(obj)
来源：http://wap.fanxiaobao.xyz/Article/details/gkmbwyzkq.sHtML

TS:   Object.entries(obj)
来源：http://blog.fanxiaobao.xyz/Article/details/gpcojijwr.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fanxiaobao.xyz/Article/details/gesqhrjly.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.fanxiaobao.xyz/Article/details/gcbbgyhjq.sHtML

Ruby: obj.instance_variables
来源：http://baike.fanxiaobao.xyz/Article/details/gnzykcbmb.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.fanxiaobao.xyz/Article/details/gpwdembvg.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gqfgactye.sHtML

H. 异常与错误处理
来源：http://wap.fanxiaobao.xyz/Article/details/gzihebyop.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gjaoknfvv.sHtML

[H01] try / catch 基础
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcbzuxrw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.fanxiaobao.xyz/Article/details/grnkgctpv.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbotdqmjs.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzawsnknk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.fanxiaobao.xyz/Article/details/gbdmcmnoj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.fanxiaobao.xyz/Article/details/gqqhaotjb.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.fanxiaobao.xyz/Article/details/gkuqwqbtc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.fanxiaobao.xyz/Article/details/gdmyvmhxr.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrapudxn.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gvarhsvlw.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.fanxiaobao.xyz/Article/details/gubeanruj.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.fanxiaobao.xyz/Article/details/gqovwsjjk.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gtsdhmcpn.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.fanxiaobao.xyz/Article/details/ggixrwuql.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzqzkwutg.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.fanxiaobao.xyz/Article/details/gqheyozrl.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gsconttjy.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gavguyaxu.sHtML

[H03] 主动抛出异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhgjckpx.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.fanxiaobao.xyz/Article/details/golzuhuft.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdkknpbr.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.fanxiaobao.xyz/Article/details/glxwqchkz.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.fanxiaobao.xyz/Article/details/gkebyfeap.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.fanxiaobao.xyz/Article/details/gjbgnklnx.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.fanxiaobao.xyz/Article/details/gtcrgwgvd.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.fanxiaobao.xyz/Article/details/gycselddx.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwrhanam.sHtML

[H04] 自定义异常类型
来源：http://wap.fanxiaobao.xyz/Article/details/gxjisbloz.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkvvaajn.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrvsufqg.sHtML

JS:   class MyError extends Error {}
来源：http://3g.fanxiaobao.xyz/Article/details/glwjabnsj.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpduummv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwwqfmxk.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fanxiaobao.xyz/Article/details/gigxabcle.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gjykuxawa.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gynwidyvf.sHtML

[H05] 捕获特定类型
来源：http://baike.fanxiaobao.xyz/Article/details/gbbtscmge.sHtML

Py:   except ValueError as e:
来源：http://wap.fanxiaobao.xyz/Article/details/gaozywpbs.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gznowdzym.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gvfjwnyoj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzfxiicw.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gdpqzbgkl.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwnkgesom.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.fanxiaobao.xyz/Article/details/gaupuzrlq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqgwyyvj.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.fanxiaobao.xyz/Article/details/gytpfthjq.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdloslqd.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvovdiurl.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.fanxiaobao.xyz/Article/details/gaxicfrje.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulfrzslb.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.fanxiaobao.xyz/Article/details/glpicjijy.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gufjanajq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.fanxiaobao.xyz/Article/details/ggprodyjp.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.fanxiaobao.xyz/Article/details/gohrovbtl.sHtML

[H07] 断言
来源：http://read.share.fanxiaobao.xyz/Article/details/gzicsnvwz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.fanxiaobao.xyz/Article/details/greowvbft.sHtML

PHP:  assert($x > 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyuxmiasg.sHtML

JS:   console.assert(x > 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gfmjujlre.sHtML

TS:   console.assert(x > 0);
来源：http://3g.fanxiaobao.xyz/Article/details/gkjqvypxh.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giryrzsal.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbrxozms.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.fanxiaobao.xyz/Article/details/gcrfifwda.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.fanxiaobao.xyz/Article/details/goyzfztmu.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.fanxiaobao.xyz/Article/details/gypriuolp.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.fanxiaobao.xyz/Article/details/gkoahlfah.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqwwjkgo.sHtML

JS:   e.message;  e.stack
来源：http://m.share.fanxiaobao.xyz/Article/details/gftgplfih.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwchssjan.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwawuczzd.sHtML

Go:   err.Error()
来源：http://www.share.fanxiaobao.xyz/Article/details/gvmjrrzlz.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.fanxiaobao.xyz/Article/details/grcnpejhp.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.fanxiaobao.xyz/Article/details/gncksifuk.sHtML

[H09] 带错误码的异常
来源：http://www.share.fanxiaobao.xyz/Article/details/giuzxiufm.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwslmldy.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.fanxiaobao.xyz/Article/details/ghsumixju.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grtwmsbbs.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gymwzprnc.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.fanxiaobao.xyz/Article/details/gbkwouyac.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gygkdfktu.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.fanxiaobao.xyz/Article/details/gfoznszph.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmosnuwtz.sHtML

[H10] 资源自动释放
来源：http://baike.fanxiaobao.xyz/Article/details/gghgmksqu.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.fanxiaobao.xyz/Article/details/gozwdloox.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.fanxiaobao.xyz/Article/details/giryeukre.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fanxiaobao.xyz/Article/details/guajqgnpf.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.fanxiaobao.xyz/Article/details/gsifavnqn.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpypwkabu.sHtML

Go:   defer f.Close()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkenjghog.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghfxluvlf.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.fanxiaobao.xyz/Article/details/gmexzcvtr.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gijidoawj.sHtML

I. 正则表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/glwyyzrbd.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gqxddetiq.sHtML

[I01] 判断是否匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gmczebmxn.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.fanxiaobao.xyz/Article/details/gqukjfysu.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://3g.fanxiaobao.xyz/Article/details/gchjntlyp.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxawbrrbr.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmtijuyvc.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.fanxiaobao.xyz/Article/details/goypntjnn.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gpppjclfj.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gieiyzule.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.fanxiaobao.xyz/Article/details/gyjopislw.sHtML

[I02] 提取所有匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/ggilycklv.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gonhwuttb.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.fanxiaobao.xyz/Article/details/gfxnwkjme.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbcrasdv.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.fanxiaobao.xyz/Article/details/gfzovclgq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.fanxiaobao.xyz/Article/details/galbrfgsg.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqxepbqi.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbylfccmy.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.fanxiaobao.xyz/Article/details/glljldiig.sHtML

[I03] 提取捕获分组
来源：http://wap.fanxiaobao.xyz/Article/details/giaztbwdf.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.fanxiaobao.xyz/Article/details/guoxspedx.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvtmdnexx.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrudcfao.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.fanxiaobao.xyz/Article/details/gcckiddgs.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpfrrgpv.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.fanxiaobao.xyz/Article/details/guacibllm.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://mobile.fanxiaobao.xyz/Article/details/gstquggyc.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://3g.fanxiaobao.xyz/Article/details/gquaibhhc.sHtML

[I04] 正则替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyiatvukd.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://blog.fanxiaobao.xyz/Article/details/gyaoxzlbf.sHtML


<!-- 参考信息 -->