代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://www.share.hesvh.cn/Article/details/grnawrlhe.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.fehbvm.com/Article/details/grptsllor.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gwyghjhtp.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.zdbjq.cn/Article/details/gyutnhjax.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gfzroxasb.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gevdymbcx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.hesvh.cn/Article/details/gjrlqtzxd.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gijhggpat.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gvmencwix.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gzxxdderu.sHtML

[F11] 复制与移动文件
来源：http://m.share.fehbvm.com/Article/details/gvruujrsi.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gkrafbbdh.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.hesvh.cn/Article/details/gwwppsypp.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gmlhofget.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gzfxrnqtu.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.hesvh.cn/Article/details/gbwmveadl.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.fehbvm.com/Article/details/gytsbhlsq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gamjumzee.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.fehbvm.com/Article/details/gswqfcpdm.sHtML

[F12] CSV 读写
来源：http://www.m.share.fehbvm.com/Article/details/gcvlrhxpj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.hesvh.cn/Article/details/gtrmhixmp.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.zdbjq.cn/Article/details/gnmwfhaue.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.hesvh.cn/Article/details/gitkmrglh.sHtML

TS:   // 同上
来源：http://baike.zdbjq.cn/Article/details/ggsfmjmwv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.hesvh.cn/Article/details/gtyovprnz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.zdbjq.cn/Article/details/gqdihcjeo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.hesvh.cn/Article/details/guodiyaoy.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fehbvm.com/Article/details/gbrrcmzcl.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gberiloqh.sHtML

G. 面向对象
来源：http://m.share.hesvh.cn/Article/details/gymojijvk.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gcecqfuyv.sHtML

[G01] 定义类
来源：http://www.share.zdbjq.cn/Article/details/gnsnmdhhr.sHtML

Py:   class User: pass
来源：http://www.share.fehbvm.com/Article/details/gfszlgyxl.sHtML

PHP:  class User {}
来源：http://3g.fehbvm.com/Article/details/gapsqgfjd.sHtML

JS:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gttjrogyw.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.zdbjq.cn/Article/details/gdeiiirmy.sHtML

Java: class User {}
来源：http://www.blog.fehbvm.com/Article/details/gfujqesir.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/gmopdgdgw.sHtML

Ruby: class User; end
来源：http://3g.zdbjq.cn/Article/details/gkmdcwsge.sHtML

C#:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/giomaceor.sHtML

[G02] 构造函数
来源：http://blog.fehbvm.com/Article/details/gmpznbztl.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.hesvh.cn/Article/details/ginfqlwoz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.zdbjq.cn/Article/details/guaqmefmh.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gzlpnsnxb.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.hesvh.cn/Article/details/gsosylefs.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gfcetxgeb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/gkckeqkvl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.fehbvm.com/Article/details/ghfjwxmzn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.zdbjq.cn/Article/details/gpvpewtdv.sHtML

[G03] 实例属性
来源：http://www.blog.fehbvm.com/Article/details/gzcruvulv.sHtML

Py:   self.name = "x"
来源：http://blog.fehbvm.com/Article/details/gfxrpcdim.sHtML

PHP:  public string $name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gspcgjnaw.sHtML

JS:   this.name = "x";
来源：http://www.blog.hesvh.cn/Article/details/guomfolec.sHtML

TS:   name: string = "x";
来源：http://baike.zdbjq.cn/Article/details/gwutxdxke.sHtML

Java: private String name;
来源：http://www.share.fehbvm.com/Article/details/glzuahncn.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.fehbvm.com/Article/details/gqztuehln.sHtML

Ruby: @name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gxvzsztog.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.zdbjq.cn/Article/details/gafzidskp.sHtML

[G04] 定义方法
来源：http://www.share.zdbjq.cn/Article/details/gzjkwrsjk.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gpozmdfua.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/ghyzjpazi.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gjchmpmmm.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gmzzpslzd.sHtML

Java: String greet() { return name; }
来源：http://baike.fehbvm.com/Article/details/gswfxujqb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gvxosgeke.sHtML

Ruby: def greet; @name; end
来源：http://3g.fehbvm.com/Article/details/gyldgxdgk.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.hesvh.cn/Article/details/gpwlrfwsl.sHtML

[G05] 继承
来源：http://mobile.zdbjq.cn/Article/details/gxxelikfd.sHtML

Py:   class Admin(User): pass
来源：http://3g.fehbvm.com/Article/details/ghkozrdve.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gvoxylvmv.sHtML

JS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gfwvgoacg.sHtML

TS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gbweqduln.sHtML

Java: class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/ghmhamagt.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.zdbjq.cn/Article/details/gdqujozed.sHtML

Ruby: class Admin < User; end
来源：http://mobile.zdbjq.cn/Article/details/gzazsuxww.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.hesvh.cn/Article/details/ghyzhbqyy.sHtML

[G06] 重写方法
来源：http://wap.zdbjq.cn/Article/details/gqbqvlnhy.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.fehbvm.com/Article/details/gichxpcuz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/ggdlfquae.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gjxjxdvmp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gkhjibpgi.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gmkdmtpho.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fehbvm.com/Article/details/gyhaotfld.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.hesvh.cn/Article/details/gwxctfmbj.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fehbvm.com/Article/details/gpdppxnjr.sHtML

[G07] 调用父类方法
来源：http://www.m.share.zdbjq.cn/Article/details/glquudaou.sHtML

Py:   super().greet()
来源：http://baike.fehbvm.com/Article/details/gloyozixm.sHtML

PHP:  parent::greet();
来源：http://mobile.hesvh.cn/Article/details/gtzycuuxo.sHtML

JS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gtianxham.sHtML

TS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gfrthxvdi.sHtML

Java: super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gldtnrfhp.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.zdbjq.cn/Article/details/ghlhmleat.sHtML

Ruby: super
来源：http://baike.fehbvm.com/Article/details/gudbjlhpl.sHtML

C#:   base.Greet();
来源：http://www.blog.fehbvm.com/Article/details/gptrhzutu.sHtML

[G08] 静态方法与属性
来源：http://mobile.fehbvm.com/Article/details/ggifqpwpl.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.zdbjq.cn/Article/details/giwouqulm.sHtML

PHP:  public static function f() {}
来源：http://www.blog.zdbjq.cn/Article/details/grtwjaohg.sHtML

JS:   static f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gkksbaafp.sHtML

TS:   static f(): void {}
来源：http://mobile.fehbvm.com/Article/details/gspsdgajy.sHtML

Java: static void f() {}
来源：http://www.m.share.hesvh.cn/Article/details/ggcaahhpw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.fehbvm.com/Article/details/gxgxuuivz.sHtML

Ruby: def self.f; end
来源：http://www.blog.zdbjq.cn/Article/details/gniqwepsk.sHtML

C#:   public static void F() {}
来源：http://www.share.fehbvm.com/Article/details/goghlkaqe.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.fehbvm.com/Article/details/gmotisrkf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.fehbvm.com/Article/details/gmikuvzcn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.zdbjq.cn/Article/details/gnxzjrpbc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.hesvh.cn/Article/details/gulonnmrg.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.zdbjq.cn/Article/details/gwcokrwdj.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fehbvm.com/Article/details/gowtxmvtn.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.zdbjq.cn/Article/details/gczgaqqhr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.hesvh.cn/Article/details/gxpmhmvat.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.zdbjq.cn/Article/details/gjfxeislz.sHtML

[G10] 访问控制
来源：http://wap.hesvh.cn/Article/details/gskqinqvx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.zdbjq.cn/Article/details/gvkratrgr.sHtML

PHP:  public / protected / private
来源：http://blog.zdbjq.cn/Article/details/ghqubrvtz.sHtML

JS:   #private 字段；其余公开
来源：http://baike.hesvh.cn/Article/details/gaacswtvk.sHtML

TS:   public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/ggfzrdztc.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fehbvm.com/Article/details/gmlixtnlk.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fehbvm.com/Article/details/gvcgqetjy.sHtML

Ruby: public / protected / private
来源：http://wap.hesvh.cn/Article/details/gyqgbygzb.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.zdbjq.cn/Article/details/gfbpxbhok.sHtML

[G11] getter / setter
来源：http://3g.fehbvm.com/Article/details/glvmxrxoy.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.zdbjq.cn/Article/details/gsororrns.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gmsafjslg.sHtML

JS:   get name() { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/gqbfufflw.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gocgkngpu.sHtML

Java: public String getName() { return name; }
来源：http://blog.fehbvm.com/Article/details/gjaiunusd.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/ghpnvjyup.sHtML

Ruby: attr_accessor :name
来源：http://www.share.hesvh.cn/Article/details/gdobhreyg.sHtML

C#:   public string Name { get; set; }
来源：http://wap.hesvh.cn/Article/details/gufdjajwm.sHtML

[G12] 对象转字符串
来源：http://3g.fehbvm.com/Article/details/ggrnpyyvz.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/ghhvrjynu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gminlilcm.sHtML

JS:   toString() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/guvtzjflj.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/glhueqdhu.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.hesvh.cn/Article/details/grufbndlu.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gumekpmtb.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gwfisboec.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.hesvh.cn/Article/details/gxezofluo.sHtML

[G13] 判断对象类型
来源：http://www.m.share.hesvh.cn/Article/details/gegumglif.sHtML

Py:   isinstance(u, User)
来源：http://read.share.fehbvm.com/Article/details/gaoxodfmt.sHtML

PHP:  $u instanceof User
来源：http://blog.hesvh.cn/Article/details/gyfgkkcjw.sHtML

JS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gamglnivr.sHtML

TS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/gdjvqkfzx.sHtML

Java: u instanceof User
来源：http://3g.hesvh.cn/Article/details/gdrvqdimz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.fehbvm.com/Article/details/glvocaivq.sHtML

Ruby: u.is_a?(User)
来源：http://baike.hesvh.cn/Article/details/gjbfwmvri.sHtML

C#:   u is User
来源：http://www.share.fehbvm.com/Article/details/gkpstbnnj.sHtML

[G14] 数据类 / record
来源：http://www.share.zdbjq.cn/Article/details/gxxlblwel.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.zdbjq.cn/Article/details/gzbsxwbbx.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.fehbvm.com/Article/details/gmfpnxuqh.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.fehbvm.com/Article/details/grkhhbemc.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.hesvh.cn/Article/details/ggdqsjagg.sHtML

Java: record User(String name, int age) {}
来源：http://blog.zdbjq.cn/Article/details/gvddhneit.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.hesvh.cn/Article/details/goqnrmmjk.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.fehbvm.com/Article/details/gfrqiazxs.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.fehbvm.com/Article/details/gnriozzxw.sHtML

[G15] 枚举
来源：http://www.blog.hesvh.cn/Article/details/gkuxcqcwb.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fehbvm.com/Article/details/glyvlefiy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fehbvm.com/Article/details/gcdfkggmk.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.zdbjq.cn/Article/details/gmmgdiitc.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gsizymixu.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.zdbjq.cn/Article/details/gaekupmuy.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.hesvh.cn/Article/details/gcsgpwmsb.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.fehbvm.com/Article/details/gmifqdjxo.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fehbvm.com/Article/details/gqnnlrycc.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.hesvh.cn/Article/details/goliqshmr.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.hesvh.cn/Article/details/gnyzzmjxe.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.hesvh.cn/Article/details/gcpjrodef.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gekqggvif.sHtML

TS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/gidlrvdbc.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.hesvh.cn/Article/details/gegwdzmka.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.fehbvm.com/Article/details/gbnrnxbrs.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.fehbvm.com/Article/details/ggtdvkjuq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.fehbvm.com/Article/details/glcdiifbr.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gvfkkrrvv.sHtML

H. 异常与错误处理
来源：http://3g.hesvh.cn/Article/details/gormqbwso.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvptxjajb.sHtML

[H01] try / catch 基础
来源：http://read.share.zdbjq.cn/Article/details/gqworfkdu.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.zdbjq.cn/Article/details/gmyntwfyz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.fehbvm.com/Article/details/gizwogzlr.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gynycdprx.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/gppmwzuzi.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.fehbvm.com/Article/details/gchoiaxem.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.zdbjq.cn/Article/details/gbljlidfy.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.zdbjq.cn/Article/details/ggovrzbjy.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.hesvh.cn/Article/details/glmfbhtgp.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.fehbvm.com/Article/details/gpzjrpdns.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.zdbjq.cn/Article/details/gaxeyifod.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gnupndmdp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gemqikcdm.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gtaqtmlak.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/guvhursat.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.fehbvm.com/Article/details/giwwaezzh.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.zdbjq.cn/Article/details/gdpakcaxn.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/ghbfgfkqv.sHtML

[H03] 主动抛出异常
来源：http://wap.fehbvm.com/Article/details/grdlgbosw.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.zdbjq.cn/Article/details/gwyrbvdlf.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/grjklcxbo.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/ggwrcbwff.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/gdzbvmcll.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gmvwvxqew.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.hesvh.cn/Article/details/gvthkasje.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.zdbjq.cn/Article/details/gyghxrolk.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gbcajtjcr.sHtML

[H04] 自定义异常类型
来源：http://baike.hesvh.cn/Article/details/gerdamino.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.hesvh.cn/Article/details/gvwbumtrq.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/gudmznucp.sHtML

JS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/grxhdxnil.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/gvtrluyyj.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.hesvh.cn/Article/details/gtlkyylox.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fehbvm.com/Article/details/gluwnxkaw.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.fehbvm.com/Article/details/gwdyhormf.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.hesvh.cn/Article/details/geipyscin.sHtML

[H05] 捕获特定类型
来源：http://read.share.fehbvm.com/Article/details/gbzkwfehh.sHtML

Py:   except ValueError as e:
来源：http://baike.hesvh.cn/Article/details/gxbfozywo.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.zdbjq.cn/Article/details/gzhkrlmeu.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/gcrdmumur.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.fehbvm.com/Article/details/gwpishlhl.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.hesvh.cn/Article/details/gzwdxgbzi.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.zdbjq.cn/Article/details/gasgdfgzi.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.hesvh.cn/Article/details/gknflszsl.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.hesvh.cn/Article/details/gehmdopsm.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.hesvh.cn/Article/details/ghxomfdvv.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.zdbjq.cn/Article/details/guaeewgug.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.fehbvm.com/Article/details/glqdtghtx.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.zdbjq.cn/Article/details/gtouakdkh.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.hesvh.cn/Article/details/geusjdqeg.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.zdbjq.cn/Article/details/gsfcljhry.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.hesvh.cn/Article/details/gbidnyqma.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.hesvh.cn/Article/details/gsabvsiml.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.hesvh.cn/Article/details/grphvvpdj.sHtML

[H07] 断言
来源：http://mobile.zdbjq.cn/Article/details/gqbhghcng.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.zdbjq.cn/Article/details/gngposrmc.sHtML

PHP:  assert($x > 0);
来源：http://read.share.fehbvm.com/Article/details/gxiglfitj.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gpsyjqbac.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gcmgxcsij.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.hesvh.cn/Article/details/grahfndkq.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.zdbjq.cn/Article/details/gevqjjzmo.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.hesvh.cn/Article/details/gwrycxttv.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/glqiyqtsa.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.zdbjq.cn/Article/details/gfysbpyeg.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.zdbjq.cn/Article/details/givukjzpj.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.zdbjq.cn/Article/details/gwjremoek.sHtML

JS:   e.message;  e.stack
来源：http://m.share.fehbvm.com/Article/details/geepikagn.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.fehbvm.com/Article/details/gaexduerk.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.zdbjq.cn/Article/details/goezggjvt.sHtML

Go:   err.Error()
来源：http://www.blog.fehbvm.com/Article/details/gmsgldidw.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.fehbvm.com/Article/details/gxcuixoha.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.zdbjq.cn/Article/details/gvuszinwx.sHtML

[H09] 带错误码的异常
来源：http://mobile.hesvh.cn/Article/details/gxqtybrpi.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.zdbjq.cn/Article/details/gkrjzwixv.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.zdbjq.cn/Article/details/gfbtdlszr.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.hesvh.cn/Article/details/gpgxqhphz.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.zdbjq.cn/Article/details/gazjqfxuu.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://m.share.zdbjq.cn/Article/details/gsoevqhak.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.fehbvm.com/Article/details/gkkhoslze.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.fehbvm.com/Article/details/gxkikmgmg.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.hesvh.cn/Article/details/gtjrexpta.sHtML

[H10] 资源自动释放
来源：http://mobile.zdbjq.cn/Article/details/ggbzxnmrt.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.fehbvm.com/Article/details/gqwsetmau.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://mobile.zdbjq.cn/Article/details/gjjaqhteu.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fehbvm.com/Article/details/gmrldmmai.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://baike.zdbjq.cn/Article/details/gvzycjsar.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://3g.hesvh.cn/Article/details/gguioagqm.sHtML

Go:   defer f.Close()
来源：http://baike.zdbjq.cn/Article/details/gcnundodw.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.hesvh.cn/Article/details/gunelqufv.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gewwilvcy.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/geyeyrvws.sHtML

I. 正则表达式
来源：http://3g.hesvh.cn/Article/details/gxzzwvxdb.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gcyeifyut.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.fehbvm.com/Article/details/gfkasznuq.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.zdbjq.cn/Article/details/gkkrygvkj.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.fehbvm.com/Article/details/gmizeresp.sHtML

JS:   /\d+/.test(s)
来源：http://baike.hesvh.cn/Article/details/gptnhrfde.sHtML

TS:   /\d+/.test(s)
来源：http://3g.hesvh.cn/Article/details/guswpygsh.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.fehbvm.com/Article/details/gvesiysqd.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.zdbjq.cn/Article/details/gwgvpmrck.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gpmpyemtx.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://mobile.zdbjq.cn/Article/details/gtbphsqjg.sHtML

[I02] 提取所有匹配
来源：http://wap.hesvh.cn/Article/details/gaeqvriro.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.zdbjq.cn/Article/details/gzobcwywy.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.zdbjq.cn/Article/details/gzrgsihpn.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.zdbjq.cn/Article/details/gmgajwdjp.sHtML

TS:   s.match(/\d+/g)
来源：http://3g.hesvh.cn/Article/details/gkzpftlov.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.fehbvm.com/Article/details/gaobnrvhs.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://3g.zdbjq.cn/Article/details/gkgghbklb.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.hesvh.cn/Article/details/gdarjpswj.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gcbvceazh.sHtML

[I03] 提取捕获分组
来源：http://m.share.hesvh.cn/Article/details/gigudoyfx.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.blog.zdbjq.cn/Article/details/gthrsuaoe.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.hesvh.cn/Article/details/gjzhngvsk.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.zdbjq.cn/Article/details/gbzyacjek.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.hesvh.cn/Article/details/ghcorrkzq.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://3g.zdbjq.cn/Article/details/gstgdxpni.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.fehbvm.com/Article/details/gnyjretcz.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.fehbvm.com/Article/details/gmffuadtk.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.fehbvm.com/Article/details/gtggbkkfo.sHtML

[I04] 正则替换
来源：http://mobile.zdbjq.cn/Article/details/gjqhjgoca.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.hesvh.cn/Article/details/grkcunnkn.sHtML


<!-- 参考信息 -->