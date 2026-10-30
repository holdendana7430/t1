代发 wailian999

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/gjrnexvwf.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fehbvm.com/Article/details/gtnkjytwo.sHtML

Ruby: Dir.children("dir")
来源：http://blog.fehbvm.com/Article/details/grensnunf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fehbvm.com/Article/details/gfghqkmfk.sHtML

[F09] 获取文件大小
来源：http://blog.hesvh.cn/Article/details/glheulmsv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gqpsqqwck.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.fehbvm.com/Article/details/guaxnujxg.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gfsmmceei.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/gtaqteaqv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gikumjjyf.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.hesvh.cn/Article/details/gwcdaxbcv.sHtML

Ruby: File.size("a.txt")
来源：http://baike.hesvh.cn/Article/details/gckgivcsv.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.fehbvm.com/Article/details/gnqzysmat.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fehbvm.com/Article/details/gcjouipnh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gplxdeotv.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fehbvm.com/Article/details/gpkdvzxeb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gwhfpexhs.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.hesvh.cn/Article/details/geofgtehn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.fehbvm.com/Article/details/guoltvnfr.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gjnqixkzx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gcwdmpdex.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/groixndvk.sHtML

[F11] 复制与移动文件
来源：http://read.share.fehbvm.com/Article/details/goqscdxms.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gfzjzqrqv.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.zdbjq.cn/Article/details/genuuojel.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gmcgttsln.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/glhfzizio.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.hesvh.cn/Article/details/genndcbxp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.hesvh.cn/Article/details/gqpydveyp.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gtuekfaba.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.zdbjq.cn/Article/details/guunomavd.sHtML

[F12] CSV 读写
来源：http://www.blog.fehbvm.com/Article/details/gjyzpejrn.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.zdbjq.cn/Article/details/gdnmaixng.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.zdbjq.cn/Article/details/gsvekzfoy.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.zdbjq.cn/Article/details/gaevxoshy.sHtML

TS:   // 同上
来源：http://baike.fehbvm.com/Article/details/gvnbitogb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.hesvh.cn/Article/details/gqymjkvrc.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.fehbvm.com/Article/details/gnndkjqxz.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.fehbvm.com/Article/details/gaisciohk.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.zdbjq.cn/Article/details/gwmxaawqp.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gfgncvaam.sHtML

G. 面向对象
来源：http://3g.hesvh.cn/Article/details/gdsrvnobq.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gwqjqcxhk.sHtML

[G01] 定义类
来源：http://baike.fehbvm.com/Article/details/gmngetenn.sHtML

Py:   class User: pass
来源：http://www.blog.fehbvm.com/Article/details/ghwnmnqdo.sHtML

PHP:  class User {}
来源：http://blog.zdbjq.cn/Article/details/gqlkzldzv.sHtML

JS:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gommtwnff.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.zdbjq.cn/Article/details/gilmhqjpm.sHtML

Java: class User {}
来源：http://www.share.fehbvm.com/Article/details/gtrtzuwae.sHtML

Go:   type User struct { Name string }
来源：http://read.share.zdbjq.cn/Article/details/gjeafrvsu.sHtML

Ruby: class User; end
来源：http://www.share.hesvh.cn/Article/details/gnqrctros.sHtML

C#:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/gpukknlpw.sHtML

[G02] 构造函数
来源：http://blog.hesvh.cn/Article/details/glpwanyxa.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.hesvh.cn/Article/details/gofbgqabx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.hesvh.cn/Article/details/gyrcmevza.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gozzgzmge.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fehbvm.com/Article/details/gynjosdpj.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gwekjzbyd.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.zdbjq.cn/Article/details/gkgfevkld.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.hesvh.cn/Article/details/ggjuewqgy.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.fehbvm.com/Article/details/grmugauyz.sHtML

[G03] 实例属性
来源：http://blog.fehbvm.com/Article/details/giuzkamnl.sHtML

Py:   self.name = "x"
来源：http://wap.fehbvm.com/Article/details/gpfmyozmz.sHtML

PHP:  public string $name = "x";
来源：http://read.share.zdbjq.cn/Article/details/ghlqqnssz.sHtML

JS:   this.name = "x";
来源：http://www.blog.hesvh.cn/Article/details/gnxqtwchw.sHtML

TS:   name: string = "x";
来源：http://read.share.hesvh.cn/Article/details/godflzgwr.sHtML

Java: private String name;
来源：http://wap.hesvh.cn/Article/details/gtahbfrxl.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fehbvm.com/Article/details/ghqdlchbm.sHtML

Ruby: @name = "x"
来源：http://3g.zdbjq.cn/Article/details/gezkrjiqp.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.fehbvm.com/Article/details/gzpvosvkb.sHtML

[G04] 定义方法
来源：http://www.m.share.hesvh.cn/Article/details/gvrydhhtd.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gbeoezmvd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gopredjiu.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gguvdskfw.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gnxtfidfi.sHtML

Java: String greet() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gjrziymlw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gzqpufubd.sHtML

Ruby: def greet; @name; end
来源：http://baike.hesvh.cn/Article/details/galtximor.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.fehbvm.com/Article/details/gxduggcsi.sHtML

[G05] 继承
来源：http://m.share.zdbjq.cn/Article/details/gdxkczyhq.sHtML

Py:   class Admin(User): pass
来源：http://www.share.hesvh.cn/Article/details/gwwofnmhf.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gnvxyhlus.sHtML

JS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/ghwnkkosv.sHtML

TS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gzdkqudrh.sHtML

Java: class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gjhwbgevp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fehbvm.com/Article/details/gjfblsfco.sHtML

Ruby: class Admin < User; end
来源：http://read.share.zdbjq.cn/Article/details/gjxncwmzz.sHtML

C#:   class Admin : User {}
来源：http://3g.fehbvm.com/Article/details/gnxgnunvd.sHtML

[G06] 重写方法
来源：http://blog.zdbjq.cn/Article/details/gsrmkvoqy.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.zdbjq.cn/Article/details/glefvqufd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gohfhvycu.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gnogzyvga.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gpxzogtkn.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gzaesdwov.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.zdbjq.cn/Article/details/gptsotsly.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fehbvm.com/Article/details/godffekca.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.zdbjq.cn/Article/details/gutnweufg.sHtML

[G07] 调用父类方法
来源：http://baike.hesvh.cn/Article/details/gnsbrzejr.sHtML

Py:   super().greet()
来源：http://wap.hesvh.cn/Article/details/gjtgqjqzh.sHtML

PHP:  parent::greet();
来源：http://3g.fehbvm.com/Article/details/gmbbzucvu.sHtML

JS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gvahruaif.sHtML

TS:   super.greet();
来源：http://m.share.hesvh.cn/Article/details/gymqrsvzi.sHtML

Java: super.greet();
来源：http://3g.fehbvm.com/Article/details/gaggjkaqd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.zdbjq.cn/Article/details/gscuqjstb.sHtML

Ruby: super
来源：http://read.share.hesvh.cn/Article/details/gvipxuiaz.sHtML

C#:   base.Greet();
来源：http://m.share.zdbjq.cn/Article/details/gnqnoztwg.sHtML

[G08] 静态方法与属性
来源：http://baike.hesvh.cn/Article/details/gccgjowae.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.hesvh.cn/Article/details/gepsvuhls.sHtML

PHP:  public static function f() {}
来源：http://3g.hesvh.cn/Article/details/gkgvlbhkx.sHtML

JS:   static f() {}
来源：http://m.share.hesvh.cn/Article/details/ggakibjbi.sHtML

TS:   static f(): void {}
来源：http://read.share.zdbjq.cn/Article/details/gnzjvirgk.sHtML

Java: static void f() {}
来源：http://www.share.zdbjq.cn/Article/details/gwymlysmy.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.hesvh.cn/Article/details/gaxkmtbub.sHtML

Ruby: def self.f; end
来源：http://www.blog.fehbvm.com/Article/details/guhlipaoo.sHtML

C#:   public static void F() {}
来源：http://baike.hesvh.cn/Article/details/gwraygthg.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.hesvh.cn/Article/details/gvlsaicvf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.fehbvm.com/Article/details/ggdlguigb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.fehbvm.com/Article/details/gqrqmpbme.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.zdbjq.cn/Article/details/gmgwfvljf.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.hesvh.cn/Article/details/gnhyzbqyy.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.zdbjq.cn/Article/details/geijuxhwp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.hesvh.cn/Article/details/gxcgzxyrj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.hesvh.cn/Article/details/gmaowruxt.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.zdbjq.cn/Article/details/gwdzgwmai.sHtML

[G10] 访问控制
来源：http://wap.zdbjq.cn/Article/details/genuqaepd.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.zdbjq.cn/Article/details/gdppntbtn.sHtML

PHP:  public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gvgdetkkq.sHtML

JS:   #private 字段；其余公开
来源：http://blog.zdbjq.cn/Article/details/gcmekjtqx.sHtML

TS:   public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gchazioqt.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.zdbjq.cn/Article/details/gtyjgyljq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.zdbjq.cn/Article/details/gcanwpepn.sHtML

Ruby: public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gbbpjainu.sHtML

C#:   public / protected / private / internal
来源：http://mobile.hesvh.cn/Article/details/gzwnqtekc.sHtML

[G11] getter / setter
来源：http://mobile.fehbvm.com/Article/details/gnwzyhpak.sHtML

Py:   @property 与 @x.setter
来源：http://baike.zdbjq.cn/Article/details/gzmerweca.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gocojhbnf.sHtML

JS:   get name() { return this._name; }
来源：http://wap.fehbvm.com/Article/details/gkcwpmvdf.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.fehbvm.com/Article/details/gasixiehg.sHtML

Java: public String getName() { return name; }
来源：http://3g.fehbvm.com/Article/details/gpgdnodaz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gabcdaifh.sHtML

Ruby: attr_accessor :name
来源：http://baike.zdbjq.cn/Article/details/goxflnbpk.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.fehbvm.com/Article/details/ggnpmxohy.sHtML

[G12] 对象转字符串
来源：http://www.share.hesvh.cn/Article/details/gngatvrzc.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.fehbvm.com/Article/details/guicxgmrt.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gbrkfzigo.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gyvipmbbo.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gajtfqrng.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gqscbzpyd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gmabdawzt.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.hesvh.cn/Article/details/ggnhlxwie.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gsswmndxd.sHtML

[G13] 判断对象类型
来源：http://3g.fehbvm.com/Article/details/gestlhdlf.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fehbvm.com/Article/details/gscdfsgca.sHtML

PHP:  $u instanceof User
来源：http://baike.hesvh.cn/Article/details/gohhfyfhv.sHtML

JS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/glratlbag.sHtML

TS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gaadqgxja.sHtML

Java: u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gghgxmepy.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.fehbvm.com/Article/details/gmikvqakl.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.zdbjq.cn/Article/details/gdkwhjbfy.sHtML

C#:   u is User
来源：http://www.m.share.zdbjq.cn/Article/details/gcfzgpsek.sHtML

[G14] 数据类 / record
来源：http://read.share.hesvh.cn/Article/details/gvskdtaja.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fehbvm.com/Article/details/gfmveytfh.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.fehbvm.com/Article/details/glojfehwo.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.hesvh.cn/Article/details/glwhocedm.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.hesvh.cn/Article/details/grlyczmlv.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.fehbvm.com/Article/details/gsqgvsmhq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.hesvh.cn/Article/details/gawlwpxvq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fehbvm.com/Article/details/gzyztlmmv.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.fehbvm.com/Article/details/gnrwwsuki.sHtML

[G15] 枚举
来源：http://baike.fehbvm.com/Article/details/gtqphbbvb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.hesvh.cn/Article/details/glhkdcesi.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://baike.zdbjq.cn/Article/details/gzdqpfhuj.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.zdbjq.cn/Article/details/gwyshswzt.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gclcxgfxk.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.fehbvm.com/Article/details/gjmhzayck.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.zdbjq.cn/Article/details/gdpcvlylo.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.fehbvm.com/Article/details/gokodatvd.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gbvclwplr.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.zdbjq.cn/Article/details/gqntrzycm.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.zdbjq.cn/Article/details/gtxjuqweh.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.hesvh.cn/Article/details/gzdsgzzkb.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/ghcyfukgm.sHtML

TS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gzemwlduh.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.fehbvm.com/Article/details/gteogmwli.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.zdbjq.cn/Article/details/gkacexsnk.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.fehbvm.com/Article/details/gluazzris.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.zdbjq.cn/Article/details/ggijytvvi.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gtziscieg.sHtML

H. 异常与错误处理
来源：http://m.share.hesvh.cn/Article/details/gypeszsrq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gcgtfyxsf.sHtML

[H01] try / catch 基础
来源：http://www.blog.hesvh.cn/Article/details/grqvsbhny.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.hesvh.cn/Article/details/gwbtljubq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.zdbjq.cn/Article/details/giriotwjo.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gnbpfoyye.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gtkymnvpw.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.hesvh.cn/Article/details/gnkfzxcxy.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.fehbvm.com/Article/details/gqtoabilu.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.fehbvm.com/Article/details/gadvvrpnv.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.hesvh.cn/Article/details/gjouoqmoa.sHtML

[H02] finally / ensure 收尾
来源：http://blog.fehbvm.com/Article/details/ginuwuvlq.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.hesvh.cn/Article/details/gpcvruagb.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gyjmgvnvz.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/goaiukbpp.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gtrjkehlz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gpyxczijq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.hesvh.cn/Article/details/gzkepibja.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.zdbjq.cn/Article/details/gzporwtsx.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/giqawqeca.sHtML

[H03] 主动抛出异常
来源：http://3g.hesvh.cn/Article/details/gkativfnh.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.hesvh.cn/Article/details/gzdtfzpgk.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gkvpxwttt.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.hesvh.cn/Article/details/grysbmrca.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gkyltdkhk.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gxhaunduy.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.zdbjq.cn/Article/details/gruegcmns.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.zdbjq.cn/Article/details/gvmoidkml.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gkbrzrlix.sHtML

[H04] 自定义异常类型
来源：http://mobile.zdbjq.cn/Article/details/ggslnsyvx.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.fehbvm.com/Article/details/gycjboogi.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/gdszevsus.sHtML

JS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/gpigknqxz.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.hesvh.cn/Article/details/geurdbhvg.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/gddmyyzrt.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.fehbvm.com/Article/details/gwefxogcs.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.fehbvm.com/Article/details/gfbbukgbm.sHtML

C#:   class MyException : Exception {}
来源：http://3g.hesvh.cn/Article/details/grrytmhfj.sHtML

[H05] 捕获特定类型
来源：http://m.share.fehbvm.com/Article/details/gyaahqftu.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.hesvh.cn/Article/details/ggwiaybuh.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.fehbvm.com/Article/details/gbolpgoeq.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/gpzyjmyoq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.hesvh.cn/Article/details/govlchjrs.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.zdbjq.cn/Article/details/gnmkzpohz.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.hesvh.cn/Article/details/gyscpwzmr.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.zdbjq.cn/Article/details/gxpoajxxk.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.fehbvm.com/Article/details/gkkuurdpa.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.zdbjq.cn/Article/details/gpshsetfh.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.zdbjq.cn/Article/details/gswtkigpy.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.hesvh.cn/Article/details/gcgxgmfep.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.hesvh.cn/Article/details/gzvtxhyrx.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/gghxegirh.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.hesvh.cn/Article/details/gyketcwzw.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.hesvh.cn/Article/details/gokzydwrk.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.hesvh.cn/Article/details/gyheorspj.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.fehbvm.com/Article/details/gatojjalq.sHtML

[H07] 断言
来源：http://mobile.fehbvm.com/Article/details/gygwxjolh.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.fehbvm.com/Article/details/grtpyjloz.sHtML

PHP:  assert($x > 0);
来源：http://wap.zdbjq.cn/Article/details/gjvbjykuy.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/gbjpyrzfx.sHtML

TS:   console.assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gshiqjcmx.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.zdbjq.cn/Article/details/gnrldfqju.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.fehbvm.com/Article/details/gzborrgxq.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.zdbjq.cn/Article/details/gbqyzrbln.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/glribtajq.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.hesvh.cn/Article/details/guajzhwcr.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.zdbjq.cn/Article/details/gasadejuo.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.fehbvm.com/Article/details/gkpxzzssa.sHtML

JS:   e.message;  e.stack
来源：http://read.share.zdbjq.cn/Article/details/gdrwuqfhr.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.hesvh.cn/Article/details/gomjzaznc.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.zdbjq.cn/Article/details/gkyqkpibd.sHtML

Go:   err.Error()
来源：http://3g.zdbjq.cn/Article/details/gweimmibe.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.fehbvm.com/Article/details/gtkmwxppv.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.zdbjq.cn/Article/details/gunsprdjb.sHtML

[H09] 带错误码的异常
来源：http://www.share.zdbjq.cn/Article/details/gffztiway.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.hesvh.cn/Article/details/glggwupjl.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.hesvh.cn/Article/details/gihqgnzev.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.zdbjq.cn/Article/details/gzbwbomdf.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://m.share.fehbvm.com/Article/details/gilrfcyor.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.zdbjq.cn/Article/details/gklnilgyh.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.fehbvm.com/Article/details/gjiyciktf.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.fehbvm.com/Article/details/gypmqkbqc.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.fehbvm.com/Article/details/glnlroxit.sHtML

[H10] 资源自动释放
来源：http://3g.hesvh.cn/Article/details/gnllsenuy.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.zdbjq.cn/Article/details/gveeyokhy.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.zdbjq.cn/Article/details/gnaamihsi.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fehbvm.com/Article/details/gyayxdiax.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fehbvm.com/Article/details/gnfvzouvi.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.zdbjq.cn/Article/details/gjbtsylzv.sHtML

Go:   defer f.Close()
来源：http://3g.fehbvm.com/Article/details/gdriacmay.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.zdbjq.cn/Article/details/gspvowrwh.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gkluzojsg.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gpjkjdkhy.sHtML

I. 正则表达式
来源：http://blog.fehbvm.com/Article/details/gmlozglbm.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gfistrsbu.sHtML

[I01] 判断是否匹配
来源：http://3g.fehbvm.com/Article/details/ghafgfhyy.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.fehbvm.com/Article/details/gkhkdufwr.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gupwdouat.sHtML

JS:   /\d+/.test(s)
来源：http://baike.fehbvm.com/Article/details/gckobwmua.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.zdbjq.cn/Article/details/gqvogyprn.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.hesvh.cn/Article/details/gnjvheesw.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.hesvh.cn/Article/details/gvccfqrys.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.hesvh.cn/Article/details/gajizkrjo.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.fehbvm.com/Article/details/gmrguehoq.sHtML

[I02] 提取所有匹配
来源：http://blog.hesvh.cn/Article/details/gkysaptye.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.hesvh.cn/Article/details/gtdpivkcx.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.m.share.zdbjq.cn/Article/details/goufhnryr.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.hesvh.cn/Article/details/grbjhyfdw.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.hesvh.cn/Article/details/golspvdpq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.m.share.hesvh.cn/Article/details/guupjrxlq.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.fehbvm.com/Article/details/gqmgwrjka.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.zdbjq.cn/Article/details/gunsmgaga.sHtML


<!-- 参考信息 -->