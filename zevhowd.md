代发 wailian999

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.zdbjq.cn/Article/details/gxiychvqf.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.zdbjq.cn/Article/details/gyzefreza.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.zdbjq.cn/Article/details/gvxtjdpxt.sHtML

[F08] 遍历目录
来源：http://read.share.zdbjq.cn/Article/details/gncuzgeox.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.hesvh.cn/Article/details/gjuodcieb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.hesvh.cn/Article/details/gqmunlyim.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gmzcwdjya.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/gnnltxrjr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gabanipdu.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.zdbjq.cn/Article/details/gjnizigjc.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gkskmzukt.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.fehbvm.com/Article/details/goepkxaca.sHtML

[F09] 获取文件大小
来源：http://blog.hesvh.cn/Article/details/gnqnrhhef.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.hesvh.cn/Article/details/gkzdpypna.sHtML

PHP:  filesize("a.txt");
来源：http://3g.hesvh.cn/Article/details/gvrpoqrnk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gpsnqcpjs.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gbmakbypy.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gcutrhzal.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.hesvh.cn/Article/details/geewrliok.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gvgytsoef.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fehbvm.com/Article/details/gguznoduf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.hesvh.cn/Article/details/gzhjmnfqn.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/grbjophpt.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gcdclgkvi.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gnmsrgvhw.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/guoeixwmq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.hesvh.cn/Article/details/gabejnogu.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gzayudgml.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/getyrqbwv.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gufzweflx.sHtML

[F11] 复制与移动文件
来源：http://baike.hesvh.cn/Article/details/gbtvhlprf.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gnkrihoke.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gwulfwhqu.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/guzveatqs.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gtexmtjgv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.zdbjq.cn/Article/details/gbblxzbxe.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.hesvh.cn/Article/details/ghgcayujm.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/ggpumsmjk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.hesvh.cn/Article/details/gtqmqewsm.sHtML

[F12] CSV 读写
来源：http://m.share.hesvh.cn/Article/details/gvgddcdkp.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.fehbvm.com/Article/details/gmrpzvwjb.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.zdbjq.cn/Article/details/gyehuowtw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.zdbjq.cn/Article/details/gglddwuze.sHtML

TS:   // 同上
来源：http://mobile.hesvh.cn/Article/details/gsprevpor.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.fehbvm.com/Article/details/gwrfqybgs.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.hesvh.cn/Article/details/gdnbbqffy.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fehbvm.com/Article/details/gadawfljv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.hesvh.cn/Article/details/gdmarkqkk.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gaduezepw.sHtML

G. 面向对象
来源：http://mobile.fehbvm.com/Article/details/gtetngddy.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gmycvlmoy.sHtML

[G01] 定义类
来源：http://read.share.hesvh.cn/Article/details/gorzyplzu.sHtML

Py:   class User: pass
来源：http://wap.fehbvm.com/Article/details/gwrgzfeqf.sHtML

PHP:  class User {}
来源：http://read.share.zdbjq.cn/Article/details/gsuzycxfz.sHtML

JS:   class User {}
来源：http://3g.hesvh.cn/Article/details/gwvyocsnf.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.fehbvm.com/Article/details/gjqgsyshi.sHtML

Java: class User {}
来源：http://mobile.fehbvm.com/Article/details/gtwabiboz.sHtML

Go:   type User struct { Name string }
来源：http://m.share.zdbjq.cn/Article/details/gqlaopudm.sHtML

Ruby: class User; end
来源：http://mobile.zdbjq.cn/Article/details/grfsasesx.sHtML

C#:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gozukozid.sHtML

[G02] 构造函数
来源：http://mobile.zdbjq.cn/Article/details/govcubflv.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.hesvh.cn/Article/details/gcwfahjzo.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.fehbvm.com/Article/details/gozactjqr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gxnojscwq.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.zdbjq.cn/Article/details/gltqvbrvn.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/goddazztn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.fehbvm.com/Article/details/gzemqmysc.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fehbvm.com/Article/details/gkkrqkkdk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.fehbvm.com/Article/details/glokqmenx.sHtML

[G03] 实例属性
来源：http://blog.zdbjq.cn/Article/details/gumraqpmg.sHtML

Py:   self.name = "x"
来源：http://wap.zdbjq.cn/Article/details/gibitboov.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gnopvjfmi.sHtML

JS:   this.name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gmdevuqiv.sHtML

TS:   name: string = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gpndthjmi.sHtML

Java: private String name;
来源：http://www.share.hesvh.cn/Article/details/geycwigsy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.zdbjq.cn/Article/details/gxlubatjq.sHtML

Ruby: @name = "x"
来源：http://m.share.zdbjq.cn/Article/details/glsliatqb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fehbvm.com/Article/details/gcpsofbaa.sHtML

[G04] 定义方法
来源：http://blog.hesvh.cn/Article/details/gkjgwanvh.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/gjztjmjkh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gludrhoxz.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gvysoubrr.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gxglejljl.sHtML

Java: String greet() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gxrgdpbok.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gxihgdqwc.sHtML

Ruby: def greet; @name; end
来源：http://read.share.hesvh.cn/Article/details/ghtrcqhhe.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fehbvm.com/Article/details/gerdpqjhy.sHtML

[G05] 继承
来源：http://www.share.fehbvm.com/Article/details/gnusnfhrg.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fehbvm.com/Article/details/gtpoqkemd.sHtML

PHP:  class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gnowtdpht.sHtML

JS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/ghcfaslzg.sHtML

TS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gbgtkzzdl.sHtML

Java: class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/ghshswmon.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.hesvh.cn/Article/details/gkvqyytuu.sHtML

Ruby: class Admin < User; end
来源：http://baike.fehbvm.com/Article/details/ggpdbrbgn.sHtML

C#:   class Admin : User {}
来源：http://www.share.fehbvm.com/Article/details/gutianixm.sHtML

[G06] 重写方法
来源：http://www.m.share.zdbjq.cn/Article/details/ghfukyuxk.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.fehbvm.com/Article/details/glglayzmz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gehfmgxcy.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gwmwtxidv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/grgafbnoi.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gtczptnyk.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.fehbvm.com/Article/details/gbeachuxa.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.zdbjq.cn/Article/details/gssnwepyq.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.zdbjq.cn/Article/details/gmxecnvzx.sHtML

[G07] 调用父类方法
来源：http://blog.hesvh.cn/Article/details/guwvbycvz.sHtML

Py:   super().greet()
来源：http://blog.zdbjq.cn/Article/details/gfwlzpvju.sHtML

PHP:  parent::greet();
来源：http://www.m.share.hesvh.cn/Article/details/ggykrfkrh.sHtML

JS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gqeoczuzv.sHtML

TS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gjjzsglwj.sHtML

Java: super.greet();
来源：http://mobile.fehbvm.com/Article/details/gwtkcqear.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.hesvh.cn/Article/details/gfunlwayu.sHtML

Ruby: super
来源：http://m.share.fehbvm.com/Article/details/gszgyvfvg.sHtML

C#:   base.Greet();
来源：http://www.share.hesvh.cn/Article/details/gvgfkrgkt.sHtML

[G08] 静态方法与属性
来源：http://m.share.zdbjq.cn/Article/details/gofvcavtk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.zdbjq.cn/Article/details/gducjakur.sHtML

PHP:  public static function f() {}
来源：http://wap.hesvh.cn/Article/details/gaaljsjxt.sHtML

JS:   static f() {}
来源：http://www.blog.hesvh.cn/Article/details/gjaixiazz.sHtML

TS:   static f(): void {}
来源：http://baike.zdbjq.cn/Article/details/gylocspes.sHtML

Java: static void f() {}
来源：http://blog.fehbvm.com/Article/details/gwhgbjpll.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.zdbjq.cn/Article/details/gnntaxdyr.sHtML

Ruby: def self.f; end
来源：http://3g.fehbvm.com/Article/details/gxemajubj.sHtML

C#:   public static void F() {}
来源：http://m.share.hesvh.cn/Article/details/gpmehoigt.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.hesvh.cn/Article/details/gxmtdbsyq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.zdbjq.cn/Article/details/glccdzwlb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.hesvh.cn/Article/details/gdjesxajw.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.hesvh.cn/Article/details/gwzckqytq.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.hesvh.cn/Article/details/gqcfbsfuz.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.fehbvm.com/Article/details/gjlejbabh.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.zdbjq.cn/Article/details/ggtlfsgur.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.fehbvm.com/Article/details/gtpvvcjec.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.zdbjq.cn/Article/details/gjwnlreqf.sHtML

[G10] 访问控制
来源：http://baike.fehbvm.com/Article/details/ginjxeckz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.zdbjq.cn/Article/details/gmkxgrccj.sHtML

PHP:  public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gtxvmilkc.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.fehbvm.com/Article/details/ginkmcuei.sHtML

TS:   public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gslsffjyz.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.zdbjq.cn/Article/details/gcvipvuzs.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.zdbjq.cn/Article/details/gfpoxaxnf.sHtML

Ruby: public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gqplfpuys.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.zdbjq.cn/Article/details/gvoordhld.sHtML

[G11] getter / setter
来源：http://baike.fehbvm.com/Article/details/ghokdzhgq.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fehbvm.com/Article/details/gsehpeyqj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gmmafwsqj.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gumgnoiby.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gcuwnvrkb.sHtML

Java: public String getName() { return name; }
来源：http://baike.fehbvm.com/Article/details/gikudzdep.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gcmxwpyro.sHtML

Ruby: attr_accessor :name
来源：http://read.share.zdbjq.cn/Article/details/gihukjhwb.sHtML

C#:   public string Name { get; set; }
来源：http://baike.fehbvm.com/Article/details/ggiwdinyv.sHtML

[G12] 对象转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gdkwcmwco.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.fehbvm.com/Article/details/gdgabbzrp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gkcjwuakb.sHtML

JS:   toString() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gewkzoyyq.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/geuawocxf.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fehbvm.com/Article/details/grnkievfj.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gytdfahna.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fehbvm.com/Article/details/gcbynlmbo.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gvrykogsq.sHtML

[G13] 判断对象类型
来源：http://www.share.zdbjq.cn/Article/details/goqztmapu.sHtML

Py:   isinstance(u, User)
来源：http://baike.hesvh.cn/Article/details/gziqgkkzs.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gzidtgjzi.sHtML

JS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/ggkvzfkil.sHtML

TS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/geawmgqam.sHtML

Java: u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gkkwzlnyc.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.zdbjq.cn/Article/details/gvpjpbqrc.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.hesvh.cn/Article/details/gvffnnels.sHtML

C#:   u is User
来源：http://www.m.share.hesvh.cn/Article/details/gixhsspsh.sHtML

[G14] 数据类 / record
来源：http://m.share.zdbjq.cn/Article/details/gjkyyvysh.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.fehbvm.com/Article/details/gvywbfhst.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.hesvh.cn/Article/details/gcmnyjhbl.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.zdbjq.cn/Article/details/gxfpgmxnd.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.zdbjq.cn/Article/details/gkoouqtub.sHtML

Java: record User(String name, int age) {}
来源：http://blog.hesvh.cn/Article/details/gpnfhkdqd.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.hesvh.cn/Article/details/gfaafwxpt.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.zdbjq.cn/Article/details/gaoovahkg.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.zdbjq.cn/Article/details/gsrxoehte.sHtML

[G15] 枚举
来源：http://www.share.fehbvm.com/Article/details/gnncdlyhg.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.fehbvm.com/Article/details/gtqxwfovg.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.hesvh.cn/Article/details/giutvmfsg.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.hesvh.cn/Article/details/gbyeqxofr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gjdxyxjxo.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.hesvh.cn/Article/details/glediajoy.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.fehbvm.com/Article/details/givekqcpu.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.hesvh.cn/Article/details/gvvsrajbb.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gbpedopmz.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.hesvh.cn/Article/details/gmsxkbbvy.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.hesvh.cn/Article/details/gkggjtvhs.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.zdbjq.cn/Article/details/gkwiwswqj.sHtML

JS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/gevlsicrm.sHtML

TS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/gehfpdujx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.fehbvm.com/Article/details/glrwwhele.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.fehbvm.com/Article/details/gnoklvlrp.sHtML

Ruby: obj.instance_variables
来源：http://m.share.hesvh.cn/Article/details/gnxzlzxbe.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.hesvh.cn/Article/details/gevnsakeo.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gbutiievl.sHtML

H. 异常与错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gtrdwfrws.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gwrsaxqhf.sHtML

[H01] try / catch 基础
来源：http://www.share.hesvh.cn/Article/details/gtmafihbu.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.zdbjq.cn/Article/details/gtgeyqilu.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.fehbvm.com/Article/details/gupwhomqs.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/gwbnmwymq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gkujkcpbf.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.hesvh.cn/Article/details/giccudfor.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.hesvh.cn/Article/details/gzwwphxsq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.hesvh.cn/Article/details/gbfvdquwk.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.hesvh.cn/Article/details/gtcutovok.sHtML

[H02] finally / ensure 收尾
来源：http://baike.zdbjq.cn/Article/details/gohkmhwgp.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.fehbvm.com/Article/details/gqpgjlofq.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gunzsknfe.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gekqkxhww.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gzguxwpcv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/ggesyktil.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.hesvh.cn/Article/details/grtnuvmwn.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.fehbvm.com/Article/details/gebvdeurp.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.hesvh.cn/Article/details/geirbnccm.sHtML

[H03] 主动抛出异常
来源：http://mobile.zdbjq.cn/Article/details/grdthffwu.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.zdbjq.cn/Article/details/gsltmuwux.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gezwxxfsk.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gzpjahlgb.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/grmtvwyqi.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gggsqoyqe.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.hesvh.cn/Article/details/gfviueqlz.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.fehbvm.com/Article/details/gbwjvyhbg.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/guidxuoke.sHtML

[H04] 自定义异常类型
来源：http://wap.zdbjq.cn/Article/details/gbmtfpcuc.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.fehbvm.com/Article/details/gifrwzyfb.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.fehbvm.com/Article/details/gerbxcfzh.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/geagueoca.sHtML

TS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/gvijcyjlf.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/ghdpbgwva.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.fehbvm.com/Article/details/goigixdvx.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.zdbjq.cn/Article/details/gjvvlxonc.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.fehbvm.com/Article/details/guuharecv.sHtML

[H05] 捕获特定类型
来源：http://www.share.fehbvm.com/Article/details/gkynxbyvw.sHtML

Py:   except ValueError as e:
来源：http://3g.hesvh.cn/Article/details/gmucjslph.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.zdbjq.cn/Article/details/gbrnlvcdj.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.hesvh.cn/Article/details/ginnvvama.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/gxunopquh.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.fehbvm.com/Article/details/ghirdmhlm.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.zdbjq.cn/Article/details/gcnhbqaxh.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.hesvh.cn/Article/details/gxduhhwew.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.fehbvm.com/Article/details/gqilwihkx.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.zdbjq.cn/Article/details/gekrydyeb.sHtML

Py:   value = d.get("k") or default
来源：http://blog.zdbjq.cn/Article/details/gotzycpml.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.hesvh.cn/Article/details/glwdzevgk.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.hesvh.cn/Article/details/gbfpbjvwt.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fehbvm.com/Article/details/gtlsbslzw.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.zdbjq.cn/Article/details/gdvjprdno.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.zdbjq.cn/Article/details/gvdribwod.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.fehbvm.com/Article/details/gsqkoswxl.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.hesvh.cn/Article/details/gucqpvlyr.sHtML

[H07] 断言
来源：http://www.blog.zdbjq.cn/Article/details/gwuapevmo.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.fehbvm.com/Article/details/gticnujot.sHtML

PHP:  assert($x > 0);
来源：http://m.share.hesvh.cn/Article/details/gryafmwbv.sHtML

JS:   console.assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gxsphvrxm.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gomouupun.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.hesvh.cn/Article/details/gthmhhwtc.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.zdbjq.cn/Article/details/gfaxdbdht.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.zdbjq.cn/Article/details/gvicinxeq.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gaxlceutw.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.fehbvm.com/Article/details/gmxmwloio.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.hesvh.cn/Article/details/goofzypqw.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.fehbvm.com/Article/details/gjrfwvakb.sHtML

JS:   e.message;  e.stack
来源：http://read.share.zdbjq.cn/Article/details/gjwusjopg.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.zdbjq.cn/Article/details/gpkcowgoi.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.fehbvm.com/Article/details/gprdgtnmi.sHtML

Go:   err.Error()
来源：http://read.share.zdbjq.cn/Article/details/gvdfyunoa.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.zdbjq.cn/Article/details/gttknndre.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.zdbjq.cn/Article/details/gxnkqujpa.sHtML

[H09] 带错误码的异常
来源：http://baike.hesvh.cn/Article/details/grivbfsty.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.fehbvm.com/Article/details/glwkqobwq.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.zdbjq.cn/Article/details/gctcajsax.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.hesvh.cn/Article/details/ggkmbmtnq.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.hesvh.cn/Article/details/ggrdtwlaq.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.blog.zdbjq.cn/Article/details/gpbadkydz.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.fehbvm.com/Article/details/gfaybezyk.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.hesvh.cn/Article/details/gaaubjqam.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.zdbjq.cn/Article/details/gixgxlqko.sHtML

[H10] 资源自动释放
来源：http://www.blog.zdbjq.cn/Article/details/gqlisiysp.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.hesvh.cn/Article/details/gfceusmum.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.zdbjq.cn/Article/details/gupmqfskg.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.zdbjq.cn/Article/details/gjkbvkgca.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.hesvh.cn/Article/details/gyszyhola.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.zdbjq.cn/Article/details/glcsnsgwn.sHtML

Go:   defer f.Close()
来源：http://mobile.zdbjq.cn/Article/details/gfhkrkkhe.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.hesvh.cn/Article/details/gogeupnwl.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gjmddnqob.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/grvlrdeye.sHtML

I. 正则表达式
来源：http://wap.fehbvm.com/Article/details/gkgfgydku.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gnpfcbtbj.sHtML

[I01] 判断是否匹配
来源：http://3g.fehbvm.com/Article/details/gbvaelxel.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.zdbjq.cn/Article/details/gfjcwvtse.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gltafnzfs.sHtML

JS:   /\d+/.test(s)
来源：http://mobile.hesvh.cn/Article/details/guqhjhqel.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.zdbjq.cn/Article/details/gkmqqogjj.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.fehbvm.com/Article/details/gxecziduy.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://baike.zdbjq.cn/Article/details/gtwvwibci.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gxnlvaxvj.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.hesvh.cn/Article/details/gcwajossw.sHtML


<!-- 参考信息 -->