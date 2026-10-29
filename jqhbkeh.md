代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/gigifxvrr.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fehbvm.com/Article/details/ghnxmyrxt.sHtML

Ruby: Dir.children("dir")
来源：http://blog.fehbvm.com/Article/details/gtnrhwyyd.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.zdbjq.cn/Article/details/ghcxmugqi.sHtML

[F09] 获取文件大小
来源：http://wap.hesvh.cn/Article/details/grmhghuho.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.hesvh.cn/Article/details/gczoirzui.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gxdvcxmkz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.hesvh.cn/Article/details/gnoxmphys.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/guzcsanhh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gbbfausov.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.fehbvm.com/Article/details/gzyscgokg.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gscywznxy.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.fehbvm.com/Article/details/golkuzjlm.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.zdbjq.cn/Article/details/gbxizlvpw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gkhystrns.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.hesvh.cn/Article/details/gbzohtkxr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gwypznqei.sHtML

TS:   path.extname("a.txt")
来源：http://3g.hesvh.cn/Article/details/ghycvlbit.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.hesvh.cn/Article/details/gggqviszt.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gihriubzt.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/grwiyozeq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/guwyjgamr.sHtML

[F11] 复制与移动文件
来源：http://blog.hesvh.cn/Article/details/goszgtjwi.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gqgwwbkyy.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.fehbvm.com/Article/details/gylryjwpd.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gnikspgvc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gbhhcmlts.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.zdbjq.cn/Article/details/ggrshjmka.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.zdbjq.cn/Article/details/gtnjgtjwj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gmphnyhwm.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.fehbvm.com/Article/details/gghazwnrx.sHtML

[F12] CSV 读写
来源：http://baike.zdbjq.cn/Article/details/gnhwlsyqu.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.zdbjq.cn/Article/details/goeepnlow.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.fehbvm.com/Article/details/gdtanlmjx.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.fehbvm.com/Article/details/gzvtxbrln.sHtML

TS:   // 同上
来源：http://blog.hesvh.cn/Article/details/ggpnqxvab.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fehbvm.com/Article/details/gvitmukfa.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.zdbjq.cn/Article/details/gjnckkgfx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fehbvm.com/Article/details/giuwlcpnh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fehbvm.com/Article/details/gdbxnbbaz.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gbyjcypxh.sHtML

G. 面向对象
来源：http://www.share.hesvh.cn/Article/details/gqetmwgkq.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gcahyxtif.sHtML

[G01] 定义类
来源：http://wap.zdbjq.cn/Article/details/gqqcaclgu.sHtML

Py:   class User: pass
来源：http://read.share.zdbjq.cn/Article/details/goaajhmoz.sHtML

PHP:  class User {}
来源：http://www.share.hesvh.cn/Article/details/gtzbfewru.sHtML

JS:   class User {}
来源：http://mobile.hesvh.cn/Article/details/grpaduwgw.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.hesvh.cn/Article/details/gcadqmodt.sHtML

Java: class User {}
来源：http://3g.fehbvm.com/Article/details/gxiugtimd.sHtML

Go:   type User struct { Name string }
来源：http://read.share.fehbvm.com/Article/details/gsgcokril.sHtML

Ruby: class User; end
来源：http://3g.zdbjq.cn/Article/details/gxoskpwdq.sHtML

C#:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gxiefvawj.sHtML

[G02] 构造函数
来源：http://wap.hesvh.cn/Article/details/gaddcqwgf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/gmlqginau.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.hesvh.cn/Article/details/grygvhwda.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/glkgcfvdb.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.fehbvm.com/Article/details/gepviuesh.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/glekqyhdw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.fehbvm.com/Article/details/gkqprxbmu.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fehbvm.com/Article/details/gcmrgnfxd.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbsgnxqdn.sHtML

[G03] 实例属性
来源：http://www.blog.fehbvm.com/Article/details/gepgvemjr.sHtML

Py:   self.name = "x"
来源：http://3g.fehbvm.com/Article/details/gcsdqdosl.sHtML

PHP:  public string $name = "x";
来源：http://3g.zdbjq.cn/Article/details/gxflrwfik.sHtML

JS:   this.name = "x";
来源：http://mobile.fehbvm.com/Article/details/ggalqqisf.sHtML

TS:   name: string = "x";
来源：http://3g.zdbjq.cn/Article/details/giqgkeikz.sHtML

Java: private String name;
来源：http://baike.fehbvm.com/Article/details/gxvdvelsq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.hesvh.cn/Article/details/gqpczhvna.sHtML

Ruby: @name = "x"
来源：http://3g.hesvh.cn/Article/details/gmbacbhuv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.zdbjq.cn/Article/details/gasmkhlda.sHtML

[G04] 定义方法
来源：http://read.share.hesvh.cn/Article/details/guhdesndf.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gfwvufros.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gpnzorvqy.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gpehpxmjt.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gysbglzbr.sHtML

Java: String greet() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gvqfeecbq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gkdxxbwhi.sHtML

Ruby: def greet; @name; end
来源：http://mobile.hesvh.cn/Article/details/gwxeppjkb.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fehbvm.com/Article/details/gnmdtojwt.sHtML

[G05] 继承
来源：http://blog.hesvh.cn/Article/details/gqacxvfjp.sHtML

Py:   class Admin(User): pass
来源：http://baike.zdbjq.cn/Article/details/gerszwege.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gjagbxcbg.sHtML

JS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gdakeiuog.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gxkeqzkkr.sHtML

Java: class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gyqrqcyao.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.zdbjq.cn/Article/details/gwznncvwh.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.zdbjq.cn/Article/details/giigidwhg.sHtML

C#:   class Admin : User {}
来源：http://www.blog.hesvh.cn/Article/details/gdukbvacl.sHtML

[G06] 重写方法
来源：http://blog.fehbvm.com/Article/details/gvyizwyff.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.zdbjq.cn/Article/details/gexcrxffb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/giszhvolq.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gsntcufgk.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gaquilbje.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gscbeyawd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.zdbjq.cn/Article/details/gbznlulab.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.hesvh.cn/Article/details/gwkdnyohh.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fehbvm.com/Article/details/gzhunauyn.sHtML

[G07] 调用父类方法
来源：http://3g.zdbjq.cn/Article/details/gynbqxjnq.sHtML

Py:   super().greet()
来源：http://read.share.zdbjq.cn/Article/details/gkfmuufcx.sHtML

PHP:  parent::greet();
来源：http://baike.hesvh.cn/Article/details/gjsmwvfqa.sHtML

JS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gmmpkhbgs.sHtML

TS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gcwqvmylq.sHtML

Java: super.greet();
来源：http://read.share.hesvh.cn/Article/details/grwikvjvc.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.zdbjq.cn/Article/details/ghvticrde.sHtML

Ruby: super
来源：http://3g.hesvh.cn/Article/details/gtpsxnjgp.sHtML

C#:   base.Greet();
来源：http://www.blog.hesvh.cn/Article/details/gsruqfdnq.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.zdbjq.cn/Article/details/gbarlmxko.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.fehbvm.com/Article/details/gtzmcydhr.sHtML

PHP:  public static function f() {}
来源：http://read.share.hesvh.cn/Article/details/gcabbqcxw.sHtML

JS:   static f() {}
来源：http://www.share.zdbjq.cn/Article/details/ggjtahpus.sHtML

TS:   static f(): void {}
来源：http://www.share.hesvh.cn/Article/details/gdyufqrto.sHtML

Java: static void f() {}
来源：http://read.share.hesvh.cn/Article/details/guaxyutsd.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.zdbjq.cn/Article/details/gyvzayibo.sHtML

Ruby: def self.f; end
来源：http://mobile.hesvh.cn/Article/details/gwmobxxkx.sHtML

C#:   public static void F() {}
来源：http://www.share.hesvh.cn/Article/details/gixbiloxy.sHtML

[G09] 接口 / 抽象类
来源：http://wap.zdbjq.cn/Article/details/gkuztdisj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.zdbjq.cn/Article/details/ghwhuxjit.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.zdbjq.cn/Article/details/gslslzcty.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.hesvh.cn/Article/details/gynzzuqam.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.hesvh.cn/Article/details/ghrmcjrds.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.zdbjq.cn/Article/details/gvvsslftn.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.hesvh.cn/Article/details/grheydgim.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fehbvm.com/Article/details/gklzxqywd.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fehbvm.com/Article/details/gqhnvgesq.sHtML

[G10] 访问控制
来源：http://www.m.share.zdbjq.cn/Article/details/gzxibzzko.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.zdbjq.cn/Article/details/grtgghgjb.sHtML

PHP:  public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gufjcpjyd.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.fehbvm.com/Article/details/gnvdsbhcv.sHtML

TS:   public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gctqkllky.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.hesvh.cn/Article/details/gdizjpgyj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.zdbjq.cn/Article/details/ghfebhssx.sHtML

Ruby: public / protected / private
来源：http://www.share.hesvh.cn/Article/details/grzwjutgi.sHtML

C#:   public / protected / private / internal
来源：http://www.share.zdbjq.cn/Article/details/gajnesgir.sHtML

[G11] getter / setter
来源：http://blog.zdbjq.cn/Article/details/gqyrjfdlp.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fehbvm.com/Article/details/gexrskpuu.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gyeiaigeu.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/ggnurptrp.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/goaaxngdj.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gjfulvcbk.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gmbtamkng.sHtML

Ruby: attr_accessor :name
来源：http://baike.hesvh.cn/Article/details/gavmqgjwu.sHtML

C#:   public string Name { get; set; }
来源：http://baike.zdbjq.cn/Article/details/gfarzncjd.sHtML

[G12] 对象转字符串
来源：http://3g.fehbvm.com/Article/details/goidqeext.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gamaprxct.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gnvvipagj.sHtML

JS:   toString() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gtqaalfmw.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gbceznbpy.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.hesvh.cn/Article/details/ghxgzhfib.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/ggraydgly.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/grltrzmfb.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.hesvh.cn/Article/details/gfxtukpsb.sHtML

[G13] 判断对象类型
来源：http://baike.hesvh.cn/Article/details/guftxtxkj.sHtML

Py:   isinstance(u, User)
来源：http://blog.fehbvm.com/Article/details/gkyxqdsol.sHtML

PHP:  $u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/ghothreht.sHtML

JS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gbykfcgnh.sHtML

TS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gwzodciyo.sHtML

Java: u instanceof User
来源：http://wap.fehbvm.com/Article/details/gbxfibeop.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.fehbvm.com/Article/details/glpzvaton.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.zdbjq.cn/Article/details/geflmkrgn.sHtML

C#:   u is User
来源：http://mobile.zdbjq.cn/Article/details/gjiioczcs.sHtML

[G14] 数据类 / record
来源：http://baike.hesvh.cn/Article/details/gexupxsak.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.hesvh.cn/Article/details/gndesplrj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.hesvh.cn/Article/details/gmninwemo.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.hesvh.cn/Article/details/gnannstjd.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.zdbjq.cn/Article/details/ggijehuib.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.fehbvm.com/Article/details/gdickxglx.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.hesvh.cn/Article/details/gdpavacwn.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.fehbvm.com/Article/details/gcfyckjzi.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.zdbjq.cn/Article/details/ggdpvgrtf.sHtML

[G15] 枚举
来源：http://read.share.zdbjq.cn/Article/details/guofvathv.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.zdbjq.cn/Article/details/gngmdzepn.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fehbvm.com/Article/details/gqcxesnrd.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.zdbjq.cn/Article/details/gunaoxdkk.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.hesvh.cn/Article/details/gadhtajtg.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.zdbjq.cn/Article/details/grnjpcmsq.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.fehbvm.com/Article/details/guxlwfuly.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.zdbjq.cn/Article/details/glhdypqij.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gcesoyrul.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.zdbjq.cn/Article/details/gxpcscnrn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.zdbjq.cn/Article/details/gtsedbtcj.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.fehbvm.com/Article/details/gfqjrftac.sHtML

JS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/ghoemolfo.sHtML

TS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/gvxtscxjx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.zdbjq.cn/Article/details/gytrtliwb.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.fehbvm.com/Article/details/glewxhgqf.sHtML

Ruby: obj.instance_variables
来源：http://3g.zdbjq.cn/Article/details/gtayyscbl.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.zdbjq.cn/Article/details/grgeuzcsm.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gnoqubvtd.sHtML

H. 异常与错误处理
来源：http://m.share.zdbjq.cn/Article/details/gmuvtxacr.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gzftjmxzg.sHtML

[H01] try / catch 基础
来源：http://blog.zdbjq.cn/Article/details/gbqsouhzb.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.hesvh.cn/Article/details/gntinzmst.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.zdbjq.cn/Article/details/grymbtyyc.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/glkemzwrl.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gciaqpziq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.hesvh.cn/Article/details/gygwirjic.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.fehbvm.com/Article/details/gsrrvmkty.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.fehbvm.com/Article/details/gakkaghsl.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.zdbjq.cn/Article/details/ggcicuwzi.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.fehbvm.com/Article/details/ghjdjwcca.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.zdbjq.cn/Article/details/gvxxdruac.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gfdkktqvu.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/glhibmclc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/ghtjmsvww.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gazozseqd.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.hesvh.cn/Article/details/gmtmlhkej.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.fehbvm.com/Article/details/gzhgbsedb.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.fehbvm.com/Article/details/govnduyiq.sHtML

[H03] 主动抛出异常
来源：http://read.share.hesvh.cn/Article/details/gwvqmwqez.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.fehbvm.com/Article/details/givbtpcxl.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gnaxybejq.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/gdnzesogh.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gwbipjchq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gecdogxmk.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.zdbjq.cn/Article/details/gfeedhljv.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.zdbjq.cn/Article/details/gtzcuoplt.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/giqijfrxp.sHtML

[H04] 自定义异常类型
来源：http://wap.zdbjq.cn/Article/details/goucnxhcp.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.hesvh.cn/Article/details/gxwceuiul.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.hesvh.cn/Article/details/guzmwjqwz.sHtML

JS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/gnjfjsmpt.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.zdbjq.cn/Article/details/gzguoauxw.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.fehbvm.com/Article/details/glnhtaixt.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.hesvh.cn/Article/details/gddgikupc.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.hesvh.cn/Article/details/gmlczvhbd.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.zdbjq.cn/Article/details/gerkpjske.sHtML

[H05] 捕获特定类型
来源：http://www.share.fehbvm.com/Article/details/gdcsajtzz.sHtML

Py:   except ValueError as e:
来源：http://m.share.zdbjq.cn/Article/details/gjgypjfmt.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.fehbvm.com/Article/details/gxfxkqiys.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/gjuyefmyj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.fehbvm.com/Article/details/gbznwxghl.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.hesvh.cn/Article/details/ghezsdbrr.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.hesvh.cn/Article/details/ggcrbdbnm.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.zdbjq.cn/Article/details/goetraoop.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.fehbvm.com/Article/details/geebgrosq.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.zdbjq.cn/Article/details/goynommvl.sHtML

Py:   value = d.get("k") or default
来源：http://blog.hesvh.cn/Article/details/gfreobgvu.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gbodaleqc.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/grkqfhmch.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/gugtpxssz.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.hesvh.cn/Article/details/giquuipmo.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.zdbjq.cn/Article/details/gabkmxpiq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.zdbjq.cn/Article/details/gadesuxuk.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.fehbvm.com/Article/details/gajvoeonv.sHtML

[H07] 断言
来源：http://blog.zdbjq.cn/Article/details/gzdsvfice.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.hesvh.cn/Article/details/grihrdqvd.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gdlqtmbqd.sHtML

JS:   console.assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/ggudmqknl.sHtML

TS:   console.assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gxssrdkwc.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.hesvh.cn/Article/details/gchfskcmy.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.fehbvm.com/Article/details/gkxsbqzon.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.fehbvm.com/Article/details/gmzzefmci.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gtxtvpthv.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.fehbvm.com/Article/details/gywiirofq.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.hesvh.cn/Article/details/gjqtwvhja.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.hesvh.cn/Article/details/gbdiaaelu.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.zdbjq.cn/Article/details/gbnachdbm.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.hesvh.cn/Article/details/gkagnjcnk.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.hesvh.cn/Article/details/gzqwyymir.sHtML

Go:   err.Error()
来源：http://mobile.hesvh.cn/Article/details/gfrrbrqzq.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.zdbjq.cn/Article/details/glcarsajy.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.hesvh.cn/Article/details/goopwhmdb.sHtML

[H09] 带错误码的异常
来源：http://www.share.zdbjq.cn/Article/details/gdtekmyxz.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.fehbvm.com/Article/details/gtttwdwda.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.fehbvm.com/Article/details/gxwuiibxr.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.fehbvm.com/Article/details/gfkkijqes.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.fehbvm.com/Article/details/grqhnbnpa.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.hesvh.cn/Article/details/gmhmaccxl.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.fehbvm.com/Article/details/gdwedqtfm.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.fehbvm.com/Article/details/gvvenyerv.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.fehbvm.com/Article/details/gfwfckvws.sHtML

[H10] 资源自动释放
来源：http://wap.zdbjq.cn/Article/details/gvfpynqqb.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.fehbvm.com/Article/details/gfiqdpimz.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.fehbvm.com/Article/details/gryxfnrmb.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.zdbjq.cn/Article/details/gdfeudprt.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fehbvm.com/Article/details/glwadoual.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.fehbvm.com/Article/details/gmeiyyfrz.sHtML

Go:   defer f.Close()
来源：http://mobile.zdbjq.cn/Article/details/gyvexxkeg.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://mobile.fehbvm.com/Article/details/gayrfuuip.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.fehbvm.com/Article/details/grfesavrq.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ghocdgwqv.sHtML

I. 正则表达式
来源：http://baike.zdbjq.cn/Article/details/gannhwddi.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gpgdkfomg.sHtML

[I01] 判断是否匹配
来源：http://wap.hesvh.cn/Article/details/ggbxejogq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.hesvh.cn/Article/details/gjukwvslv.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gzppbjjny.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.hesvh.cn/Article/details/gfrlpfikv.sHtML

TS:   /\d+/.test(s)
来源：http://wap.zdbjq.cn/Article/details/gcztqfoyo.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://read.share.fehbvm.com/Article/details/gingfgbwx.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.fehbvm.com/Article/details/gqqzprecc.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.hesvh.cn/Article/details/ggagertho.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.fehbvm.com/Article/details/grddgznat.sHtML

[I02] 提取所有匹配
来源：http://mobile.zdbjq.cn/Article/details/gvgpmxyil.sHtML

Py:   re.findall(r"\d+", s)
来源：http://baike.zdbjq.cn/Article/details/grixxexcw.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.zdbjq.cn/Article/details/gmzugehij.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.zdbjq.cn/Article/details/gvcrujzkc.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.zdbjq.cn/Article/details/gjqamrkxb.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.fehbvm.com/Article/details/gdhaszjod.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.hesvh.cn/Article/details/gzugcansh.sHtML

Ruby: s.scan(/\d+/)
来源：http://blog.hesvh.cn/Article/details/gsdjfagwo.sHtML


<!-- 参考信息 -->