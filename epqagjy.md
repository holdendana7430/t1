代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/gktzcaurz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/ghlyjqety.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.zdbjq.cn/Article/details/gkswhktpm.sHtML

Ruby: File.size("a.txt")
来源：http://wap.hesvh.cn/Article/details/gvuqzmkqi.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fehbvm.com/Article/details/gpptkmckq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.hesvh.cn/Article/details/gccrmxbrt.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gmvhdmzej.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.hesvh.cn/Article/details/gkpxgwsuj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gbzjyizsa.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gejaanlqc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fehbvm.com/Article/details/gzgqdogco.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gpyfujrdh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gllyvkpyi.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gtnnpyvhp.sHtML

[F11] 复制与移动文件
来源：http://blog.hesvh.cn/Article/details/ghrfkrmcg.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gbjqhoine.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.hesvh.cn/Article/details/gtmumoqrb.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gzsynsjcj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/ggnmsyqtt.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gkxhyglja.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.hesvh.cn/Article/details/gqmmafunv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gtsoenfsd.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.zdbjq.cn/Article/details/gdaclosvm.sHtML

[F12] CSV 读写
来源：http://www.blog.zdbjq.cn/Article/details/ggwzxltyx.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fehbvm.com/Article/details/gymwuvbwi.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.fehbvm.com/Article/details/giopcijob.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.zdbjq.cn/Article/details/gnayyeyel.sHtML

TS:   // 同上
来源：http://www.share.zdbjq.cn/Article/details/gnxryiiuw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.hesvh.cn/Article/details/gizxfdyco.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.zdbjq.cn/Article/details/ghpujmtvr.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.zdbjq.cn/Article/details/gypibbzbz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.fehbvm.com/Article/details/gjllaobiz.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/grndkauju.sHtML

G. 面向对象
来源：http://www.blog.hesvh.cn/Article/details/gumfmdgzd.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqemeaeku.sHtML

[G01] 定义类
来源：http://3g.hesvh.cn/Article/details/gerirknfh.sHtML

Py:   class User: pass
来源：http://read.share.zdbjq.cn/Article/details/gcwgkasnn.sHtML

PHP:  class User {}
来源：http://blog.hesvh.cn/Article/details/gstifpncx.sHtML

JS:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gnbctcvzm.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.zdbjq.cn/Article/details/gxbqkstbb.sHtML

Java: class User {}
来源：http://3g.hesvh.cn/Article/details/gcajqgxwp.sHtML

Go:   type User struct { Name string }
来源：http://baike.fehbvm.com/Article/details/gsvwcgynk.sHtML

Ruby: class User; end
来源：http://www.m.share.fehbvm.com/Article/details/gxuhpkjnv.sHtML

C#:   class User {}
来源：http://m.share.fehbvm.com/Article/details/grynzgvxk.sHtML

[G02] 构造函数
来源：http://read.share.fehbvm.com/Article/details/gapvjdugx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fehbvm.com/Article/details/gnwpldyfl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.zdbjq.cn/Article/details/gqlfnucfe.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gsfsbhicy.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.fehbvm.com/Article/details/givmhktxj.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/ggygelwmo.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.zdbjq.cn/Article/details/gwerrtwlh.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.hesvh.cn/Article/details/grbnltcbx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.hesvh.cn/Article/details/gzrunsnzu.sHtML

[G03] 实例属性
来源：http://www.m.share.fehbvm.com/Article/details/gipidiakb.sHtML

Py:   self.name = "x"
来源：http://3g.zdbjq.cn/Article/details/gubsgywce.sHtML

PHP:  public string $name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gvxkwagec.sHtML

JS:   this.name = "x";
来源：http://mobile.hesvh.cn/Article/details/ghdrvrykk.sHtML

TS:   name: string = "x";
来源：http://blog.hesvh.cn/Article/details/gterxnyiv.sHtML

Java: private String name;
来源：http://wap.fehbvm.com/Article/details/giccdggsn.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.zdbjq.cn/Article/details/gygjolscl.sHtML

Ruby: @name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gibmopuay.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.hesvh.cn/Article/details/gcvuujmpx.sHtML

[G04] 定义方法
来源：http://blog.zdbjq.cn/Article/details/grwsmsyim.sHtML

Py:   def greet(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gytcskxhj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gqyorynpt.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gvetivmdm.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gueytjtvp.sHtML

Java: String greet() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gidiqxlrw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/ggihupoid.sHtML

Ruby: def greet; @name; end
来源：http://m.share.zdbjq.cn/Article/details/gvpqcyrkn.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.hesvh.cn/Article/details/gbpqsrvkx.sHtML

[G05] 继承
来源：http://read.share.zdbjq.cn/Article/details/gojzkvxfh.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/gsbiccssp.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gwfxsfzvt.sHtML

JS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gdppwcpeu.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gpelkchhv.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/glhbqzrbx.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.hesvh.cn/Article/details/gyhmzjwcq.sHtML

Ruby: class Admin < User; end
来源：http://3g.zdbjq.cn/Article/details/gsrxziozl.sHtML

C#:   class Admin : User {}
来源：http://mobile.fehbvm.com/Article/details/gdqasgcwq.sHtML

[G06] 重写方法
来源：http://m.share.fehbvm.com/Article/details/gqbgbndfx.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.zdbjq.cn/Article/details/gaeiltqdf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghajorxhd.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gvxqbuphk.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gllnbocsh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gqmjeuavr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.zdbjq.cn/Article/details/gwbtzgoza.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.zdbjq.cn/Article/details/ggydhhnrs.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.hesvh.cn/Article/details/gjrlpezua.sHtML

[G07] 调用父类方法
来源：http://baike.zdbjq.cn/Article/details/gdflhcvvr.sHtML

Py:   super().greet()
来源：http://www.share.fehbvm.com/Article/details/gsrnctwgd.sHtML

PHP:  parent::greet();
来源：http://mobile.fehbvm.com/Article/details/gsyizebbc.sHtML

JS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gmgyblqpb.sHtML

TS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gupraxhfm.sHtML

Java: super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gjahcbauf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.fehbvm.com/Article/details/gcpmxrchn.sHtML

Ruby: super
来源：http://read.share.hesvh.cn/Article/details/ghcbrjcxr.sHtML

C#:   base.Greet();
来源：http://blog.zdbjq.cn/Article/details/gvhiakeql.sHtML

[G08] 静态方法与属性
来源：http://baike.fehbvm.com/Article/details/gjwuormuj.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.zdbjq.cn/Article/details/gmnpdrspw.sHtML

PHP:  public static function f() {}
来源：http://wap.fehbvm.com/Article/details/gxukiqtuq.sHtML

JS:   static f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gctjqqdtv.sHtML

TS:   static f(): void {}
来源：http://www.share.hesvh.cn/Article/details/gjdjtblou.sHtML

Java: static void f() {}
来源：http://m.share.zdbjq.cn/Article/details/gampixynm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.zdbjq.cn/Article/details/gtntlpapr.sHtML

Ruby: def self.f; end
来源：http://blog.fehbvm.com/Article/details/gfwmxqyya.sHtML

C#:   public static void F() {}
来源：http://blog.zdbjq.cn/Article/details/gynkhqpyx.sHtML

[G09] 接口 / 抽象类
来源：http://wap.zdbjq.cn/Article/details/gqysfktoj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.hesvh.cn/Article/details/gzorthhvp.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.hesvh.cn/Article/details/gjeemcolv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.zdbjq.cn/Article/details/gwwiyeunl.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fehbvm.com/Article/details/gwmpgkihh.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fehbvm.com/Article/details/ghpkaezhf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.zdbjq.cn/Article/details/gofbcsesv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.zdbjq.cn/Article/details/gfticfhil.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.zdbjq.cn/Article/details/ghfpotcxe.sHtML

[G10] 访问控制
来源：http://www.m.share.fehbvm.com/Article/details/ghmreiokb.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.hesvh.cn/Article/details/gjduolrgv.sHtML

PHP:  public / protected / private
来源：http://baike.zdbjq.cn/Article/details/guhotzihr.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.zdbjq.cn/Article/details/gcoeqggsp.sHtML

TS:   public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gbwudgkkh.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.zdbjq.cn/Article/details/gyybjrtto.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.zdbjq.cn/Article/details/golgenzrj.sHtML

Ruby: public / protected / private
来源：http://baike.fehbvm.com/Article/details/gkhtacamc.sHtML

C#:   public / protected / private / internal
来源：http://read.share.fehbvm.com/Article/details/glroxlvun.sHtML

[G11] getter / setter
来源：http://m.share.fehbvm.com/Article/details/gbexjuoyy.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.fehbvm.com/Article/details/gmqivkgvx.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gvgrriclb.sHtML

JS:   get name() { return this._name; }
来源：http://baike.fehbvm.com/Article/details/gtsldbccj.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gqszamgjk.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gweqfxdml.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gnnpaxfvf.sHtML

Ruby: attr_accessor :name
来源：http://baike.zdbjq.cn/Article/details/gentkcrbx.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.fehbvm.com/Article/details/giscopxqj.sHtML

[G12] 对象转字符串
来源：http://read.share.zdbjq.cn/Article/details/gdvmohpft.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gynjvadux.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtymotwlb.sHtML

JS:   toString() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gfxuiegwu.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gbjtdirfa.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gadrigowi.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gdxzdtxgi.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.hesvh.cn/Article/details/gbbwkvguq.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.hesvh.cn/Article/details/gpbsblrrv.sHtML

[G13] 判断对象类型
来源：http://www.m.share.zdbjq.cn/Article/details/gfakydugg.sHtML

Py:   isinstance(u, User)
来源：http://m.share.zdbjq.cn/Article/details/gocwfadiv.sHtML

PHP:  $u instanceof User
来源：http://read.share.hesvh.cn/Article/details/glygvyqmf.sHtML

JS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gofwbzqie.sHtML

TS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gnntgjbck.sHtML

Java: u instanceof User
来源：http://baike.hesvh.cn/Article/details/gmowuepgp.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.zdbjq.cn/Article/details/geiubyjsk.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.zdbjq.cn/Article/details/gbagnqbfg.sHtML

C#:   u is User
来源：http://www.blog.zdbjq.cn/Article/details/gbtdpjuxz.sHtML

[G14] 数据类 / record
来源：http://www.share.zdbjq.cn/Article/details/gjakhetgk.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.fehbvm.com/Article/details/gaxtzejwf.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.hesvh.cn/Article/details/gsktxfbhq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.zdbjq.cn/Article/details/gassvsbws.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.hesvh.cn/Article/details/ghphfeukg.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.hesvh.cn/Article/details/gsmtpbngp.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.hesvh.cn/Article/details/ggiejyllx.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.hesvh.cn/Article/details/gasjvmivq.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.fehbvm.com/Article/details/gtblxbxcn.sHtML

[G15] 枚举
来源：http://read.share.hesvh.cn/Article/details/gnmeqcajk.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.zdbjq.cn/Article/details/gmhzxlseh.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.zdbjq.cn/Article/details/guyjnfhoy.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.zdbjq.cn/Article/details/giptrdfju.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gwcxnqjoi.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fehbvm.com/Article/details/ggjmtebes.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.hesvh.cn/Article/details/gxuxfhequ.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.hesvh.cn/Article/details/goefpzocg.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gyluvfmmg.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.hesvh.cn/Article/details/geneahxxw.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.hesvh.cn/Article/details/gwbvhedme.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.fehbvm.com/Article/details/grwofepin.sHtML

JS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gjluikwns.sHtML

TS:   Object.entries(obj)
来源：http://wap.zdbjq.cn/Article/details/gnhjolrfj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.zdbjq.cn/Article/details/gqnndstuw.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.hesvh.cn/Article/details/ggkpnirad.sHtML

Ruby: obj.instance_variables
来源：http://blog.zdbjq.cn/Article/details/gzncyxrtz.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.hesvh.cn/Article/details/gylbktdvu.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gusoqnphg.sHtML

H. 异常与错误处理
来源：http://mobile.fehbvm.com/Article/details/gtyriqmss.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gnbvhqger.sHtML

[H01] try / catch 基础
来源：http://wap.fehbvm.com/Article/details/gjijmaoyf.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.hesvh.cn/Article/details/gmhvhcfmg.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.zdbjq.cn/Article/details/glhyhzkjk.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gmtsyznwv.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gzwzinewp.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.fehbvm.com/Article/details/gjapzvaag.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.hesvh.cn/Article/details/gvkfnktmb.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.zdbjq.cn/Article/details/gicehijku.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.zdbjq.cn/Article/details/gnarmmsgz.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.zdbjq.cn/Article/details/gijqaqenr.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.fehbvm.com/Article/details/gmrlwuebv.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gkhxdoidm.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gsrnhyhkj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/guoutoggf.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gxeybnkre.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.fehbvm.com/Article/details/gyfmjqdxq.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.hesvh.cn/Article/details/gmtazlxdt.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gmsvdhaxd.sHtML

[H03] 主动抛出异常
来源：http://mobile.zdbjq.cn/Article/details/grescylhu.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.fehbvm.com/Article/details/gyicosltm.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gkjodamiy.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gcudukrod.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gakqsjgnl.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gvgryovzo.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.hesvh.cn/Article/details/gszyrrbmk.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.fehbvm.com/Article/details/gxwnmzdwd.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gqjrxecbv.sHtML

[H04] 自定义异常类型
来源：http://blog.hesvh.cn/Article/details/gnbvjvxhi.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.hesvh.cn/Article/details/gamrfotkh.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.fehbvm.com/Article/details/gepzmbyoa.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.hesvh.cn/Article/details/gczugmdgd.sHtML

TS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/gblzseczv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.hesvh.cn/Article/details/gxzqhillu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.fehbvm.com/Article/details/gzihucqen.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.hesvh.cn/Article/details/gsehtejtz.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.zdbjq.cn/Article/details/gzfkyxpmu.sHtML

[H05] 捕获特定类型
来源：http://www.blog.fehbvm.com/Article/details/gpbesdiot.sHtML

Py:   except ValueError as e:
来源：http://wap.hesvh.cn/Article/details/glvxxqruy.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.fehbvm.com/Article/details/gilydrlid.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/gnovvllsv.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/gxclrgwce.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.fehbvm.com/Article/details/ghpakyrjv.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.hesvh.cn/Article/details/gimdblkzj.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.fehbvm.com/Article/details/gxsnwuyxy.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.hesvh.cn/Article/details/gdkfrihrv.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.hesvh.cn/Article/details/gfrursxfe.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.zdbjq.cn/Article/details/ggpitimzg.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gpockbhmp.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.hesvh.cn/Article/details/gornwyfco.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.hesvh.cn/Article/details/gfubcriuq.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.hesvh.cn/Article/details/gxailffbq.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.zdbjq.cn/Article/details/gtwxkioku.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.zdbjq.cn/Article/details/gfxgbyjbj.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.zdbjq.cn/Article/details/ghhptfnux.sHtML

[H07] 断言
来源：http://3g.zdbjq.cn/Article/details/ghsxtdusx.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.hesvh.cn/Article/details/gsdqgoxaa.sHtML

PHP:  assert($x > 0);
来源：http://baike.zdbjq.cn/Article/details/gukvjelbg.sHtML

JS:   console.assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/guqlbticb.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/gqnfysvcw.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.fehbvm.com/Article/details/gycdbzztu.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.zdbjq.cn/Article/details/gqrcqwqbe.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.share.hesvh.cn/Article/details/gmtjgsmmk.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gjqfalxeg.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.zdbjq.cn/Article/details/gnuxdptil.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.hesvh.cn/Article/details/gwgcnxgxe.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.m.share.zdbjq.cn/Article/details/gozroclqa.sHtML

JS:   e.message;  e.stack
来源：http://www.share.hesvh.cn/Article/details/gmtxfgtjx.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://baike.hesvh.cn/Article/details/gofwnqtac.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.zdbjq.cn/Article/details/gajyppzaf.sHtML

Go:   err.Error()
来源：http://baike.fehbvm.com/Article/details/gazujxsjz.sHtML

Ruby: e.message;  e.backtrace
来源：http://wap.fehbvm.com/Article/details/gaccxwmad.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.fehbvm.com/Article/details/gsloicswq.sHtML

[H09] 带错误码的异常
来源：http://wap.fehbvm.com/Article/details/gictnhqvp.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.zdbjq.cn/Article/details/gantpmrtx.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.fehbvm.com/Article/details/gycucumsy.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.zdbjq.cn/Article/details/gjynfrbfb.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.zdbjq.cn/Article/details/gqvkcplap.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.hesvh.cn/Article/details/giabfpjei.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.hesvh.cn/Article/details/gdkfjhpya.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.fehbvm.com/Article/details/gjdbssdtd.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.hesvh.cn/Article/details/gemmgriyh.sHtML

[H10] 资源自动释放
来源：http://3g.zdbjq.cn/Article/details/gqdwmveyo.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.fehbvm.com/Article/details/gjweagznm.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.fehbvm.com/Article/details/gnpcgcivg.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.zdbjq.cn/Article/details/gnldqlxtz.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.hesvh.cn/Article/details/gthdzrbqy.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.blog.hesvh.cn/Article/details/gubescput.sHtML

Go:   defer f.Close()
来源：http://m.share.fehbvm.com/Article/details/gophkkfnv.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://read.share.fehbvm.com/Article/details/gyanuginy.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/ggkeojrsk.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gydmuvbqb.sHtML

I. 正则表达式
来源：http://blog.zdbjq.cn/Article/details/giflowdip.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gpjigcpom.sHtML

[I01] 判断是否匹配
来源：http://www.share.hesvh.cn/Article/details/ggrbxsbqf.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.hesvh.cn/Article/details/gssxlhupz.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.fehbvm.com/Article/details/gwcqrvgwf.sHtML

JS:   /\d+/.test(s)
来源：http://wap.zdbjq.cn/Article/details/gehtbwzad.sHtML

TS:   /\d+/.test(s)
来源：http://baike.fehbvm.com/Article/details/gdmmlqyqw.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://m.share.zdbjq.cn/Article/details/gonoqvbhd.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.fehbvm.com/Article/details/gdmeutbql.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.zdbjq.cn/Article/details/gnrraauwb.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.hesvh.cn/Article/details/gqpugzbzs.sHtML

[I02] 提取所有匹配
来源：http://m.share.zdbjq.cn/Article/details/gjroknosa.sHtML

Py:   re.findall(r"\d+", s)
来源：http://blog.hesvh.cn/Article/details/gctstczus.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.zdbjq.cn/Article/details/gudyducmr.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.fehbvm.com/Article/details/grhfwwses.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.zdbjq.cn/Article/details/ghoyfvyxh.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.hesvh.cn/Article/details/gdzmydlfp.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.fehbvm.com/Article/details/gfdjbvpxj.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.hesvh.cn/Article/details/gwzevilhy.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://m.share.hesvh.cn/Article/details/gvqjewiak.sHtML

[I03] 提取捕获分组
来源：http://blog.zdbjq.cn/Article/details/gqpgmkmwj.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.fehbvm.com/Article/details/goqeorekb.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gedeuygar.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.blog.hesvh.cn/Article/details/gbnzxtxuv.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://m.share.fehbvm.com/Article/details/grhtvkipo.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.fehbvm.com/Article/details/gpsxivnux.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.hesvh.cn/Article/details/gjwktsduq.sHtML


<!-- 参考信息 -->