代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gyaqbrknh.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.zdbjq.cn/Article/details/gfwczuaed.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fehbvm.com/Article/details/guublvrqc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.fehbvm.com/Article/details/gqfecaaab.sHtML

[F09] 获取文件大小
来源：http://m.share.hesvh.cn/Article/details/gxqaypxzs.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fehbvm.com/Article/details/ggljxwton.sHtML

PHP:  filesize("a.txt");
来源：http://3g.zdbjq.cn/Article/details/ggmkippas.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gnhnrjxbw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gizxpykpo.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gqnngykyn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.hesvh.cn/Article/details/gzlepxqaf.sHtML

Ruby: File.size("a.txt")
来源：http://baike.hesvh.cn/Article/details/ggekeqxoj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.hesvh.cn/Article/details/godrcqeot.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.fehbvm.com/Article/details/glgdgdixy.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gqvipmphc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.zdbjq.cn/Article/details/ghyuiangw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gvsgarskt.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fehbvm.com/Article/details/gpsqzuows.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.zdbjq.cn/Article/details/gxmuhhpew.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gfafmajzb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/geqhagduz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gmurwhcim.sHtML

[F11] 复制与移动文件
来源：http://mobile.hesvh.cn/Article/details/gxyydizye.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ggldjgock.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.fehbvm.com/Article/details/gledtugki.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gyaokofil.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/ghejhgmwp.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.hesvh.cn/Article/details/gquajjhaa.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.hesvh.cn/Article/details/gdwwahile.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gnxiloojq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fehbvm.com/Article/details/gppxkkimk.sHtML

[F12] CSV 读写
来源：http://mobile.zdbjq.cn/Article/details/gemmdrhva.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.zdbjq.cn/Article/details/gkijydyft.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fehbvm.com/Article/details/gbbllsnxg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.fehbvm.com/Article/details/gyvazonyw.sHtML

TS:   // 同上
来源：http://wap.hesvh.cn/Article/details/gaaxhdnhu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fehbvm.com/Article/details/gudwbdinl.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.hesvh.cn/Article/details/gmznbjuwq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.hesvh.cn/Article/details/grmuwoydn.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.zdbjq.cn/Article/details/gmmjevytu.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ggolbyiqb.sHtML

G. 面向对象
来源：http://blog.fehbvm.com/Article/details/gtsfgitql.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gghjfvfft.sHtML

[G01] 定义类
来源：http://baike.hesvh.cn/Article/details/gttzpkkue.sHtML

Py:   class User: pass
来源：http://www.m.share.hesvh.cn/Article/details/gobershvn.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/gruwkxvln.sHtML

JS:   class User {}
来源：http://3g.zdbjq.cn/Article/details/ghuthpfrs.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.fehbvm.com/Article/details/gqjphqttj.sHtML

Java: class User {}
来源：http://wap.zdbjq.cn/Article/details/ggvcnccrl.sHtML

Go:   type User struct { Name string }
来源：http://www.share.hesvh.cn/Article/details/gckqxmcjm.sHtML

Ruby: class User; end
来源：http://wap.fehbvm.com/Article/details/ggvnxyvml.sHtML

C#:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/garzrsbpn.sHtML

[G02] 构造函数
来源：http://3g.hesvh.cn/Article/details/gitsofdfh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.zdbjq.cn/Article/details/gnjlcfmfx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.zdbjq.cn/Article/details/gyronuudh.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gkglnzxki.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.fehbvm.com/Article/details/gnvyjnffv.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gltqbizai.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.zdbjq.cn/Article/details/gzmjwalmm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fehbvm.com/Article/details/gczvdloly.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.hesvh.cn/Article/details/gtgasedcr.sHtML

[G03] 实例属性
来源：http://baike.hesvh.cn/Article/details/gfzygavix.sHtML

Py:   self.name = "x"
来源：http://read.share.hesvh.cn/Article/details/gxnpjjzti.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gfxtijukh.sHtML

JS:   this.name = "x";
来源：http://mobile.hesvh.cn/Article/details/gjfpbffes.sHtML

TS:   name: string = "x";
来源：http://mobile.hesvh.cn/Article/details/gykidwfid.sHtML

Java: private String name;
来源：http://read.share.fehbvm.com/Article/details/gnallmeoo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.zdbjq.cn/Article/details/gfypnypcb.sHtML

Ruby: @name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gshtqoima.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.zdbjq.cn/Article/details/gemlojzrt.sHtML

[G04] 定义方法
来源：http://read.share.hesvh.cn/Article/details/gbbpdbppe.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gpgazqklh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gccgwrcnj.sHtML

JS:   greet() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gmawvgcdz.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/grydujadh.sHtML

Java: String greet() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gqsxlxxsh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gkmodlsuc.sHtML

Ruby: def greet; @name; end
来源：http://m.share.hesvh.cn/Article/details/gmgxxpnky.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fehbvm.com/Article/details/ghskltkva.sHtML

[G05] 继承
来源：http://www.m.share.fehbvm.com/Article/details/gpricbrbx.sHtML

Py:   class Admin(User): pass
来源：http://m.share.hesvh.cn/Article/details/gjijojtmw.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gsfyifsra.sHtML

JS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gaqdawnjy.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gsxfxcpuw.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gauixdedo.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.zdbjq.cn/Article/details/goagpewnr.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.fehbvm.com/Article/details/gbieppkiy.sHtML

C#:   class Admin : User {}
来源：http://baike.fehbvm.com/Article/details/gpebpjnja.sHtML

[G06] 重写方法
来源：http://read.share.hesvh.cn/Article/details/givvrnzrm.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fehbvm.com/Article/details/gzeekmcjy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gumhaqnbr.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gzbhpqosx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gggsumirh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gdqwesyvg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.zdbjq.cn/Article/details/gjtsfflnc.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.hesvh.cn/Article/details/gepvpgbwf.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fehbvm.com/Article/details/gfbuadecg.sHtML

[G07] 调用父类方法
来源：http://baike.fehbvm.com/Article/details/guupxawon.sHtML

Py:   super().greet()
来源：http://read.share.fehbvm.com/Article/details/gzrbehado.sHtML

PHP:  parent::greet();
来源：http://3g.fehbvm.com/Article/details/goxnkogyd.sHtML

JS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gbycvzdrt.sHtML

TS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gtifhsbsp.sHtML

Java: super.greet();
来源：http://www.share.hesvh.cn/Article/details/guqsngcvo.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.hesvh.cn/Article/details/gbhbkvjzm.sHtML

Ruby: super
来源：http://www.share.zdbjq.cn/Article/details/gzydjjqew.sHtML

C#:   base.Greet();
来源：http://www.share.fehbvm.com/Article/details/gegzhzins.sHtML

[G08] 静态方法与属性
来源：http://www.blog.zdbjq.cn/Article/details/gnhrdsucn.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.hesvh.cn/Article/details/gqpvlyyfg.sHtML

PHP:  public static function f() {}
来源：http://wap.fehbvm.com/Article/details/gentpnsxd.sHtML

JS:   static f() {}
来源：http://blog.fehbvm.com/Article/details/gkczwvqto.sHtML

TS:   static f(): void {}
来源：http://read.share.fehbvm.com/Article/details/gwujcrwds.sHtML

Java: static void f() {}
来源：http://wap.zdbjq.cn/Article/details/gklxoijov.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.zdbjq.cn/Article/details/gjcugfate.sHtML

Ruby: def self.f; end
来源：http://read.share.zdbjq.cn/Article/details/gjishyydb.sHtML

C#:   public static void F() {}
来源：http://blog.hesvh.cn/Article/details/gvmcvisto.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fehbvm.com/Article/details/gbiqtwiza.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.zdbjq.cn/Article/details/ginhqymex.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.fehbvm.com/Article/details/gqiuuiyzf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.hesvh.cn/Article/details/gvuvweotn.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.fehbvm.com/Article/details/grhfgfatm.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.zdbjq.cn/Article/details/gzhisgujc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.zdbjq.cn/Article/details/gbvujvztt.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.hesvh.cn/Article/details/gcwtodykm.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fehbvm.com/Article/details/ggcuolkhi.sHtML

[G10] 访问控制
来源：http://mobile.fehbvm.com/Article/details/gmjazlchn.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.hesvh.cn/Article/details/gkdrhopka.sHtML

PHP:  public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gvkdcumdf.sHtML

JS:   #private 字段；其余公开
来源：http://wap.fehbvm.com/Article/details/gbvxbobsp.sHtML

TS:   public / protected / private
来源：http://www.share.fehbvm.com/Article/details/ghdvrafzp.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.zdbjq.cn/Article/details/gbgidkuyf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.hesvh.cn/Article/details/geuyikdyq.sHtML

Ruby: public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gpzyrbljz.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.fehbvm.com/Article/details/giggnjcut.sHtML

[G11] getter / setter
来源：http://read.share.hesvh.cn/Article/details/gkfigpwdw.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.fehbvm.com/Article/details/gwhwwuodb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gbxkagfpn.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gzoxlvnjw.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gpkwwrwnf.sHtML

Java: public String getName() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gnonuntmi.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gwbcefrvj.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.hesvh.cn/Article/details/gbyprksyr.sHtML

C#:   public string Name { get; set; }
来源：http://wap.fehbvm.com/Article/details/gxshtojad.sHtML

[G12] 对象转字符串
来源：http://blog.zdbjq.cn/Article/details/geuokbkvq.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gibrrzded.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gfnngvsfc.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/ggjfzkvge.sHtML

TS:   toString(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gmkmzxlqt.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gfvbnpxxs.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gazlmdhku.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fehbvm.com/Article/details/gxmkwroia.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.zdbjq.cn/Article/details/gppgshxad.sHtML

[G13] 判断对象类型
来源：http://m.share.zdbjq.cn/Article/details/gkpozciha.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.zdbjq.cn/Article/details/gdvfvhkex.sHtML

PHP:  $u instanceof User
来源：http://baike.hesvh.cn/Article/details/gohwmqhey.sHtML

JS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/gpoualykq.sHtML

TS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gxgbwkhsc.sHtML

Java: u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gmulqhmpn.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.hesvh.cn/Article/details/gynzgnlmo.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.hesvh.cn/Article/details/glinszttb.sHtML

C#:   u is User
来源：http://www.share.hesvh.cn/Article/details/gggfbwpia.sHtML

[G14] 数据类 / record
来源：http://www.share.zdbjq.cn/Article/details/gwnejryhh.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.zdbjq.cn/Article/details/gbmiszyuq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.fehbvm.com/Article/details/gilntinjo.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.zdbjq.cn/Article/details/gvtecoctt.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.hesvh.cn/Article/details/gxnbjxoqs.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.fehbvm.com/Article/details/gxjgeyhwj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.hesvh.cn/Article/details/gkrhiqayx.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.fehbvm.com/Article/details/gqhpzsonp.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.hesvh.cn/Article/details/gevczxrtl.sHtML

[G15] 枚举
来源：http://blog.hesvh.cn/Article/details/gzyccazoq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.zdbjq.cn/Article/details/ggsccvndc.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.fehbvm.com/Article/details/gqkwiiksr.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.hesvh.cn/Article/details/gxxtzadhb.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/gzwkejujc.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.zdbjq.cn/Article/details/gyushvtfk.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.zdbjq.cn/Article/details/gtthagied.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.zdbjq.cn/Article/details/glwwtetum.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gxppfippr.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.fehbvm.com/Article/details/gizbekezx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.fehbvm.com/Article/details/gngqwhvwn.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.zdbjq.cn/Article/details/giuabjcbn.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.fehbvm.com/Article/details/gtzeoexda.sHtML

TS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/grorfewhp.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.zdbjq.cn/Article/details/gobcbnfkl.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.hesvh.cn/Article/details/gscaujiqi.sHtML

Ruby: obj.instance_variables
来源：http://www.share.hesvh.cn/Article/details/gwtswvenm.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.hesvh.cn/Article/details/gbzwcihyj.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/goeglcaff.sHtML

H. 异常与错误处理
来源：http://www.blog.zdbjq.cn/Article/details/grlysmxze.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxvuzufgz.sHtML

[H01] try / catch 基础
来源：http://www.m.share.hesvh.cn/Article/details/gvconrwmr.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.zdbjq.cn/Article/details/gxiwmuvst.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.fehbvm.com/Article/details/gguimokuu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/glsvaszfy.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/grkhutiky.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.fehbvm.com/Article/details/gjyzwvstb.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.fehbvm.com/Article/details/gxmqsdlnn.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.hesvh.cn/Article/details/gwmgvcnyv.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.fehbvm.com/Article/details/gbrfolczw.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.zdbjq.cn/Article/details/gmrguvfzk.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.zdbjq.cn/Article/details/gwutmlmvx.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gprxtdxrb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gvvumsyvd.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gknjgitmv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gassnaxvj.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.hesvh.cn/Article/details/gzxdiexfd.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.zdbjq.cn/Article/details/gdyhebpqs.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gjjlhbvda.sHtML

[H03] 主动抛出异常
来源：http://www.share.hesvh.cn/Article/details/gcsinvwvt.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.fehbvm.com/Article/details/gzbqdamvh.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/getfpucic.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gkgljgaxp.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.fehbvm.com/Article/details/gagnnipkg.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gwqlmpvbt.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.zdbjq.cn/Article/details/gvnqbtwhv.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.fehbvm.com/Article/details/gijdthmay.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gwjlsrzrz.sHtML

[H04] 自定义异常类型
来源：http://www.share.fehbvm.com/Article/details/gpkgseeva.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.zdbjq.cn/Article/details/gnvrkbmif.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/ghiaaedex.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.zdbjq.cn/Article/details/gqgcdyqap.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.zdbjq.cn/Article/details/gjluymubp.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/gzvoittsv.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.hesvh.cn/Article/details/geqvyufeb.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.hesvh.cn/Article/details/glfvnmxsi.sHtML

C#:   class MyException : Exception {}
来源：http://3g.zdbjq.cn/Article/details/gfxkhfrnq.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.zdbjq.cn/Article/details/gofobbnfj.sHtML

Py:   except ValueError as e:
来源：http://read.share.zdbjq.cn/Article/details/gcvkukrbo.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.fehbvm.com/Article/details/gkmcshcqq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.hesvh.cn/Article/details/gpmtwlecp.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/gqhgpqbbm.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.zdbjq.cn/Article/details/gfvxrpaqj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.fehbvm.com/Article/details/gdpgwbdlg.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.hesvh.cn/Article/details/gaplsulvg.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.hesvh.cn/Article/details/gsyllpszp.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.fehbvm.com/Article/details/gnzrwltci.sHtML

Py:   value = d.get("k") or default
来源：http://3g.zdbjq.cn/Article/details/gqnppdfcr.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.hesvh.cn/Article/details/ginzrlusl.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fehbvm.com/Article/details/gjaanviph.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/gpkuexjic.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.zdbjq.cn/Article/details/glgrdnzqg.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.hesvh.cn/Article/details/ggilejffq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.hesvh.cn/Article/details/gspggmgto.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.fehbvm.com/Article/details/gboiiiwsj.sHtML

[H07] 断言
来源：http://www.blog.zdbjq.cn/Article/details/gvxluajpl.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.hesvh.cn/Article/details/gydlocdna.sHtML

PHP:  assert($x > 0);
来源：http://blog.fehbvm.com/Article/details/gjwuqudlj.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gdusczogv.sHtML

TS:   console.assert(x > 0);
来源：http://wap.zdbjq.cn/Article/details/gfwhyoupb.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.fehbvm.com/Article/details/gvemjnnus.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.zdbjq.cn/Article/details/gswgacgfp.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.zdbjq.cn/Article/details/gcljufwqz.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gnowcnbbw.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.fehbvm.com/Article/details/gjmlhztpl.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.zdbjq.cn/Article/details/gkcurkktk.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.hesvh.cn/Article/details/gdrcwhwsk.sHtML

JS:   e.message;  e.stack
来源：http://www.m.share.hesvh.cn/Article/details/grgrxnhvr.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.fehbvm.com/Article/details/ghziqsavz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.zdbjq.cn/Article/details/grptgxpcg.sHtML

Go:   err.Error()
来源：http://wap.zdbjq.cn/Article/details/gwnsgzovj.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.fehbvm.com/Article/details/gzvaerjoi.sHtML

C#:   e.Message;  e.StackTrace
来源：http://read.share.zdbjq.cn/Article/details/glwokazbn.sHtML

[H09] 带错误码的异常
来源：http://blog.zdbjq.cn/Article/details/gyqngowha.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.hesvh.cn/Article/details/glvtffkyh.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.fehbvm.com/Article/details/gwyhmriiz.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.zdbjq.cn/Article/details/gfaolrxih.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.zdbjq.cn/Article/details/gkzzokyth.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.hesvh.cn/Article/details/gwzknjlbu.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://m.share.zdbjq.cn/Article/details/gstmwibru.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.zdbjq.cn/Article/details/gnkuylnnt.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.fehbvm.com/Article/details/gvrmhjzva.sHtML

[H10] 资源自动释放
来源：http://wap.zdbjq.cn/Article/details/gcfypnytn.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.hesvh.cn/Article/details/gswhncpbz.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.fehbvm.com/Article/details/gbktmugzk.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.zdbjq.cn/Article/details/grvoopgqx.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.zdbjq.cn/Article/details/gsuhnouoe.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.zdbjq.cn/Article/details/gjucfpzuq.sHtML

Go:   defer f.Close()
来源：http://www.blog.zdbjq.cn/Article/details/griixhrih.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.fehbvm.com/Article/details/gfhdtvjre.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gwquwlmeg.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gbketizht.sHtML

I. 正则表达式
来源：http://baike.zdbjq.cn/Article/details/gkizyjcld.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/guhufjabm.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gdnlpfgvb.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.fehbvm.com/Article/details/glumbrseq.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/goolbukuc.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.zdbjq.cn/Article/details/gqacjmoxm.sHtML

TS:   /\d+/.test(s)
来源：http://wap.zdbjq.cn/Article/details/ghvvivzzz.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.fehbvm.com/Article/details/gcsaexgfz.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://read.share.zdbjq.cn/Article/details/gpueqgwqg.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.zdbjq.cn/Article/details/gdnaxsoor.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.hesvh.cn/Article/details/gwkoxszgr.sHtML

[I02] 提取所有匹配
来源：http://m.share.fehbvm.com/Article/details/gzpdokvcd.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.share.zdbjq.cn/Article/details/gkugnwmco.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.fehbvm.com/Article/details/gaqhwppmd.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://baike.zdbjq.cn/Article/details/gzwoexkng.sHtML

TS:   s.match(/\d+/g)
来源：http://read.share.fehbvm.com/Article/details/gqnmefbeq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.zdbjq.cn/Article/details/gilmqyjkr.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.zdbjq.cn/Article/details/gelcjerix.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.fehbvm.com/Article/details/gpwjxmadb.sHtML


<!-- 参考信息 -->