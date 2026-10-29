代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gawqfqndu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gqykjusyc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.hesvh.cn/Article/details/gytxirxik.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/ghdmqlotx.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.hesvh.cn/Article/details/gcnkktufk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fehbvm.com/Article/details/gtghdcqmy.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gecvkaqar.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.hesvh.cn/Article/details/glqppeqmx.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gmfnuzlos.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gibfzfycr.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.zdbjq.cn/Article/details/gujczvlrp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gqesafadw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gjetebucg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gfpfrrkgq.sHtML

[F11] 复制与移动文件
来源：http://wap.fehbvm.com/Article/details/gvbhjaqze.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gltupmupb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.hesvh.cn/Article/details/gnbbvktlc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gqvulceqn.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gkjafypsu.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.fehbvm.com/Article/details/gffamhszg.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.hesvh.cn/Article/details/givesddjp.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gnpjslkdz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.hesvh.cn/Article/details/gyjuvjlkc.sHtML

[F12] CSV 读写
来源：http://www.share.zdbjq.cn/Article/details/gfgtmzuyo.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.fehbvm.com/Article/details/gsclgeksn.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.fehbvm.com/Article/details/garehdvxl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fehbvm.com/Article/details/gxbazxveu.sHtML

TS:   // 同上
来源：http://baike.zdbjq.cn/Article/details/gdsnteuqw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fehbvm.com/Article/details/gyghicntq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fehbvm.com/Article/details/gugzqsfah.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.zdbjq.cn/Article/details/gjmtrkuyl.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.hesvh.cn/Article/details/geowxvgrq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ggofrubhe.sHtML

G. 面向对象
来源：http://www.share.fehbvm.com/Article/details/gzbacjrmv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/grownegut.sHtML

[G01] 定义类
来源：http://mobile.hesvh.cn/Article/details/gesspsoda.sHtML

Py:   class User: pass
来源：http://www.blog.fehbvm.com/Article/details/ggcgicoyx.sHtML

PHP:  class User {}
来源：http://blog.hesvh.cn/Article/details/gcckreopd.sHtML

JS:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gyiwmrhnt.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.fehbvm.com/Article/details/ggvcxkhaj.sHtML

Java: class User {}
来源：http://3g.zdbjq.cn/Article/details/gjvmkcstb.sHtML

Go:   type User struct { Name string }
来源：http://m.share.hesvh.cn/Article/details/gscawayxo.sHtML

Ruby: class User; end
来源：http://www.m.share.zdbjq.cn/Article/details/gxzvmwojs.sHtML

C#:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gdwbucrtk.sHtML

[G02] 构造函数
来源：http://www.blog.hesvh.cn/Article/details/gqoehfgfs.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.hesvh.cn/Article/details/gdvifptxm.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.fehbvm.com/Article/details/gpdgghysf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.fehbvm.com/Article/details/gjicqcwhv.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.hesvh.cn/Article/details/ghgwxnvsb.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gvacubcka.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.fehbvm.com/Article/details/guwlufdoy.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fehbvm.com/Article/details/gocxpgnyj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfxcwilbt.sHtML

[G03] 实例属性
来源：http://www.blog.zdbjq.cn/Article/details/guysxxvmr.sHtML

Py:   self.name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gvbncxkqz.sHtML

PHP:  public string $name = "x";
来源：http://wap.zdbjq.cn/Article/details/gwnwcbtgs.sHtML

JS:   this.name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gvrjkyxds.sHtML

TS:   name: string = "x";
来源：http://www.blog.hesvh.cn/Article/details/ghiopuqsn.sHtML

Java: private String name;
来源：http://www.m.share.hesvh.cn/Article/details/gdejcnhmp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.hesvh.cn/Article/details/gjdintavp.sHtML

Ruby: @name = "x"
来源：http://baike.zdbjq.cn/Article/details/geyfygxmg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.fehbvm.com/Article/details/gknozeakq.sHtML

[G04] 定义方法
来源：http://m.share.hesvh.cn/Article/details/gpsgxrnlq.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/goiaofevg.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gsffvcgvd.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gkfytiyjj.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gwhskshro.sHtML

Java: String greet() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gpafssqzg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gbjytiygr.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fehbvm.com/Article/details/gmhykhbjr.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.hesvh.cn/Article/details/gftrwkzuw.sHtML

[G05] 继承
来源：http://baike.hesvh.cn/Article/details/guntuyxmi.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.zdbjq.cn/Article/details/gduzcriod.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gibkqhqtk.sHtML

JS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/grrwkrcbv.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gpguczkqf.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/ggvwmlzsd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.zdbjq.cn/Article/details/gbswemqqb.sHtML

Ruby: class Admin < User; end
来源：http://wap.hesvh.cn/Article/details/giddezlvd.sHtML

C#:   class Admin : User {}
来源：http://baike.zdbjq.cn/Article/details/gblcsrbaj.sHtML

[G06] 重写方法
来源：http://www.share.hesvh.cn/Article/details/gcztujogo.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.zdbjq.cn/Article/details/glhvhqkqs.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gcvvincfx.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gnztkdwoi.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gbxqnolrv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gikfjauxc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.zdbjq.cn/Article/details/guqdbeltl.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.zdbjq.cn/Article/details/gyixcwasg.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.hesvh.cn/Article/details/gikcifntl.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fehbvm.com/Article/details/gzwysjbgt.sHtML

Py:   super().greet()
来源：http://www.m.share.zdbjq.cn/Article/details/ghnjaqrxi.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fehbvm.com/Article/details/gegjfdkzc.sHtML

JS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gygpxfbxe.sHtML

TS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gaqyxdfmw.sHtML

Java: super.greet();
来源：http://3g.zdbjq.cn/Article/details/ghhnkbowj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.fehbvm.com/Article/details/gvfnjcwyn.sHtML

Ruby: super
来源：http://blog.hesvh.cn/Article/details/gmnxxaizz.sHtML

C#:   base.Greet();
来源：http://www.m.share.fehbvm.com/Article/details/gbfbkqtcu.sHtML

[G08] 静态方法与属性
来源：http://read.share.fehbvm.com/Article/details/gplenbhfm.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.fehbvm.com/Article/details/gfrgpfaes.sHtML

PHP:  public static function f() {}
来源：http://read.share.zdbjq.cn/Article/details/gpbypbacd.sHtML

JS:   static f() {}
来源：http://www.share.fehbvm.com/Article/details/gkuhvajxm.sHtML

TS:   static f(): void {}
来源：http://3g.hesvh.cn/Article/details/gkpiadjsb.sHtML

Java: static void f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gxwqraolt.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.hesvh.cn/Article/details/gefabksuu.sHtML

Ruby: def self.f; end
来源：http://baike.fehbvm.com/Article/details/godspaelj.sHtML

C#:   public static void F() {}
来源：http://3g.hesvh.cn/Article/details/gnkephkmd.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.fehbvm.com/Article/details/ggyeceeuk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.zdbjq.cn/Article/details/gbxakqpbb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fehbvm.com/Article/details/gdibbepqh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.fehbvm.com/Article/details/gbzctbuba.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.hesvh.cn/Article/details/gqjkqjpmg.sHtML

Java: interface Shape { double area(); }
来源：http://3g.fehbvm.com/Article/details/gcdamjlag.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.hesvh.cn/Article/details/gkgnwjhtg.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.zdbjq.cn/Article/details/gbzzrtgau.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gabybosbk.sHtML

[G10] 访问控制
来源：http://www.m.share.fehbvm.com/Article/details/gpkoghnmo.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.fehbvm.com/Article/details/gdczezbzs.sHtML

PHP:  public / protected / private
来源：http://blog.fehbvm.com/Article/details/gcmmjpzdu.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fehbvm.com/Article/details/gqnjpslbf.sHtML

TS:   public / protected / private
来源：http://baike.zdbjq.cn/Article/details/ghsacrdjv.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.hesvh.cn/Article/details/genuztrzu.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fehbvm.com/Article/details/gsfdwoyfu.sHtML

Ruby: public / protected / private
来源：http://wap.zdbjq.cn/Article/details/ghxvhnnzq.sHtML

C#:   public / protected / private / internal
来源：http://mobile.hesvh.cn/Article/details/gqmdkfsgi.sHtML

[G11] getter / setter
来源：http://www.share.fehbvm.com/Article/details/gvowvsgjx.sHtML

Py:   @property 与 @x.setter
来源：http://3g.zdbjq.cn/Article/details/gygcfamns.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gqjkzntud.sHtML

JS:   get name() { return this._name; }
来源：http://3g.hesvh.cn/Article/details/gtrocgicz.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gojkqsmfv.sHtML

Java: public String getName() { return name; }
来源：http://baike.fehbvm.com/Article/details/ggswofhxv.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gjdhdgrzs.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fehbvm.com/Article/details/gqteixgnu.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.fehbvm.com/Article/details/gjkyupwdc.sHtML

[G12] 对象转字符串
来源：http://mobile.zdbjq.cn/Article/details/gpgrepcdx.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/ggkrvoqdj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/ghuaxutmb.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/giihxszuz.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gkbjqyiao.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.hesvh.cn/Article/details/gddjdknki.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/glioqvyim.sHtML

Ruby: def to_s; @name; end
来源：http://baike.hesvh.cn/Article/details/gtjfrvktq.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gtcburvjb.sHtML

[G13] 判断对象类型
来源：http://www.m.share.hesvh.cn/Article/details/godbjnsvg.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fehbvm.com/Article/details/gtkxwkffk.sHtML

PHP:  $u instanceof User
来源：http://baike.fehbvm.com/Article/details/gzwomvpze.sHtML

JS:   u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/grljftkhl.sHtML

TS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/glifxhiix.sHtML

Java: u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gwiycxsav.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.hesvh.cn/Article/details/gsqvhcksv.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.zdbjq.cn/Article/details/gackljsxo.sHtML

C#:   u is User
来源：http://3g.hesvh.cn/Article/details/gdbsdjjsf.sHtML

[G14] 数据类 / record
来源：http://wap.hesvh.cn/Article/details/gqojzyevq.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.zdbjq.cn/Article/details/gmcmiyuwn.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.fehbvm.com/Article/details/giuijrpny.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.fehbvm.com/Article/details/gehigjuml.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.fehbvm.com/Article/details/gwgifuhnq.sHtML

Java: record User(String name, int age) {}
来源：http://baike.zdbjq.cn/Article/details/gpxzvxneu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.hesvh.cn/Article/details/gpzcaxjud.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.zdbjq.cn/Article/details/gjzdzregn.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.zdbjq.cn/Article/details/gsazbgvaw.sHtML

[G15] 枚举
来源：http://m.share.zdbjq.cn/Article/details/ghobkwuut.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.zdbjq.cn/Article/details/gnxddabnl.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.zdbjq.cn/Article/details/ghdnzfsdd.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fehbvm.com/Article/details/grqversrk.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gvptnjbij.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.fehbvm.com/Article/details/gkzibgjdx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.zdbjq.cn/Article/details/gsghjdqod.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.hesvh.cn/Article/details/gcmrxmozd.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gublpuchj.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.fehbvm.com/Article/details/gfrlwkhky.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.zdbjq.cn/Article/details/glwiosvdl.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.fehbvm.com/Article/details/gckpohpft.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.zdbjq.cn/Article/details/ggwesncrt.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/gvzzsfyqc.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.hesvh.cn/Article/details/gxicnycmz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.hesvh.cn/Article/details/gbmskmglq.sHtML

Ruby: obj.instance_variables
来源：http://3g.fehbvm.com/Article/details/gchlfmvnc.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.zdbjq.cn/Article/details/gsbmsrleh.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gsnzjdmhp.sHtML

H. 异常与错误处理
来源：http://mobile.zdbjq.cn/Article/details/gjyqosdil.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/giodnfzxi.sHtML

[H01] try / catch 基础
来源：http://m.share.fehbvm.com/Article/details/gmnooctpz.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.hesvh.cn/Article/details/gykfxqbzw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.zdbjq.cn/Article/details/gehbkmefm.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gkgevecej.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gkwisjsxk.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.zdbjq.cn/Article/details/ggznzgzhc.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.fehbvm.com/Article/details/ghkhophiw.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.fehbvm.com/Article/details/gmjxcqkqy.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.hesvh.cn/Article/details/gfwzdfbbv.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.zdbjq.cn/Article/details/gzskepecv.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.fehbvm.com/Article/details/gkgivfway.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gavwoyrpy.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/grilfiwtr.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gnntooxki.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gfmqeutwx.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.fehbvm.com/Article/details/glxqonoqo.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.fehbvm.com/Article/details/giqyibiyl.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gwymvicgc.sHtML

[H03] 主动抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/gbwhexkil.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.hesvh.cn/Article/details/gnrxddqdw.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gmlptjtwl.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/grvueditv.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/gnksjybpa.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gzgdqkucf.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.zdbjq.cn/Article/details/ghpghaiex.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.fehbvm.com/Article/details/gxlgsyjrp.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/graozibod.sHtML

[H04] 自定义异常类型
来源：http://3g.zdbjq.cn/Article/details/guzhllqdu.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.fehbvm.com/Article/details/gejzhditc.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.hesvh.cn/Article/details/gpwwpqapg.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/gvwxuhcex.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/gqfrglhax.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.fehbvm.com/Article/details/gdcpobqbu.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.hesvh.cn/Article/details/gbtfazvmu.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.fehbvm.com/Article/details/ghzrgsmxp.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.hesvh.cn/Article/details/gkdoyjsrw.sHtML

[H05] 捕获特定类型
来源：http://m.share.hesvh.cn/Article/details/gkrnxxzda.sHtML

Py:   except ValueError as e:
来源：http://www.share.hesvh.cn/Article/details/gyzfbkjsw.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.zdbjq.cn/Article/details/gvwdwplmd.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/gqlosyqrm.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/gutkesygm.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.fehbvm.com/Article/details/goasqqvcm.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.zdbjq.cn/Article/details/gdvbjpyzq.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.hesvh.cn/Article/details/gmcisdyat.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.fehbvm.com/Article/details/gfommcbwy.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.hesvh.cn/Article/details/gkpzoxrdz.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.fehbvm.com/Article/details/gqdppaswy.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/gaiqfmjbx.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.hesvh.cn/Article/details/gdmwxvrhe.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fehbvm.com/Article/details/gkzxsnzkn.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.fehbvm.com/Article/details/gjnnksrrh.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.fehbvm.com/Article/details/gksfkahlr.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.fehbvm.com/Article/details/gjvbhkygg.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.hesvh.cn/Article/details/gimknihpp.sHtML

[H07] 断言
来源：http://blog.zdbjq.cn/Article/details/gwzgumjkw.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.zdbjq.cn/Article/details/ghmrltzbw.sHtML

PHP:  assert($x > 0);
来源：http://m.share.hesvh.cn/Article/details/gitkingyh.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gkoazetox.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gegvhhvtg.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.hesvh.cn/Article/details/gsxbkghcg.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.fehbvm.com/Article/details/gptpfjmvj.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.fehbvm.com/Article/details/gbzvfnmuk.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gunicpadn.sHtML

[H08] 获取错误信息与堆栈
来源：http://3g.hesvh.cn/Article/details/gtagayjrn.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.hesvh.cn/Article/details/givawzmne.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.zdbjq.cn/Article/details/ggwnsasjb.sHtML

JS:   e.message;  e.stack
来源：http://blog.fehbvm.com/Article/details/ghqisbcnf.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.fehbvm.com/Article/details/gqjwjrzch.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.blog.zdbjq.cn/Article/details/gksfcqpoj.sHtML

Go:   err.Error()
来源：http://baike.zdbjq.cn/Article/details/guassbwjg.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.zdbjq.cn/Article/details/gitxostny.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.zdbjq.cn/Article/details/gsjmfvebj.sHtML

[H09] 带错误码的异常
来源：http://read.share.hesvh.cn/Article/details/gfzvhresj.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.zdbjq.cn/Article/details/gvlvuldtz.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.fehbvm.com/Article/details/gjrhtoaou.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.hesvh.cn/Article/details/gqlsujxxt.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.zdbjq.cn/Article/details/gtwsgfzdg.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.fehbvm.com/Article/details/gcproiukn.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.zdbjq.cn/Article/details/gxlcfnayv.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.blog.hesvh.cn/Article/details/gaymedojr.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://read.share.fehbvm.com/Article/details/ggankqhuz.sHtML

[H10] 资源自动释放
来源：http://www.share.hesvh.cn/Article/details/gngftjrut.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.hesvh.cn/Article/details/gbxfkhoqp.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.zdbjq.cn/Article/details/gqspwisoq.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.hesvh.cn/Article/details/gsocudzvl.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.zdbjq.cn/Article/details/ggzfibxfn.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.fehbvm.com/Article/details/gmashvqhd.sHtML

Go:   defer f.Close()
来源：http://wap.hesvh.cn/Article/details/gldtiljew.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.hesvh.cn/Article/details/gnqujjhuj.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gihfdbscf.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gsabugwpm.sHtML

I. 正则表达式
来源：http://3g.fehbvm.com/Article/details/gfknaogxa.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gqtbkcgog.sHtML

[I01] 判断是否匹配
来源：http://www.blog.zdbjq.cn/Article/details/gbcbxtwvx.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.hesvh.cn/Article/details/gzidebxdv.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.fehbvm.com/Article/details/glnomcmhm.sHtML

JS:   /\d+/.test(s)
来源：http://3g.hesvh.cn/Article/details/gazgxqtzv.sHtML

TS:   /\d+/.test(s)
来源：http://wap.fehbvm.com/Article/details/gissfsbdz.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.fehbvm.com/Article/details/gokmzftzj.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.hesvh.cn/Article/details/gomcywdpd.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.zdbjq.cn/Article/details/gadisfnfv.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.fehbvm.com/Article/details/gcvsaiblt.sHtML

[I02] 提取所有匹配
来源：http://blog.hesvh.cn/Article/details/gxnbpepkf.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.zdbjq.cn/Article/details/gbbwkxeea.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.hesvh.cn/Article/details/gvidvpklt.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.zdbjq.cn/Article/details/gxfuhhlfk.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.zdbjq.cn/Article/details/gpdnemozz.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.zdbjq.cn/Article/details/gphjppnqc.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.hesvh.cn/Article/details/gywsipvos.sHtML

Ruby: s.scan(/\d+/)
来源：http://wap.zdbjq.cn/Article/details/giumnrriu.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gohgygefk.sHtML

[I03] 提取捕获分组
来源：http://3g.zdbjq.cn/Article/details/gjybslnsy.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.hesvh.cn/Article/details/gehibnyue.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gwrcdyvbm.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.zdbjq.cn/Article/details/gdqsrqmap.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://blog.fehbvm.com/Article/details/gwqkqqecr.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://baike.hesvh.cn/Article/details/gdzmergxd.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://3g.hesvh.cn/Article/details/grhvfxykm.sHtML


<!-- 参考信息 -->