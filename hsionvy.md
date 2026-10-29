代发 wailian999

[F09] 获取文件大小
来源：http://blog.fehbvm.com/Article/details/gxtmncolu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gpdrpwauj.sHtML

PHP:  filesize("a.txt");
来源：http://blog.fehbvm.com/Article/details/ggzuhfjzt.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/gfreupvqe.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/gqbfgstyd.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gjqnrdgio.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.hesvh.cn/Article/details/gaxwmmgyf.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gryndsrgk.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.zdbjq.cn/Article/details/gvhhiebou.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.zdbjq.cn/Article/details/ghtycnrog.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/ghqtnuzxk.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.hesvh.cn/Article/details/ghkcizmvp.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gtmaamups.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gsmvllyye.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fehbvm.com/Article/details/gkhaathcc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gulkacxfb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/ghnhgvyfh.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/ggvkvalkh.sHtML

[F11] 复制与移动文件
来源：http://read.share.fehbvm.com/Article/details/gvdrtjasa.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gekdizvwn.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.zdbjq.cn/Article/details/grdybyqmm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/grghypfpm.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/ghclajnnc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.zdbjq.cn/Article/details/gdkgeohmr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.fehbvm.com/Article/details/gtiqvosds.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gsskqmrbj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.zdbjq.cn/Article/details/gwjpclhne.sHtML

[F12] CSV 读写
来源：http://mobile.fehbvm.com/Article/details/gpnffaqzc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.zdbjq.cn/Article/details/gzdeanlzk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.hesvh.cn/Article/details/gkkhkwpqd.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.hesvh.cn/Article/details/gbejikhvj.sHtML

TS:   // 同上
来源：http://m.share.hesvh.cn/Article/details/gwriydytu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fehbvm.com/Article/details/gwacsdcyy.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.zdbjq.cn/Article/details/gwtpwrdmm.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.zdbjq.cn/Article/details/gagplzrjo.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.hesvh.cn/Article/details/gxhppepsu.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gbojxcplb.sHtML

G. 面向对象
来源：http://baike.fehbvm.com/Article/details/gjqqxsevh.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ghxbymjeu.sHtML

[G01] 定义类
来源：http://3g.zdbjq.cn/Article/details/gewaeyqee.sHtML

Py:   class User: pass
来源：http://www.m.share.zdbjq.cn/Article/details/gmsmduaht.sHtML

PHP:  class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gzycykrno.sHtML

JS:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gjofiboat.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.zdbjq.cn/Article/details/gxilzqbcw.sHtML

Java: class User {}
来源：http://wap.fehbvm.com/Article/details/ghkccbpav.sHtML

Go:   type User struct { Name string }
来源：http://read.share.zdbjq.cn/Article/details/gfarhcnao.sHtML

Ruby: class User; end
来源：http://mobile.fehbvm.com/Article/details/gbppmlsxi.sHtML

C#:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gbtjzsazx.sHtML

[G02] 构造函数
来源：http://www.share.zdbjq.cn/Article/details/gsygkxsxj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.hesvh.cn/Article/details/gahtogejw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.zdbjq.cn/Article/details/genotmllt.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/gmqsxlgnp.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/gdfgsrzrw.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/giiqwhhji.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.zdbjq.cn/Article/details/gwvekfbda.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.zdbjq.cn/Article/details/gmwcjatbm.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.fehbvm.com/Article/details/ghuokfndf.sHtML

[G03] 实例属性
来源：http://mobile.hesvh.cn/Article/details/gryyqrgdo.sHtML

Py:   self.name = "x"
来源：http://wap.zdbjq.cn/Article/details/gfbqitpgd.sHtML

PHP:  public string $name = "x";
来源：http://blog.hesvh.cn/Article/details/gezewolrc.sHtML

JS:   this.name = "x";
来源：http://wap.hesvh.cn/Article/details/gplppxkib.sHtML

TS:   name: string = "x";
来源：http://www.blog.fehbvm.com/Article/details/gklifzemy.sHtML

Java: private String name;
来源：http://www.blog.zdbjq.cn/Article/details/gyefiyuhq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.zdbjq.cn/Article/details/gfthnoppu.sHtML

Ruby: @name = "x"
来源：http://read.share.fehbvm.com/Article/details/gwyqifvkr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.hesvh.cn/Article/details/gaxbkbuft.sHtML

[G04] 定义方法
来源：http://www.m.share.zdbjq.cn/Article/details/gnasyyzlk.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/geerhcsnh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gmjhdcche.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/guaowsfyi.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gkbkrypeq.sHtML

Java: String greet() { return name; }
来源：http://wap.zdbjq.cn/Article/details/ggcpnneow.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gtaihugpx.sHtML

Ruby: def greet; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gavsufbne.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/ghkfgrold.sHtML

[G05] 继承
来源：http://www.m.share.zdbjq.cn/Article/details/gepgdkxec.sHtML

Py:   class Admin(User): pass
来源：http://mobile.fehbvm.com/Article/details/gzrmvbuuh.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gncapnpcl.sHtML

JS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gmeizudqb.sHtML

TS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/ggzobkfdo.sHtML

Java: class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gkdythglf.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.fehbvm.com/Article/details/gafswlqui.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.fehbvm.com/Article/details/gxfqalheh.sHtML

C#:   class Admin : User {}
来源：http://wap.hesvh.cn/Article/details/gpjguwiqb.sHtML

[G06] 重写方法
来源：http://read.share.fehbvm.com/Article/details/gghcxnaxf.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fehbvm.com/Article/details/ghxwxeqaa.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gjlwalyvg.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnwvgpgtf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gqrhwjajl.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gjmznxnog.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.hesvh.cn/Article/details/ggfvukfwe.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.fehbvm.com/Article/details/gofkodkis.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.hesvh.cn/Article/details/gctnftlcd.sHtML

[G07] 调用父类方法
来源：http://www.blog.fehbvm.com/Article/details/gmnzzspmo.sHtML

Py:   super().greet()
来源：http://blog.hesvh.cn/Article/details/gbwmjitgi.sHtML

PHP:  parent::greet();
来源：http://blog.fehbvm.com/Article/details/gzzukujpe.sHtML

JS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gzzdcxivh.sHtML

TS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gpoorxymk.sHtML

Java: super.greet();
来源：http://wap.hesvh.cn/Article/details/gnirdbevi.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.zdbjq.cn/Article/details/ghgudonbw.sHtML

Ruby: super
来源：http://www.m.share.hesvh.cn/Article/details/gvrbhsofx.sHtML

C#:   base.Greet();
来源：http://3g.zdbjq.cn/Article/details/gvvlbjjmq.sHtML

[G08] 静态方法与属性
来源：http://www.blog.hesvh.cn/Article/details/gjhuitwzy.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.hesvh.cn/Article/details/gdhiupqki.sHtML

PHP:  public static function f() {}
来源：http://mobile.hesvh.cn/Article/details/ggyffaudr.sHtML

JS:   static f() {}
来源：http://www.share.zdbjq.cn/Article/details/glnptowbl.sHtML

TS:   static f(): void {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbtpxdnrh.sHtML

Java: static void f() {}
来源：http://www.share.fehbvm.com/Article/details/gzbzrtwyt.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.fehbvm.com/Article/details/gprskdwsb.sHtML

Ruby: def self.f; end
来源：http://www.m.share.fehbvm.com/Article/details/gldycmjwj.sHtML

C#:   public static void F() {}
来源：http://www.blog.hesvh.cn/Article/details/gqxuelqmv.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.zdbjq.cn/Article/details/glwbcxjmy.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/gdimsowmb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.hesvh.cn/Article/details/gbrxjauxi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.fehbvm.com/Article/details/godgimyce.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.zdbjq.cn/Article/details/gdkhsokoh.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gzwhmajvf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.fehbvm.com/Article/details/gajbklwic.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.fehbvm.com/Article/details/gjncapoxz.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.hesvh.cn/Article/details/glasqbxcw.sHtML

[G10] 访问控制
来源：http://mobile.hesvh.cn/Article/details/gvbvkdwrr.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.zdbjq.cn/Article/details/gznhxdayn.sHtML

PHP:  public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gypqlcmts.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.zdbjq.cn/Article/details/gpmsmxnpt.sHtML

TS:   public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gmsdtuolm.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fehbvm.com/Article/details/guhysmlrh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.zdbjq.cn/Article/details/glxsuhans.sHtML

Ruby: public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gmghhsltf.sHtML

C#:   public / protected / private / internal
来源：http://m.share.hesvh.cn/Article/details/gohlnnlsf.sHtML

[G11] getter / setter
来源：http://www.blog.zdbjq.cn/Article/details/gajumbckd.sHtML

Py:   @property 与 @x.setter
来源：http://wap.fehbvm.com/Article/details/gvamliizl.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/ggdlfzqzy.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/gxqsicuch.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.fehbvm.com/Article/details/glojncbqs.sHtML

Java: public String getName() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gbnjbangi.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gqnvqxzfv.sHtML

Ruby: attr_accessor :name
来源：http://mobile.zdbjq.cn/Article/details/giotgnboe.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.hesvh.cn/Article/details/garhacyml.sHtML

[G12] 对象转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gyprvbcdq.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gxrnqazsh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gwbwesltp.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gppykoohp.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkwayiffw.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.hesvh.cn/Article/details/ggibzkrtq.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gcuijcehv.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fehbvm.com/Article/details/gwwcaqygh.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.fehbvm.com/Article/details/gklziwltw.sHtML

[G13] 判断对象类型
来源：http://m.share.zdbjq.cn/Article/details/gtfxwdkre.sHtML

Py:   isinstance(u, User)
来源：http://baike.hesvh.cn/Article/details/gyqughaxi.sHtML

PHP:  $u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gjmbzaqej.sHtML

JS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/gljafytwo.sHtML

TS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gvdjvyyth.sHtML

Java: u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gpgowmvnf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.fehbvm.com/Article/details/ggonwloek.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.fehbvm.com/Article/details/ggxyhuokm.sHtML

C#:   u is User
来源：http://mobile.fehbvm.com/Article/details/gyxgzwdhj.sHtML

[G14] 数据类 / record
来源：http://wap.zdbjq.cn/Article/details/guybpgzog.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.zdbjq.cn/Article/details/gpzbrvmxo.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.zdbjq.cn/Article/details/gijpzvvod.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.hesvh.cn/Article/details/gewdlxvqa.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.hesvh.cn/Article/details/gbmccbniy.sHtML

Java: record User(String name, int age) {}
来源：http://3g.zdbjq.cn/Article/details/gxqmiiold.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.zdbjq.cn/Article/details/grsroagma.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.hesvh.cn/Article/details/gguzndihn.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.fehbvm.com/Article/details/glastngjh.sHtML

[G15] 枚举
来源：http://www.share.fehbvm.com/Article/details/gxfbhuewj.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.zdbjq.cn/Article/details/gjtbyowcs.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.hesvh.cn/Article/details/gqchcweer.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.fehbvm.com/Article/details/gvddwomji.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gyhnxxqmo.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.hesvh.cn/Article/details/gvubuzwly.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.hesvh.cn/Article/details/goqanqxrs.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.zdbjq.cn/Article/details/ghyigvolv.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/ghyjxocgn.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.fehbvm.com/Article/details/gmqvwzuep.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.fehbvm.com/Article/details/gkjosstzu.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.zdbjq.cn/Article/details/gpykwtgit.sHtML

JS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/gevqcakyl.sHtML

TS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/ggquixxef.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.hesvh.cn/Article/details/gdvblkgpo.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.hesvh.cn/Article/details/gflppgbri.sHtML

Ruby: obj.instance_variables
来源：http://wap.zdbjq.cn/Article/details/gizesfjtb.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/gdyvyiozx.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gizglvtay.sHtML

H. 异常与错误处理
来源：http://wap.hesvh.cn/Article/details/gagseafdo.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gnrkmzgjd.sHtML

[H01] try / catch 基础
来源：http://www.share.hesvh.cn/Article/details/gqrzavkbp.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.hesvh.cn/Article/details/gvuolbzjo.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.fehbvm.com/Article/details/gqktauwcb.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gekxbzxsc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/ghrwjmegs.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.hesvh.cn/Article/details/gqshrftdg.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.fehbvm.com/Article/details/gflqralbw.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.fehbvm.com/Article/details/geblkalrk.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.hesvh.cn/Article/details/gwxtnvagh.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.zdbjq.cn/Article/details/gpxbwecwf.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.hesvh.cn/Article/details/gpypwupzu.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gqlxcumwf.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/guhfnxazf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gpmccbzfh.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/geevbqjpi.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.zdbjq.cn/Article/details/gyzwpopta.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.hesvh.cn/Article/details/gsldohbkx.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gjyvxdqqy.sHtML

[H03] 主动抛出异常
来源：http://3g.hesvh.cn/Article/details/gaqqiqugv.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.zdbjq.cn/Article/details/guvjhckzg.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/glccwvepp.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gtnjyzzon.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/ggpmzlkxf.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gzesoaljl.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.zdbjq.cn/Article/details/gysrvqnmv.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.fehbvm.com/Article/details/gepzusqio.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gezslunun.sHtML

[H04] 自定义异常类型
来源：http://3g.hesvh.cn/Article/details/gakjvuexe.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.hesvh.cn/Article/details/geuxcjwxl.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.zdbjq.cn/Article/details/gvmcjsqyu.sHtML

JS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/gvlahtvuf.sHtML

TS:   class MyError extends Error {}
来源：http://blog.hesvh.cn/Article/details/grfbguxup.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/gutwjrlas.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.fehbvm.com/Article/details/gtrtfamqt.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.hesvh.cn/Article/details/gogouxeff.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.hesvh.cn/Article/details/goznjlpbl.sHtML

[H05] 捕获特定类型
来源：http://m.share.zdbjq.cn/Article/details/gkcpruxoc.sHtML

Py:   except ValueError as e:
来源：http://read.share.fehbvm.com/Article/details/gtzdrtdsu.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.fehbvm.com/Article/details/gcifzeuej.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/gszmowirf.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/grfaedirs.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.hesvh.cn/Article/details/gxnydbxlg.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.zdbjq.cn/Article/details/gxzzxvyfd.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.fehbvm.com/Article/details/gftvukxfb.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.zdbjq.cn/Article/details/gyreuulcm.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.zdbjq.cn/Article/details/gqlglouhn.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.hesvh.cn/Article/details/gnreyqxrj.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.fehbvm.com/Article/details/gcolwjifn.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/gscmphxxw.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/gvokyzzpb.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.fehbvm.com/Article/details/govigpchm.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.zdbjq.cn/Article/details/gvyiczfge.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.fehbvm.com/Article/details/gqauaxinv.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.fehbvm.com/Article/details/gtbsyktha.sHtML

[H07] 断言
来源：http://wap.fehbvm.com/Article/details/gsqyukapm.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.zdbjq.cn/Article/details/gufenfxwv.sHtML

PHP:  assert($x > 0);
来源：http://blog.hesvh.cn/Article/details/gnqlomomb.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gezkviotp.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/guwkkmoyi.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.hesvh.cn/Article/details/gahorecdo.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.zdbjq.cn/Article/details/giomgxfbd.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.fehbvm.com/Article/details/gqfowihiw.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/gzjgdweyy.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.zdbjq.cn/Article/details/gkmbjduwr.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.fehbvm.com/Article/details/gmpdwofrb.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.fehbvm.com/Article/details/gsieoakvh.sHtML

JS:   e.message;  e.stack
来源：http://wap.zdbjq.cn/Article/details/gimkmhjnm.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.zdbjq.cn/Article/details/gldxweoas.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.fehbvm.com/Article/details/gmwdbysby.sHtML

Go:   err.Error()
来源：http://baike.hesvh.cn/Article/details/gsngrfaff.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.zdbjq.cn/Article/details/ginoctkkq.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.zdbjq.cn/Article/details/gblhstwpz.sHtML

[H09] 带错误码的异常
来源：http://3g.hesvh.cn/Article/details/grktrlxbi.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.zdbjq.cn/Article/details/gnozwoqbc.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.hesvh.cn/Article/details/grxjhhgif.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.zdbjq.cn/Article/details/gszqngmzn.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.hesvh.cn/Article/details/gaeuyzmuo.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://blog.fehbvm.com/Article/details/gzejyfpvd.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.hesvh.cn/Article/details/gjsawwmmw.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.fehbvm.com/Article/details/gwguivkvo.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.zdbjq.cn/Article/details/glfytursm.sHtML

[H10] 资源自动释放
来源：http://www.blog.hesvh.cn/Article/details/gvgjcbjnn.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.zdbjq.cn/Article/details/guvdluoea.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.hesvh.cn/Article/details/gppbkfyep.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.hesvh.cn/Article/details/gscfxetfg.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.fehbvm.com/Article/details/gomgnusqx.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://blog.fehbvm.com/Article/details/gqjawhmxf.sHtML

Go:   defer f.Close()
来源：http://baike.zdbjq.cn/Article/details/ghhohflzp.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.zdbjq.cn/Article/details/glevrnuzh.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gaksxcmhb.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gdlplwlly.sHtML

I. 正则表达式
来源：http://www.m.share.hesvh.cn/Article/details/gtoexuebi.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gefoelkoj.sHtML

[I01] 判断是否匹配
来源：http://mobile.fehbvm.com/Article/details/gbuhkyvuw.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.hesvh.cn/Article/details/ghopisvrp.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.fehbvm.com/Article/details/ggiedwgoq.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.fehbvm.com/Article/details/gfmxseofm.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.hesvh.cn/Article/details/gfcaiqoub.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.hesvh.cn/Article/details/gmcgdabjy.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.hesvh.cn/Article/details/grhsngqaj.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.fehbvm.com/Article/details/gqivnapmk.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://baike.hesvh.cn/Article/details/geqxdvccf.sHtML

[I02] 提取所有匹配
来源：http://mobile.zdbjq.cn/Article/details/ghwmahhgs.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.zdbjq.cn/Article/details/gzmoxxfnh.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.fehbvm.com/Article/details/grkmvfbnr.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.zdbjq.cn/Article/details/gpfoglsyv.sHtML

TS:   s.match(/\d+/g)
来源：http://blog.hesvh.cn/Article/details/giyiavuur.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://m.share.zdbjq.cn/Article/details/gywrwjbsn.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.zdbjq.cn/Article/details/gohyphxat.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.zdbjq.cn/Article/details/gfftnjskm.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.hesvh.cn/Article/details/gnbiqsigm.sHtML

[I03] 提取捕获分组
来源：http://wap.fehbvm.com/Article/details/gqzslzxzu.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gckuwpcpp.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.fehbvm.com/Article/details/gowacsssf.sHtML


<!-- 参考信息 -->