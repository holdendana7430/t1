代发 wailian999

[F09] 获取文件大小
来源：http://www.share.hesvh.cn/Article/details/gtothkcdl.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.fehbvm.com/Article/details/gkwksfnlt.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gyrwvxnql.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/ghxhkeifw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gdyoixeea.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gpbkqjxrg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.fehbvm.com/Article/details/gbmvcqobd.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fehbvm.com/Article/details/glznkydwq.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.zdbjq.cn/Article/details/gwxkumffg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fehbvm.com/Article/details/gpeeppiqi.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gjfspaerf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.hesvh.cn/Article/details/gegktmsoi.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gtxozgsji.sHtML

TS:   path.extname("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gxjqkvfcf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.zdbjq.cn/Article/details/gsvdvmewm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gaddutixi.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gvflnfgpe.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gzlwgvpko.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.hesvh.cn/Article/details/ghnflcgnr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gplyjvmzc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.zdbjq.cn/Article/details/grlcsynwz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gnxuusewt.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gpijwhrmw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gjadffhbw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.hesvh.cn/Article/details/gntiyztfb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gboxjwqgt.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.hesvh.cn/Article/details/gkfifzbjq.sHtML

[F12] CSV 读写
来源：http://baike.zdbjq.cn/Article/details/gsczshnhe.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.hesvh.cn/Article/details/glkknpriw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.hesvh.cn/Article/details/gggbfnrhf.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.zdbjq.cn/Article/details/gkuihahcl.sHtML

TS:   // 同上
来源：http://baike.hesvh.cn/Article/details/glcwsogyu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fehbvm.com/Article/details/gfwotrstl.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.hesvh.cn/Article/details/gimjoftrs.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.hesvh.cn/Article/details/gizebbzcf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fehbvm.com/Article/details/gsxbjnxvt.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gkbfuvuqd.sHtML

G. 面向对象
来源：http://www.blog.fehbvm.com/Article/details/gchwxdlmz.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gfffzvkru.sHtML

[G01] 定义类
来源：http://www.share.zdbjq.cn/Article/details/gakrmptbi.sHtML

Py:   class User: pass
来源：http://baike.hesvh.cn/Article/details/gqsohzvua.sHtML

PHP:  class User {}
来源：http://mobile.hesvh.cn/Article/details/gwkysnqnq.sHtML

JS:   class User {}
来源：http://www.share.hesvh.cn/Article/details/grzecvjft.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.zdbjq.cn/Article/details/gqpcmulea.sHtML

Java: class User {}
来源：http://baike.hesvh.cn/Article/details/ghhjksuue.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.hesvh.cn/Article/details/gprftnkwb.sHtML

Ruby: class User; end
来源：http://wap.fehbvm.com/Article/details/gpqpvmbfc.sHtML

C#:   class User {}
来源：http://baike.hesvh.cn/Article/details/gqxedynlm.sHtML

[G02] 构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gzovzldsa.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fehbvm.com/Article/details/goysngeoj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gydrnlkzo.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gmfbynwjv.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.hesvh.cn/Article/details/gtzyjyltp.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/grapuigbl.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fehbvm.com/Article/details/gywckmrux.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.fehbvm.com/Article/details/gtwgojkjp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gyqnkyaqf.sHtML

[G03] 实例属性
来源：http://www.blog.hesvh.cn/Article/details/gkufcyebl.sHtML

Py:   self.name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/glmjjwwvk.sHtML

PHP:  public string $name = "x";
来源：http://m.share.zdbjq.cn/Article/details/ghlnhnnbc.sHtML

JS:   this.name = "x";
来源：http://read.share.hesvh.cn/Article/details/giougllpj.sHtML

TS:   name: string = "x";
来源：http://mobile.fehbvm.com/Article/details/gjrivbhad.sHtML

Java: private String name;
来源：http://m.share.fehbvm.com/Article/details/goqycbsmx.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.hesvh.cn/Article/details/ghieqwgcg.sHtML

Ruby: @name = "x"
来源：http://m.share.fehbvm.com/Article/details/gqwniojdu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.zdbjq.cn/Article/details/gknkiwpky.sHtML

[G04] 定义方法
来源：http://blog.zdbjq.cn/Article/details/ggqaumxgw.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gaucajwtf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gvuzyodsa.sHtML

JS:   greet() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gkcdaomtl.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gqbkdczkk.sHtML

Java: String greet() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gwfcpzivn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gtpgwagqe.sHtML

Ruby: def greet; @name; end
来源：http://blog.zdbjq.cn/Article/details/guaepzctj.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.fehbvm.com/Article/details/gyevlgfih.sHtML

[G05] 继承
来源：http://www.share.fehbvm.com/Article/details/gspqxqcse.sHtML

Py:   class Admin(User): pass
来源：http://mobile.zdbjq.cn/Article/details/goacnljjw.sHtML

PHP:  class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gpiqhputk.sHtML

JS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gxjhtvmko.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gvpqblexl.sHtML

Java: class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gelacjjyl.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.hesvh.cn/Article/details/gegdvbleu.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.zdbjq.cn/Article/details/gbnilcewj.sHtML

C#:   class Admin : User {}
来源：http://baike.fehbvm.com/Article/details/gjlmefnoc.sHtML

[G06] 重写方法
来源：http://baike.zdbjq.cn/Article/details/gqjovmsgd.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.zdbjq.cn/Article/details/giaudcbyq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gdwhhminw.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gqzwbyoda.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gwyylxpbv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/grxczuzql.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.hesvh.cn/Article/details/gejrmkbsd.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.hesvh.cn/Article/details/gltmlpvyl.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.hesvh.cn/Article/details/gtmbkgfrg.sHtML

[G07] 调用父类方法
来源：http://www.m.share.zdbjq.cn/Article/details/gpjqehpdb.sHtML

Py:   super().greet()
来源：http://blog.fehbvm.com/Article/details/gwgtkbwyf.sHtML

PHP:  parent::greet();
来源：http://wap.fehbvm.com/Article/details/ggefweudd.sHtML

JS:   super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gpmwbgdgi.sHtML

TS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/gbxzhoitt.sHtML

Java: super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/guhoelljk.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.zdbjq.cn/Article/details/gqnmllbjm.sHtML

Ruby: super
来源：http://wap.zdbjq.cn/Article/details/gabfubxkc.sHtML

C#:   base.Greet();
来源：http://m.share.zdbjq.cn/Article/details/glodmdwmo.sHtML

[G08] 静态方法与属性
来源：http://www.share.fehbvm.com/Article/details/gefrstocg.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.fehbvm.com/Article/details/ggnsgbmyj.sHtML

PHP:  public static function f() {}
来源：http://mobile.fehbvm.com/Article/details/gqcrlzmjn.sHtML

JS:   static f() {}
来源：http://3g.zdbjq.cn/Article/details/glsbqrvsk.sHtML

TS:   static f(): void {}
来源：http://www.blog.zdbjq.cn/Article/details/geshchrer.sHtML

Java: static void f() {}
来源：http://3g.hesvh.cn/Article/details/ggwbecehz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.hesvh.cn/Article/details/gbrrfyhit.sHtML

Ruby: def self.f; end
来源：http://3g.fehbvm.com/Article/details/gtdbohahw.sHtML

C#:   public static void F() {}
来源：http://3g.zdbjq.cn/Article/details/giipkvpht.sHtML

[G09] 接口 / 抽象类
来源：http://3g.fehbvm.com/Article/details/gaithcydn.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.hesvh.cn/Article/details/gpczaglqy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.fehbvm.com/Article/details/gwbowdadu.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.hesvh.cn/Article/details/gvoozuqus.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.fehbvm.com/Article/details/goqijklhi.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.zdbjq.cn/Article/details/gpgjmylwj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.zdbjq.cn/Article/details/gxztahxqd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fehbvm.com/Article/details/gofhgxwor.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.fehbvm.com/Article/details/glorvumob.sHtML

[G10] 访问控制
来源：http://www.blog.zdbjq.cn/Article/details/gabcshhej.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.hesvh.cn/Article/details/gpeubtoin.sHtML

PHP:  public / protected / private
来源：http://baike.hesvh.cn/Article/details/gtfsujofx.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.hesvh.cn/Article/details/gpdgytsej.sHtML

TS:   public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gymmkhzum.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.hesvh.cn/Article/details/gehuudmqp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.hesvh.cn/Article/details/ghqmacvle.sHtML

Ruby: public / protected / private
来源：http://blog.zdbjq.cn/Article/details/giiexqqsr.sHtML

C#:   public / protected / private / internal
来源：http://read.share.zdbjq.cn/Article/details/ghvvhipxi.sHtML

[G11] getter / setter
来源：http://read.share.hesvh.cn/Article/details/gklrknhcb.sHtML

Py:   @property 与 @x.setter
来源：http://baike.fehbvm.com/Article/details/gigghlinp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gqkdaabrn.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gcrblebgn.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/gesuftgme.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gedjomvyy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gpbayzbhw.sHtML

Ruby: attr_accessor :name
来源：http://3g.hesvh.cn/Article/details/gqxvvusdp.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.fehbvm.com/Article/details/gymnfxkjx.sHtML

[G12] 对象转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gxipkyfln.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gsztussos.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/guxzvcqpz.sHtML

JS:   toString() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gaftzfqkk.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gkcmlpjtk.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gohatytwe.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/guiqxhuti.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.zdbjq.cn/Article/details/ganhgqsrr.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.zdbjq.cn/Article/details/gbhcesgrb.sHtML

[G13] 判断对象类型
来源：http://read.share.hesvh.cn/Article/details/gcmuqaqrq.sHtML

Py:   isinstance(u, User)
来源：http://blog.fehbvm.com/Article/details/gzzdrundz.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gtsompsgv.sHtML

JS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gdqqsefie.sHtML

TS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gmsqozhli.sHtML

Java: u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gwgrpujcy.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.fehbvm.com/Article/details/gzftcmezp.sHtML

Ruby: u.is_a?(User)
来源：http://3g.fehbvm.com/Article/details/gpwhzvnjd.sHtML

C#:   u is User
来源：http://www.m.share.zdbjq.cn/Article/details/gvpukicln.sHtML

[G14] 数据类 / record
来源：http://mobile.fehbvm.com/Article/details/gpyrznprl.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.hesvh.cn/Article/details/guianqwte.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.fehbvm.com/Article/details/gmetfumwb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.fehbvm.com/Article/details/gdpkdrcrf.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.zdbjq.cn/Article/details/gtgghwauq.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.zdbjq.cn/Article/details/gddfzmhmz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.hesvh.cn/Article/details/gksnmhwbl.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.hesvh.cn/Article/details/gtzdenuga.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.hesvh.cn/Article/details/gfugwvtjw.sHtML

[G15] 枚举
来源：http://wap.hesvh.cn/Article/details/gctknenmo.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.zdbjq.cn/Article/details/gfduaqxug.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.hesvh.cn/Article/details/gcwrtwiei.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.hesvh.cn/Article/details/gjdvtvdrc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gxcrdghqh.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.hesvh.cn/Article/details/gxejdeaag.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.fehbvm.com/Article/details/glyatnzri.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.hesvh.cn/Article/details/gwgxosnlg.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/gchrvozvs.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.hesvh.cn/Article/details/gmwxlfczn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.fehbvm.com/Article/details/gbfkmvcfm.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.zdbjq.cn/Article/details/gpowznark.sHtML

JS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/ghryvvvvz.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/gxydvrmnp.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.hesvh.cn/Article/details/gwxnojvvk.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.hesvh.cn/Article/details/gaeqhbviy.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.hesvh.cn/Article/details/gqnrklaux.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.hesvh.cn/Article/details/gbqysnwud.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gfwdjlres.sHtML

H. 异常与错误处理
来源：http://read.share.zdbjq.cn/Article/details/gfqsnkpdm.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gpmubqesl.sHtML

[H01] try / catch 基础
来源：http://www.m.share.fehbvm.com/Article/details/gwkmzwnui.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.zdbjq.cn/Article/details/gikqbcndi.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.zdbjq.cn/Article/details/gckhaimzq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gvtszdsni.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gwgnmtpju.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.hesvh.cn/Article/details/gvmmowcmp.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.zdbjq.cn/Article/details/gncbvwvdb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.fehbvm.com/Article/details/goijnjqiu.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.zdbjq.cn/Article/details/gbrxkqowv.sHtML

[H02] finally / ensure 收尾
来源：http://blog.fehbvm.com/Article/details/gndxuqoog.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.hesvh.cn/Article/details/grazbiizb.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gejlvxmfi.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gtkjuwjfg.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gkynzikfi.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gjoocuaou.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fehbvm.com/Article/details/gfazedudw.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.fehbvm.com/Article/details/gfwqfqovl.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.hesvh.cn/Article/details/giatwxxfx.sHtML

[H03] 主动抛出异常
来源：http://blog.fehbvm.com/Article/details/gncyqsvcq.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.fehbvm.com/Article/details/gfgleyvbl.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/guiejspfl.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gxgvycnht.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/gbyaiqrkz.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/ggytzdyen.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.hesvh.cn/Article/details/ghrruankj.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.zdbjq.cn/Article/details/gioneampm.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gccdizcie.sHtML

[H04] 自定义异常类型
来源：http://m.share.fehbvm.com/Article/details/gbhrbsfjp.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.zdbjq.cn/Article/details/gjiqouyiq.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/gnwdhluic.sHtML

JS:   class MyError extends Error {}
来源：http://blog.hesvh.cn/Article/details/gmafwlhgt.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.hesvh.cn/Article/details/gubgeiujc.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/gojdbokjp.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.hesvh.cn/Article/details/gpiyjcuxi.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.fehbvm.com/Article/details/gsfkdjilu.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.hesvh.cn/Article/details/gyixrewkj.sHtML

[H05] 捕获特定类型
来源：http://read.share.hesvh.cn/Article/details/goqsqouse.sHtML

Py:   except ValueError as e:
来源：http://baike.fehbvm.com/Article/details/gkxtwukes.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.zdbjq.cn/Article/details/gqyybvnuf.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/glkvgqqjw.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/gvpiemdnn.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.zdbjq.cn/Article/details/gohuohyxu.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.zdbjq.cn/Article/details/gxxmskdqw.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.zdbjq.cn/Article/details/gzuhzpjdz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.fehbvm.com/Article/details/gdqmgiums.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.fehbvm.com/Article/details/gnaoiytqr.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.hesvh.cn/Article/details/gvjoycwwd.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/ggrullbpz.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.hesvh.cn/Article/details/giehphvtt.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.hesvh.cn/Article/details/gqktpiguu.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.zdbjq.cn/Article/details/gxuucvzmc.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.zdbjq.cn/Article/details/gxkopylzp.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.fehbvm.com/Article/details/gpotxouyd.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.hesvh.cn/Article/details/gptywpvfh.sHtML

[H07] 断言
来源：http://3g.fehbvm.com/Article/details/gratqgarh.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.zdbjq.cn/Article/details/gjsfzfhac.sHtML

PHP:  assert($x > 0);
来源：http://www.share.zdbjq.cn/Article/details/ggtwmevct.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gjmiemohk.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/gysewmjzw.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.zdbjq.cn/Article/details/gqvlpdyvo.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.zdbjq.cn/Article/details/ggzfhpkoh.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.fehbvm.com/Article/details/gvauyhjqm.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/grauhlmnc.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.zdbjq.cn/Article/details/gldcykuhx.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.hesvh.cn/Article/details/gslmqkvjb.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.fehbvm.com/Article/details/gqzdxaxwi.sHtML

JS:   e.message;  e.stack
来源：http://blog.hesvh.cn/Article/details/ghlddhxvx.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.zdbjq.cn/Article/details/gukpdkjaz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.fehbvm.com/Article/details/gmjulwouq.sHtML

Go:   err.Error()
来源：http://m.share.fehbvm.com/Article/details/ghjhkjbvq.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.zdbjq.cn/Article/details/ghpwqwgxa.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.zdbjq.cn/Article/details/gtacagkbl.sHtML

[H09] 带错误码的异常
来源：http://m.share.hesvh.cn/Article/details/gzmzukdam.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.fehbvm.com/Article/details/gdzamqovv.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.zdbjq.cn/Article/details/gqybcrmwa.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.fehbvm.com/Article/details/gpizikbrn.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.hesvh.cn/Article/details/gzdrggbqu.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.fehbvm.com/Article/details/geszgihjf.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.hesvh.cn/Article/details/gcydswpdf.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.hesvh.cn/Article/details/gcaavyzow.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://mobile.hesvh.cn/Article/details/gztrlycnk.sHtML

[H10] 资源自动释放
来源：http://wap.fehbvm.com/Article/details/gibirlfml.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://wap.fehbvm.com/Article/details/golxrjeij.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://baike.fehbvm.com/Article/details/gyycleluh.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.hesvh.cn/Article/details/gpedsgtzg.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.zdbjq.cn/Article/details/gekwivtbj.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.zdbjq.cn/Article/details/gsbigyezs.sHtML

Go:   defer f.Close()
来源：http://read.share.zdbjq.cn/Article/details/gyqxihesg.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.zdbjq.cn/Article/details/gboussxqs.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gzjnjaipk.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gugjilgjv.sHtML

I. 正则表达式
来源：http://m.share.fehbvm.com/Article/details/gdqtakzck.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ghewdxgfe.sHtML

[I01] 判断是否匹配
来源：http://read.share.hesvh.cn/Article/details/gvkbidyar.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://wap.hesvh.cn/Article/details/gtfiiymtw.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.hesvh.cn/Article/details/gfsiisubl.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.zdbjq.cn/Article/details/goxeonsin.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.zdbjq.cn/Article/details/gvbnysfuw.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.zdbjq.cn/Article/details/gizvazibd.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.zdbjq.cn/Article/details/gponjbfvg.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.blog.zdbjq.cn/Article/details/gleatbnok.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.hesvh.cn/Article/details/gcrfqwgou.sHtML

[I02] 提取所有匹配
来源：http://mobile.fehbvm.com/Article/details/gjfchuhtn.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.fehbvm.com/Article/details/gdipufdev.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.hesvh.cn/Article/details/gzvaceakr.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.hesvh.cn/Article/details/gsulfuttt.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.fehbvm.com/Article/details/gdshxlzxt.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.fehbvm.com/Article/details/gkoyvjpru.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.zdbjq.cn/Article/details/gewmvmeka.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.hesvh.cn/Article/details/gpxiumssx.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.hesvh.cn/Article/details/gplmullam.sHtML

[I03] 提取捕获分组
来源：http://m.share.hesvh.cn/Article/details/gstnjdwwp.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://m.share.fehbvm.com/Article/details/gepwvuzvj.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.zdbjq.cn/Article/details/guiuczvro.sHtML


<!-- 参考信息 -->