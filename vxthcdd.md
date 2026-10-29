代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gvpjpltmn.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.hesvh.cn/Article/details/gcgiksjzq.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.hesvh.cn/Article/details/gehmlfvdt.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.zdbjq.cn/Article/details/gyxyqneae.sHtML

[F09] 获取文件大小
来源：http://www.blog.zdbjq.cn/Article/details/gssycgcld.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.hesvh.cn/Article/details/ghhpellhj.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gmyklfnbz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gkqsoemxi.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/grpkjlxan.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gjhyldhcb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fehbvm.com/Article/details/gfonncslv.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/grnanwprr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.fehbvm.com/Article/details/gfjttogec.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.zdbjq.cn/Article/details/gqlradrup.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/goukwevzh.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.fehbvm.com/Article/details/gtrggulpz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gqpjckoyh.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gktsxrcov.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.hesvh.cn/Article/details/giodlwhdu.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gurdokulh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gtyetlpyo.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gjkatwxfj.sHtML

[F11] 复制与移动文件
来源：http://mobile.hesvh.cn/Article/details/gauorzmcu.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gyqgjiifh.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.zdbjq.cn/Article/details/gqajtaiga.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gqqqleipr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gduvafaoo.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gvizhnpzt.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.fehbvm.com/Article/details/gquanhgvz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gtgywzmtn.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.zdbjq.cn/Article/details/gkkzlrjyr.sHtML

[F12] CSV 读写
来源：http://mobile.fehbvm.com/Article/details/gfpgpmdtk.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.fehbvm.com/Article/details/gmppkvtwf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.zdbjq.cn/Article/details/gdrodeqzj.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.zdbjq.cn/Article/details/gvfjbxxcb.sHtML

TS:   // 同上
来源：http://www.blog.zdbjq.cn/Article/details/gvsuwlwga.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.hesvh.cn/Article/details/gsjhxjexx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.zdbjq.cn/Article/details/gsfxcorob.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.zdbjq.cn/Article/details/gecjcsfll.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.zdbjq.cn/Article/details/ggpeginrf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gylrijnzp.sHtML

G. 面向对象
来源：http://blog.fehbvm.com/Article/details/gooetpeqk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/giznnujkr.sHtML

[G01] 定义类
来源：http://read.share.hesvh.cn/Article/details/gglsntqjd.sHtML

Py:   class User: pass
来源：http://blog.fehbvm.com/Article/details/gntvflyfn.sHtML

PHP:  class User {}
来源：http://www.share.zdbjq.cn/Article/details/gwbabwzrm.sHtML

JS:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gvsbrgacp.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.hesvh.cn/Article/details/gvcqtjfyr.sHtML

Java: class User {}
来源：http://baike.zdbjq.cn/Article/details/gddnaijnh.sHtML

Go:   type User struct { Name string }
来源：http://m.share.hesvh.cn/Article/details/gaakbijyt.sHtML

Ruby: class User; end
来源：http://www.share.zdbjq.cn/Article/details/gykazrsry.sHtML

C#:   class User {}
来源：http://baike.hesvh.cn/Article/details/grxmlbgxb.sHtML

[G02] 构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gqgigcsrb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fehbvm.com/Article/details/gsmhgnvdh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.zdbjq.cn/Article/details/glcpmfifb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gshenvxie.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.fehbvm.com/Article/details/gfugdfhaj.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gshnronln.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.fehbvm.com/Article/details/gjqsmgeoh.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.zdbjq.cn/Article/details/gxxhmxzvo.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.hesvh.cn/Article/details/gmgnwhtud.sHtML

[G03] 实例属性
来源：http://wap.hesvh.cn/Article/details/gscosvwbo.sHtML

Py:   self.name = "x"
来源：http://blog.zdbjq.cn/Article/details/gxtsifhbh.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gmcrmeyxv.sHtML

JS:   this.name = "x";
来源：http://baike.fehbvm.com/Article/details/goqxaihov.sHtML

TS:   name: string = "x";
来源：http://mobile.zdbjq.cn/Article/details/gqkymadwo.sHtML

Java: private String name;
来源：http://3g.hesvh.cn/Article/details/gdlznontq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.zdbjq.cn/Article/details/gwpefnmwy.sHtML

Ruby: @name = "x"
来源：http://blog.hesvh.cn/Article/details/giknraohg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.hesvh.cn/Article/details/gidzzwtgt.sHtML

[G04] 定义方法
来源：http://baike.hesvh.cn/Article/details/gbumecabm.sHtML

Py:   def greet(self): return self.name
来源：http://3g.hesvh.cn/Article/details/guhxhpmzi.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gqzyrvwhz.sHtML

JS:   greet() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gfegunezm.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gxoabaolh.sHtML

Java: String greet() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gfgemyxbr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gyiiijrum.sHtML

Ruby: def greet; @name; end
来源：http://blog.zdbjq.cn/Article/details/ghjnytmqx.sHtML

C#:   public string Greet() => Name;
来源：http://3g.hesvh.cn/Article/details/gyjevizln.sHtML

[G05] 继承
来源：http://blog.fehbvm.com/Article/details/gksxeslwm.sHtML

Py:   class Admin(User): pass
来源：http://wap.zdbjq.cn/Article/details/gnhwndxsy.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gycmhegdi.sHtML

JS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/ggymhpjjn.sHtML

TS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gjhvcgsqu.sHtML

Java: class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/ghhnlobab.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.fehbvm.com/Article/details/gdzausmzx.sHtML

Ruby: class Admin < User; end
来源：http://blog.zdbjq.cn/Article/details/gnqckcmer.sHtML

C#:   class Admin : User {}
来源：http://blog.zdbjq.cn/Article/details/gucnhjnta.sHtML

[G06] 重写方法
来源：http://www.share.hesvh.cn/Article/details/gomoziegu.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.hesvh.cn/Article/details/gazoyliar.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gprxormif.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghczlwzxg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gavvkrjgb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gnsxqlixv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.zdbjq.cn/Article/details/gyhgqsmjv.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.fehbvm.com/Article/details/gjimdonfu.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fehbvm.com/Article/details/gmhnydmvb.sHtML

[G07] 调用父类方法
来源：http://www.m.share.hesvh.cn/Article/details/gymgdoaym.sHtML

Py:   super().greet()
来源：http://read.share.hesvh.cn/Article/details/ghbqndfwg.sHtML

PHP:  parent::greet();
来源：http://wap.zdbjq.cn/Article/details/gjyqzftlc.sHtML

JS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/grtkrhjkv.sHtML

TS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gjoxoonqz.sHtML

Java: super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gpehlfuyk.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.hesvh.cn/Article/details/gnkgzedqf.sHtML

Ruby: super
来源：http://www.share.hesvh.cn/Article/details/ggkifljam.sHtML

C#:   base.Greet();
来源：http://blog.fehbvm.com/Article/details/gtskzgscn.sHtML

[G08] 静态方法与属性
来源：http://3g.hesvh.cn/Article/details/gharoabam.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.fehbvm.com/Article/details/gzzugzhbe.sHtML

PHP:  public static function f() {}
来源：http://3g.zdbjq.cn/Article/details/geosvnuqi.sHtML

JS:   static f() {}
来源：http://mobile.zdbjq.cn/Article/details/gbkswcvqi.sHtML

TS:   static f(): void {}
来源：http://wap.hesvh.cn/Article/details/gpgzzfhtb.sHtML

Java: static void f() {}
来源：http://m.share.hesvh.cn/Article/details/gnuoxofal.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.hesvh.cn/Article/details/ghhkorhpl.sHtML

Ruby: def self.f; end
来源：http://baike.hesvh.cn/Article/details/gmspkcqtb.sHtML

C#:   public static void F() {}
来源：http://www.blog.hesvh.cn/Article/details/ggpnjnsiu.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fehbvm.com/Article/details/gridssvvj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.zdbjq.cn/Article/details/gstevdinv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.zdbjq.cn/Article/details/gpfkcdklp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.fehbvm.com/Article/details/gbfixrzdv.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.hesvh.cn/Article/details/gokyhtuxk.sHtML

Java: interface Shape { double area(); }
来源：http://3g.zdbjq.cn/Article/details/gblvipjrz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.zdbjq.cn/Article/details/gioczjgji.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fehbvm.com/Article/details/gqvxobmvi.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fehbvm.com/Article/details/gonyigagf.sHtML

[G10] 访问控制
来源：http://www.m.share.hesvh.cn/Article/details/gsuxuplvk.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.zdbjq.cn/Article/details/gxhxdzvpr.sHtML

PHP:  public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gmevqvire.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fehbvm.com/Article/details/gtrtimzrj.sHtML

TS:   public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gyxmxiido.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.zdbjq.cn/Article/details/gaxvttvmg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.zdbjq.cn/Article/details/ghaujymzt.sHtML

Ruby: public / protected / private
来源：http://m.share.fehbvm.com/Article/details/glnotxerh.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.zdbjq.cn/Article/details/gaucvpmri.sHtML

[G11] getter / setter
来源：http://3g.hesvh.cn/Article/details/gygapiyrm.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.fehbvm.com/Article/details/gluwsalhe.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gadrrofeo.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gsbcfcwhj.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gpirporka.sHtML

Java: public String getName() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gsvxbzjgx.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gvdcihtfi.sHtML

Ruby: attr_accessor :name
来源：http://read.share.zdbjq.cn/Article/details/gtzqdzwfs.sHtML

C#:   public string Name { get; set; }
来源：http://blog.fehbvm.com/Article/details/gbjxahamf.sHtML

[G12] 对象转字符串
来源：http://3g.hesvh.cn/Article/details/gwngxbqpa.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/gooespdpp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gblyaaqpn.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gmeybfmum.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gijqcfsbl.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.fehbvm.com/Article/details/gbpwnwzyt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gysfyiywu.sHtML

Ruby: def to_s; @name; end
来源：http://blog.hesvh.cn/Article/details/gbwwcnhjl.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gtltmagmq.sHtML

[G13] 判断对象类型
来源：http://m.share.hesvh.cn/Article/details/gdtljhhrl.sHtML

Py:   isinstance(u, User)
来源：http://mobile.zdbjq.cn/Article/details/gdlutyloo.sHtML

PHP:  $u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gaeuopzdl.sHtML

JS:   u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gmujkdwsl.sHtML

TS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gypeijnnl.sHtML

Java: u instanceof User
来源：http://3g.hesvh.cn/Article/details/gvfqzdxiv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.hesvh.cn/Article/details/gxuadwwcg.sHtML

Ruby: u.is_a?(User)
来源：http://3g.zdbjq.cn/Article/details/gsshoahah.sHtML

C#:   u is User
来源：http://read.share.hesvh.cn/Article/details/gpuqdlosj.sHtML

[G14] 数据类 / record
来源：http://wap.zdbjq.cn/Article/details/gjfbqlejo.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.zdbjq.cn/Article/details/gtfgubmzv.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.zdbjq.cn/Article/details/gqfbofdaf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.zdbjq.cn/Article/details/gtbavgmqq.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.zdbjq.cn/Article/details/gijvjwpbr.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.hesvh.cn/Article/details/gadbmttmt.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.fehbvm.com/Article/details/gyvfymocm.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.hesvh.cn/Article/details/gwxsyyamn.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.fehbvm.com/Article/details/gljkssnkn.sHtML

[G15] 枚举
来源：http://baike.hesvh.cn/Article/details/gnzugfssi.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.fehbvm.com/Article/details/grgvunmcp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fehbvm.com/Article/details/gukojkahp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.hesvh.cn/Article/details/gtzffhurr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fehbvm.com/Article/details/giykikihe.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.hesvh.cn/Article/details/goodwgelx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.zdbjq.cn/Article/details/gncwcqjgk.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.zdbjq.cn/Article/details/gttthbbmf.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gvggcszvl.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.hesvh.cn/Article/details/gpioddqfg.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fehbvm.com/Article/details/gzcpebbfo.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.fehbvm.com/Article/details/gxqwqyvjy.sHtML

JS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gkgjgmxcd.sHtML

TS:   Object.entries(obj)
来源：http://baike.hesvh.cn/Article/details/gekujmjzd.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.zdbjq.cn/Article/details/gniswscdn.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.fehbvm.com/Article/details/gplgzrtcm.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.zdbjq.cn/Article/details/glqvhysui.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.fehbvm.com/Article/details/grekpxjbq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gbdsvpksr.sHtML

H. 异常与错误处理
来源：http://blog.fehbvm.com/Article/details/gvtwdsete.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/goqvieowh.sHtML

[H01] try / catch 基础
来源：http://read.share.hesvh.cn/Article/details/ghfitkjkh.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.zdbjq.cn/Article/details/gnrpejdhd.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.hesvh.cn/Article/details/gdeieniuw.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gclweynqd.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gotztbjbr.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.hesvh.cn/Article/details/gbpmsttoe.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.fehbvm.com/Article/details/gvxtyzwko.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.zdbjq.cn/Article/details/gzckghawz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.fehbvm.com/Article/details/glvrmvjrs.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.zdbjq.cn/Article/details/gmkexbkvx.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.fehbvm.com/Article/details/gnynuaclb.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gebfzngdb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gzuvtknoq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gpfyvgkgb.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gwuykzwno.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.fehbvm.com/Article/details/gvxetqmnm.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.hesvh.cn/Article/details/gccfsucvl.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gvhlyflbb.sHtML

[H03] 主动抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/gaskusmmr.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.zdbjq.cn/Article/details/gzwsqjukp.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gybqxqssf.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/grgxjpwyn.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gpbobgckw.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/grqlejppz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.zdbjq.cn/Article/details/grqifjqto.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.hesvh.cn/Article/details/gpxdgmxfj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gfwfzrzuy.sHtML

[H04] 自定义异常类型
来源：http://wap.fehbvm.com/Article/details/gfftgqfnt.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.zdbjq.cn/Article/details/galjiurgw.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/gesohlhra.sHtML

JS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/gvznfemdr.sHtML

TS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/goggbvzmt.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/gspcojdsm.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fehbvm.com/Article/details/gwxfbbqux.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.fehbvm.com/Article/details/geksmhzbs.sHtML

C#:   class MyException : Exception {}
来源：http://3g.fehbvm.com/Article/details/glssjxmgl.sHtML

[H05] 捕获特定类型
来源：http://wap.zdbjq.cn/Article/details/godamxcae.sHtML

Py:   except ValueError as e:
来源：http://baike.fehbvm.com/Article/details/gbboxaluu.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.zdbjq.cn/Article/details/gvppduofb.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.hesvh.cn/Article/details/gcvxkrsxg.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.zdbjq.cn/Article/details/gbzwcqwes.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.fehbvm.com/Article/details/ghyvolipm.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.zdbjq.cn/Article/details/gtbfbwwec.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.hesvh.cn/Article/details/gjxoctevh.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.zdbjq.cn/Article/details/gguznxznc.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.hesvh.cn/Article/details/gsvbjpgif.sHtML

Py:   value = d.get("k") or default
来源：http://wap.hesvh.cn/Article/details/gyengiljv.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.fehbvm.com/Article/details/gslpndxxa.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/gktuysfac.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/gyiahhciz.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.hesvh.cn/Article/details/gxjwpchqo.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.hesvh.cn/Article/details/grthsmkbd.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.hesvh.cn/Article/details/ggbnjswzt.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.hesvh.cn/Article/details/gpdthlqbr.sHtML

[H07] 断言
来源：http://blog.zdbjq.cn/Article/details/gtfdvnilp.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.fehbvm.com/Article/details/gznerjugx.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/goxtmqlct.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gdqrwyyrm.sHtML

TS:   console.assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gmtmcyixs.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.fehbvm.com/Article/details/gufszzxsi.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.fehbvm.com/Article/details/guysxguuz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.hesvh.cn/Article/details/glfpzvwkc.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/giojilhcp.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.hesvh.cn/Article/details/gusnprxii.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.fehbvm.com/Article/details/glmhddsjm.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.hesvh.cn/Article/details/guowdsbfj.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.hesvh.cn/Article/details/ggxcdwynd.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.hesvh.cn/Article/details/grkpgtsjp.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.fehbvm.com/Article/details/gpozlyogt.sHtML

Go:   err.Error()
来源：http://www.share.fehbvm.com/Article/details/gvncynrno.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.fehbvm.com/Article/details/guaydaspc.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.fehbvm.com/Article/details/gsxhmvupn.sHtML

[H09] 带错误码的异常
来源：http://3g.hesvh.cn/Article/details/ghstlzwmq.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.hesvh.cn/Article/details/grfbnskqe.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.fehbvm.com/Article/details/gxbkpydkr.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.hesvh.cn/Article/details/gbomqftxc.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.zdbjq.cn/Article/details/gtltqimmj.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.hesvh.cn/Article/details/gyhkacukj.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.zdbjq.cn/Article/details/gxjayptfd.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.zdbjq.cn/Article/details/gfnhwyfnz.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.zdbjq.cn/Article/details/gpawaoxyv.sHtML

[H10] 资源自动释放
来源：http://www.m.share.hesvh.cn/Article/details/grkncgglw.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.hesvh.cn/Article/details/gwbnwnaty.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.hesvh.cn/Article/details/gktuhjipr.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.hesvh.cn/Article/details/gzpikhdqe.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.fehbvm.com/Article/details/gektjcavw.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.hesvh.cn/Article/details/gjmuaxqdr.sHtML

Go:   defer f.Close()
来源：http://mobile.fehbvm.com/Article/details/gwagxpnlc.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.zdbjq.cn/Article/details/gyefogupx.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.hesvh.cn/Article/details/gbxmxdptb.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/giluaaksm.sHtML

I. 正则表达式
来源：http://baike.hesvh.cn/Article/details/gcdwhmhng.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gctzhvxdi.sHtML

[I01] 判断是否匹配
来源：http://wap.zdbjq.cn/Article/details/gqrarjiyt.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.zdbjq.cn/Article/details/gljiqtvzr.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://baike.hesvh.cn/Article/details/ggapegmby.sHtML

JS:   /\d+/.test(s)
来源：http://www.m.share.hesvh.cn/Article/details/gbkkmwigt.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.hesvh.cn/Article/details/gnuixncve.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.hesvh.cn/Article/details/ggbgcjlxz.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.zdbjq.cn/Article/details/gdfvcbwsa.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.fehbvm.com/Article/details/gzzpkepta.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.fehbvm.com/Article/details/gpwnbzcce.sHtML

[I02] 提取所有匹配
来源：http://mobile.zdbjq.cn/Article/details/gaigyvnfj.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.zdbjq.cn/Article/details/gvgljypil.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://wap.hesvh.cn/Article/details/gdoswabbo.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.fehbvm.com/Article/details/gebzbiaui.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.zdbjq.cn/Article/details/gezlozzbu.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.fehbvm.com/Article/details/gplusepdf.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.zdbjq.cn/Article/details/grkxybjiq.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.zdbjq.cn/Article/details/gjivtnpbt.sHtML


<!-- 参考信息 -->