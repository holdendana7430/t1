代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gbomtynju.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fehbvm.com/Article/details/gvefduava.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.zdbjq.cn/Article/details/gmyxvxwrr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gqzlomilm.sHtML

[F09] 获取文件大小
来源：http://blog.fehbvm.com/Article/details/gpkrrwfwy.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gapekunyd.sHtML

PHP:  filesize("a.txt");
来源：http://wap.fehbvm.com/Article/details/gstlxtvqf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/giaxhrvlf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gqmucdqvx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gazipqshk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.zdbjq.cn/Article/details/glvylrmly.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gopojrmvk.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fehbvm.com/Article/details/gxlitzehp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.hesvh.cn/Article/details/gwttibmgc.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gncaettip.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fehbvm.com/Article/details/gqtnmpkxl.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gapakisum.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gzgessarc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.zdbjq.cn/Article/details/ggcpsehho.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gmfjeuvgt.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gbwdcvwvk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/glnjcpgyr.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.fehbvm.com/Article/details/glrcgyzxa.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gnrklsxhc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.zdbjq.cn/Article/details/gclvoihtc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/glujrnkbi.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gvbdjltza.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.zdbjq.cn/Article/details/gsfhsmdeh.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.hesvh.cn/Article/details/gjsbfdfnv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gbxvuegak.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.hesvh.cn/Article/details/gtnqzszgz.sHtML

[F12] CSV 读写
来源：http://www.blog.hesvh.cn/Article/details/gdivrrtmw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.zdbjq.cn/Article/details/gmqqkksui.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.fehbvm.com/Article/details/gfnkligqd.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.zdbjq.cn/Article/details/gmwmyfhtp.sHtML

TS:   // 同上
来源：http://mobile.zdbjq.cn/Article/details/gzsmijyzd.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fehbvm.com/Article/details/gcxktyusa.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.zdbjq.cn/Article/details/gajohyncy.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fehbvm.com/Article/details/gnwndhzxr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.fehbvm.com/Article/details/grfonvafd.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gcmfutlza.sHtML

G. 面向对象
来源：http://read.share.fehbvm.com/Article/details/gilmuguvx.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gjmxpupuu.sHtML

[G01] 定义类
来源：http://read.share.fehbvm.com/Article/details/gjbttkkks.sHtML

Py:   class User: pass
来源：http://3g.fehbvm.com/Article/details/gkrhwuimb.sHtML

PHP:  class User {}
来源：http://www.blog.fehbvm.com/Article/details/gpmoapzsp.sHtML

JS:   class User {}
来源：http://wap.hesvh.cn/Article/details/ghwbuvuil.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.hesvh.cn/Article/details/ggmvkszlv.sHtML

Java: class User {}
来源：http://read.share.fehbvm.com/Article/details/grhugpuap.sHtML

Go:   type User struct { Name string }
来源：http://m.share.hesvh.cn/Article/details/gedxkuszf.sHtML

Ruby: class User; end
来源：http://read.share.zdbjq.cn/Article/details/gqblbveit.sHtML

C#:   class User {}
来源：http://read.share.fehbvm.com/Article/details/glxeuumpc.sHtML

[G02] 构造函数
来源：http://read.share.zdbjq.cn/Article/details/gqrxqdyna.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.hesvh.cn/Article/details/guhilgtar.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.fehbvm.com/Article/details/gwwvmhwac.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gztiamwkr.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fehbvm.com/Article/details/gdpamcytc.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gkzgmxtow.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.fehbvm.com/Article/details/gcrvojddt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.zdbjq.cn/Article/details/ghhdscyvq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gqvbwdwia.sHtML

[G03] 实例属性
来源：http://www.blog.fehbvm.com/Article/details/googbsjwp.sHtML

Py:   self.name = "x"
来源：http://read.share.fehbvm.com/Article/details/gvhsgphwa.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.hesvh.cn/Article/details/gybeirldn.sHtML

JS:   this.name = "x";
来源：http://mobile.hesvh.cn/Article/details/ggwsimyjk.sHtML

TS:   name: string = "x";
来源：http://read.share.fehbvm.com/Article/details/gbsplzsjm.sHtML

Java: private String name;
来源：http://3g.hesvh.cn/Article/details/gndflbaun.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.hesvh.cn/Article/details/gqlcrmfjl.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gbstsfjmf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.hesvh.cn/Article/details/gplxxqoqx.sHtML

[G04] 定义方法
来源：http://baike.zdbjq.cn/Article/details/grmqqvdqx.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gkrgzrfwm.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/glbtelnqo.sHtML

JS:   greet() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/ggdnxfwwf.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gxfgernuu.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gsqireogf.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gautfeyed.sHtML

Ruby: def greet; @name; end
来源：http://www.share.hesvh.cn/Article/details/gcrksbunr.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gutfssznp.sHtML

[G05] 继承
来源：http://m.share.hesvh.cn/Article/details/gmjtrdvyj.sHtML

Py:   class Admin(User): pass
来源：http://3g.fehbvm.com/Article/details/gimrnjpmf.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gdygyglpd.sHtML

JS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gqdbvdwxg.sHtML

TS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gbzyuaglz.sHtML

Java: class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gxumhhbsg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.hesvh.cn/Article/details/gfaqkyvqz.sHtML

Ruby: class Admin < User; end
来源：http://3g.hesvh.cn/Article/details/gpyirhtjj.sHtML

C#:   class Admin : User {}
来源：http://m.share.zdbjq.cn/Article/details/gvrytkppr.sHtML

[G06] 重写方法
来源：http://www.m.share.hesvh.cn/Article/details/gmapgnxeh.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.zdbjq.cn/Article/details/gikzpynuj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gxkfiuoha.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/guxcmdsmv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/ggpyewgxo.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gcdjinnjb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fehbvm.com/Article/details/grheujzpf.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.fehbvm.com/Article/details/glbptjqqm.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fehbvm.com/Article/details/gdfgehjme.sHtML

[G07] 调用父类方法
来源：http://read.share.hesvh.cn/Article/details/ggzpsbbhr.sHtML

Py:   super().greet()
来源：http://3g.zdbjq.cn/Article/details/gcfoghncv.sHtML

PHP:  parent::greet();
来源：http://blog.hesvh.cn/Article/details/ggcwmlauc.sHtML

JS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gyaxnmpvz.sHtML

TS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/ghwkuxusp.sHtML

Java: super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gxytikhtl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fehbvm.com/Article/details/gsqwyqoyy.sHtML

Ruby: super
来源：http://read.share.fehbvm.com/Article/details/gkxjvsrmj.sHtML

C#:   base.Greet();
来源：http://blog.hesvh.cn/Article/details/gvbtscjdq.sHtML

[G08] 静态方法与属性
来源：http://www.blog.hesvh.cn/Article/details/gxresqgec.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.zdbjq.cn/Article/details/gdaxgflvy.sHtML

PHP:  public static function f() {}
来源：http://www.share.fehbvm.com/Article/details/gkwjcglyt.sHtML

JS:   static f() {}
来源：http://3g.hesvh.cn/Article/details/grbeoemvi.sHtML

TS:   static f(): void {}
来源：http://blog.hesvh.cn/Article/details/gcwkmufjp.sHtML

Java: static void f() {}
来源：http://www.blog.hesvh.cn/Article/details/gsgcuaeoo.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fehbvm.com/Article/details/gixmbvrxl.sHtML

Ruby: def self.f; end
来源：http://blog.fehbvm.com/Article/details/gxfhoxgsd.sHtML

C#:   public static void F() {}
来源：http://blog.fehbvm.com/Article/details/gculzxlse.sHtML

[G09] 接口 / 抽象类
来源：http://3g.fehbvm.com/Article/details/gecrlqlzd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.zdbjq.cn/Article/details/gdqtosdat.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.zdbjq.cn/Article/details/gumitrqla.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.hesvh.cn/Article/details/ghwzwkwyt.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.zdbjq.cn/Article/details/gusqykpuw.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fehbvm.com/Article/details/gqtbdysfi.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.zdbjq.cn/Article/details/gdctpsbih.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fehbvm.com/Article/details/goyaiielv.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.fehbvm.com/Article/details/ghceuwdlr.sHtML

[G10] 访问控制
来源：http://3g.zdbjq.cn/Article/details/ggzoymmjt.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.fehbvm.com/Article/details/gojzgxnco.sHtML

PHP:  public / protected / private
来源：http://3g.zdbjq.cn/Article/details/ggbcyuhls.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.fehbvm.com/Article/details/guxnyhrkt.sHtML

TS:   public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gksijiifx.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.hesvh.cn/Article/details/gxazislrk.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.zdbjq.cn/Article/details/gygfnzuwo.sHtML

Ruby: public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gwoigypxd.sHtML

C#:   public / protected / private / internal
来源：http://m.share.hesvh.cn/Article/details/gydrwosds.sHtML

[G11] getter / setter
来源：http://www.share.hesvh.cn/Article/details/giamjmqgd.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fehbvm.com/Article/details/gpmuxcvaw.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gvmfdrbxx.sHtML

JS:   get name() { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gmzfldkbu.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/greiwmild.sHtML

Java: public String getName() { return name; }
来源：http://blog.zdbjq.cn/Article/details/ghibhvpuf.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/goeypbigu.sHtML

Ruby: attr_accessor :name
来源：http://3g.fehbvm.com/Article/details/giwqswjcf.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.hesvh.cn/Article/details/gkasfdhre.sHtML

[G12] 对象转字符串
来源：http://mobile.zdbjq.cn/Article/details/gijwqdjjw.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gezdkqeok.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gxojlcdpd.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gvliprjyq.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gedmvxqow.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gmdhdzesh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/ghehwezdy.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.hesvh.cn/Article/details/gskezaave.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gvmmgtllr.sHtML

[G13] 判断对象类型
来源：http://baike.hesvh.cn/Article/details/gpcbssbuq.sHtML

Py:   isinstance(u, User)
来源：http://wap.fehbvm.com/Article/details/gqdvlindt.sHtML

PHP:  $u instanceof User
来源：http://baike.hesvh.cn/Article/details/guvyvxdxf.sHtML

JS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gtagonfvx.sHtML

TS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gzeroieey.sHtML

Java: u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gcnijzsbd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.fehbvm.com/Article/details/ggvjdhuwy.sHtML

Ruby: u.is_a?(User)
来源：http://wap.zdbjq.cn/Article/details/gmreeaiug.sHtML

C#:   u is User
来源：http://baike.zdbjq.cn/Article/details/gjfoiriaq.sHtML

[G14] 数据类 / record
来源：http://www.share.fehbvm.com/Article/details/gfhmpszni.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.zdbjq.cn/Article/details/gumwlimtj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.fehbvm.com/Article/details/ggfjnnxqb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.fehbvm.com/Article/details/gucauxctt.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.fehbvm.com/Article/details/gzxomyeba.sHtML

Java: record User(String name, int age) {}
来源：http://3g.fehbvm.com/Article/details/gaiueveja.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.hesvh.cn/Article/details/gsfarglhn.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.hesvh.cn/Article/details/gnnqqcjwv.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.hesvh.cn/Article/details/gueordjsh.sHtML

[G15] 枚举
来源：http://wap.zdbjq.cn/Article/details/gansuuavz.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.hesvh.cn/Article/details/gnqdtnnnp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.hesvh.cn/Article/details/gijiarpjh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.zdbjq.cn/Article/details/gutzvkogk.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fehbvm.com/Article/details/gmmbsklsv.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.hesvh.cn/Article/details/gnvaejnyk.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.hesvh.cn/Article/details/gstxsvgej.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.fehbvm.com/Article/details/gsxroclck.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gbbkkwwaz.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.fehbvm.com/Article/details/gyaijphke.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.fehbvm.com/Article/details/gqcfkqzld.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.hesvh.cn/Article/details/gwhqeowbt.sHtML

JS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/gzykzcayi.sHtML

TS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/gjbfanffj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.zdbjq.cn/Article/details/gytyaewmy.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.hesvh.cn/Article/details/gqibueeok.sHtML

Ruby: obj.instance_variables
来源：http://read.share.fehbvm.com/Article/details/grjifzbqm.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/gngkavovv.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gfmvrsxga.sHtML

H. 异常与错误处理
来源：http://baike.zdbjq.cn/Article/details/gbtfebsph.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gztzrahve.sHtML

[H01] try / catch 基础
来源：http://3g.fehbvm.com/Article/details/ginevadob.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.zdbjq.cn/Article/details/gnvirbqdw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.hesvh.cn/Article/details/gpwbdyaxa.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gmqdyqwhm.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/giotjtkuj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.hesvh.cn/Article/details/gwcqdjpjj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.zdbjq.cn/Article/details/giyarkkzo.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.hesvh.cn/Article/details/gsijvdzcz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.fehbvm.com/Article/details/gdlaabpfv.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.zdbjq.cn/Article/details/gliaqxhly.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.hesvh.cn/Article/details/grmfcuafp.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gcbpxtpdq.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gckbgwsip.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gybwqmfvz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gqgubowlu.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.zdbjq.cn/Article/details/gcczbsjzj.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.zdbjq.cn/Article/details/gqopumivz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gjygbgdeo.sHtML

[H03] 主动抛出异常
来源：http://m.share.fehbvm.com/Article/details/genibikwd.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.zdbjq.cn/Article/details/glbjoiiec.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gxqhoyape.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gltunpaxx.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/gazknhjlk.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/garhnpovo.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.zdbjq.cn/Article/details/ggrgrbhxm.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.fehbvm.com/Article/details/gbfuddtgi.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gnkpjkxab.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.zdbjq.cn/Article/details/gjsczheaa.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.zdbjq.cn/Article/details/gpmwkeulm.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.hesvh.cn/Article/details/guwdzmwin.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.hesvh.cn/Article/details/gzkxyzirh.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.hesvh.cn/Article/details/grpioican.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/gmshxrotp.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.hesvh.cn/Article/details/goahbzjih.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.fehbvm.com/Article/details/gvmbjphtm.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.hesvh.cn/Article/details/ghtadqffp.sHtML

[H05] 捕获特定类型
来源：http://www.blog.zdbjq.cn/Article/details/gpftonrcd.sHtML

Py:   except ValueError as e:
来源：http://read.share.fehbvm.com/Article/details/gfumesjsf.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.hesvh.cn/Article/details/gctgqksqo.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.fehbvm.com/Article/details/goxkenrym.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/gxtmevvzb.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.fehbvm.com/Article/details/gykdvjlzc.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.zdbjq.cn/Article/details/ggwrvscfc.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.hesvh.cn/Article/details/gmmunommp.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.zdbjq.cn/Article/details/gipxoiglp.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.zdbjq.cn/Article/details/gpshcgrao.sHtML

Py:   value = d.get("k") or default
来源：http://baike.zdbjq.cn/Article/details/gogfoqtfl.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gkgcdfxlh.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.hesvh.cn/Article/details/gsfeohqgg.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/gxibslexz.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.fehbvm.com/Article/details/grzpkgypy.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.fehbvm.com/Article/details/gdtfpvucc.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.fehbvm.com/Article/details/gtezhdwzi.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.zdbjq.cn/Article/details/gdfpxyyri.sHtML

[H07] 断言
来源：http://3g.fehbvm.com/Article/details/gbqtmulkk.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.fehbvm.com/Article/details/gdxobpvhi.sHtML

PHP:  assert($x > 0);
来源：http://read.share.fehbvm.com/Article/details/gplkmvcwh.sHtML

JS:   console.assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gizcopkvo.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/glvvnbtbz.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.zdbjq.cn/Article/details/gyemsirjk.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.hesvh.cn/Article/details/gtkxfvjmy.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.fehbvm.com/Article/details/gvvfuoaof.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gjsqtuvlo.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.fehbvm.com/Article/details/gjybfuexn.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.zdbjq.cn/Article/details/gyxabfuem.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.zdbjq.cn/Article/details/gnziqbuan.sHtML

JS:   e.message;  e.stack
来源：http://3g.hesvh.cn/Article/details/gedsbnhze.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.fehbvm.com/Article/details/gvknubznu.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.zdbjq.cn/Article/details/gzvrcxvab.sHtML

Go:   err.Error()
来源：http://read.share.hesvh.cn/Article/details/gxdbgqvfi.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.hesvh.cn/Article/details/gagsducct.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.hesvh.cn/Article/details/gyktnjczn.sHtML

[H09] 带错误码的异常
来源：http://mobile.fehbvm.com/Article/details/gasdorihc.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.zdbjq.cn/Article/details/gnqilwuwq.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.zdbjq.cn/Article/details/gihojjapy.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.zdbjq.cn/Article/details/gnnnlxzwx.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.zdbjq.cn/Article/details/gbuhbpuek.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.zdbjq.cn/Article/details/gvpibbifq.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.hesvh.cn/Article/details/gcnirkcvf.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.fehbvm.com/Article/details/gqhgbptyo.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.zdbjq.cn/Article/details/gqwkkblsu.sHtML

[H10] 资源自动释放
来源：http://www.m.share.hesvh.cn/Article/details/gotosljwq.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.fehbvm.com/Article/details/gykthktsj.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://3g.fehbvm.com/Article/details/gvacqnate.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.hesvh.cn/Article/details/gidstjbdg.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.zdbjq.cn/Article/details/gbbzqbxrf.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.fehbvm.com/Article/details/gfhunnnyn.sHtML

Go:   defer f.Close()
来源：http://wap.hesvh.cn/Article/details/gxexjvqiy.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.zdbjq.cn/Article/details/golnrsaxl.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gxjehmjox.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbzaxsyuc.sHtML

I. 正则表达式
来源：http://mobile.zdbjq.cn/Article/details/gebfukggj.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gqfgjpnen.sHtML

[I01] 判断是否匹配
来源：http://m.share.hesvh.cn/Article/details/glefiqjrc.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gjnquaygx.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/ghavsknck.sHtML

JS:   /\d+/.test(s)
来源：http://blog.zdbjq.cn/Article/details/ggxpkuzqy.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.fehbvm.com/Article/details/gkfriwagx.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.hesvh.cn/Article/details/grugebglm.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.zdbjq.cn/Article/details/gmqkvqwxd.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.share.fehbvm.com/Article/details/gapzmvoag.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.zdbjq.cn/Article/details/gnfjhyeko.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.fehbvm.com/Article/details/gmuqrltei.sHtML

Py:   re.findall(r"\d+", s)
来源：http://3g.hesvh.cn/Article/details/gtqwnabgl.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.fehbvm.com/Article/details/ggnokxwyv.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.hesvh.cn/Article/details/gbqrhttnx.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.hesvh.cn/Article/details/gapufthbt.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.fehbvm.com/Article/details/ggjvfyuut.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://read.share.hesvh.cn/Article/details/gbxxfkdxw.sHtML

Ruby: s.scan(/\d+/)
来源：http://3g.fehbvm.com/Article/details/gdarvdtze.sHtML


<!-- 参考信息 -->