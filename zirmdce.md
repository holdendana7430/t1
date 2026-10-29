代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gplytjisx.sHtML

TS:   path.extname("a.txt")
来源：http://blog.hesvh.cn/Article/details/gtimnrqnk.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.fehbvm.com/Article/details/gasmtcwrx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gugefydde.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gfzdnjaqz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/glzbclsvd.sHtML

[F11] 复制与移动文件
来源：http://baike.fehbvm.com/Article/details/gipoveudr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gfmrmipyp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.fehbvm.com/Article/details/gcetzccya.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gxglhbecb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gvvefuvxc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.fehbvm.com/Article/details/gdfhkhxll.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.zdbjq.cn/Article/details/gxiohcsmg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gxugxeogd.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.hesvh.cn/Article/details/gcrhqniyc.sHtML

[F12] CSV 读写
来源：http://blog.fehbvm.com/Article/details/gmflnukao.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.zdbjq.cn/Article/details/gsappqbyx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.zdbjq.cn/Article/details/gliadetft.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.hesvh.cn/Article/details/gwjmvmtqq.sHtML

TS:   // 同上
来源：http://m.share.fehbvm.com/Article/details/gyfccvymp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.hesvh.cn/Article/details/gyqwlafxm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.fehbvm.com/Article/details/gmrkstvnu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fehbvm.com/Article/details/gbdwtzeie.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.zdbjq.cn/Article/details/gllfmckvo.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gzpprzhqv.sHtML

G. 面向对象
来源：http://wap.zdbjq.cn/Article/details/gbrkolhrv.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gsbonkxva.sHtML

[G01] 定义类
来源：http://mobile.hesvh.cn/Article/details/gpvyrqrzp.sHtML

Py:   class User: pass
来源：http://baike.hesvh.cn/Article/details/gjjziwipj.sHtML

PHP:  class User {}
来源：http://www.share.hesvh.cn/Article/details/gxjgncaoy.sHtML

JS:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gxelzgipv.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fehbvm.com/Article/details/gdqiaynmn.sHtML

Java: class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gnyykmrnn.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.fehbvm.com/Article/details/grijjbnhq.sHtML

Ruby: class User; end
来源：http://3g.zdbjq.cn/Article/details/gzfbqauiy.sHtML

C#:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gpdocimhl.sHtML

[G02] 构造函数
来源：http://m.share.hesvh.cn/Article/details/goqsdmdsx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.hesvh.cn/Article/details/ggzuaeqau.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gnkdfglds.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gabgrsiny.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fehbvm.com/Article/details/gjojdpjzo.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gfgbvhjpn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.zdbjq.cn/Article/details/gwsnbbolu.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.hesvh.cn/Article/details/grihsagun.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fehbvm.com/Article/details/gyhjhgcvk.sHtML

[G03] 实例属性
来源：http://www.share.fehbvm.com/Article/details/gepymhssq.sHtML

Py:   self.name = "x"
来源：http://wap.zdbjq.cn/Article/details/gxqegkgej.sHtML

PHP:  public string $name = "x";
来源：http://baike.hesvh.cn/Article/details/gaaquriyi.sHtML

JS:   this.name = "x";
来源：http://blog.fehbvm.com/Article/details/grhibulmf.sHtML

TS:   name: string = "x";
来源：http://read.share.fehbvm.com/Article/details/gaokflxra.sHtML

Java: private String name;
来源：http://wap.zdbjq.cn/Article/details/gmqotnfqr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.zdbjq.cn/Article/details/ghhwcebxk.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gtjlxuayw.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.hesvh.cn/Article/details/ghmzyhjmp.sHtML

[G04] 定义方法
来源：http://m.share.fehbvm.com/Article/details/gtsfvborg.sHtML

Py:   def greet(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gmfrlmnru.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gutvytutp.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gexkjnxzk.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gkbidvupy.sHtML

Java: String greet() { return name; }
来源：http://wap.hesvh.cn/Article/details/gcxljfmnb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gjguoicfp.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/grirdhtss.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.hesvh.cn/Article/details/gtvyovvwm.sHtML

[G05] 继承
来源：http://www.blog.hesvh.cn/Article/details/gmuzabdmb.sHtML

Py:   class Admin(User): pass
来源：http://mobile.zdbjq.cn/Article/details/grldsxbvq.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gcqunyoej.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gzaoiykxf.sHtML

TS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gxvjuqyti.sHtML

Java: class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gpjfitnsr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.hesvh.cn/Article/details/gyxodyxor.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.fehbvm.com/Article/details/gaafbfxwn.sHtML

C#:   class Admin : User {}
来源：http://mobile.hesvh.cn/Article/details/gqqoqwteg.sHtML

[G06] 重写方法
来源：http://baike.hesvh.cn/Article/details/gupnctjcc.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.zdbjq.cn/Article/details/gkbegjiez.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gptwghosq.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gdyhhhyzh.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gceegiomk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/ghpknnhtn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.zdbjq.cn/Article/details/gsermwxjm.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.hesvh.cn/Article/details/gittzsdsp.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.hesvh.cn/Article/details/gcommulxr.sHtML

[G07] 调用父类方法
来源：http://www.blog.fehbvm.com/Article/details/gvgslgmfk.sHtML

Py:   super().greet()
来源：http://wap.zdbjq.cn/Article/details/gtpsjgdzw.sHtML

PHP:  parent::greet();
来源：http://m.share.zdbjq.cn/Article/details/gtebwggbk.sHtML

JS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gqpsjdnfi.sHtML

TS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gbqxjpteo.sHtML

Java: super.greet();
来源：http://wap.zdbjq.cn/Article/details/gjqhiczya.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.zdbjq.cn/Article/details/gzoewreut.sHtML

Ruby: super
来源：http://blog.zdbjq.cn/Article/details/gfnkyjpkt.sHtML

C#:   base.Greet();
来源：http://read.share.hesvh.cn/Article/details/gkumjdlxp.sHtML

[G08] 静态方法与属性
来源：http://m.share.hesvh.cn/Article/details/gdwwqlscz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.fehbvm.com/Article/details/gakvyaxxo.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gpuioymyg.sHtML

JS:   static f() {}
来源：http://m.share.zdbjq.cn/Article/details/ggdsutmad.sHtML

TS:   static f(): void {}
来源：http://www.share.zdbjq.cn/Article/details/gofvxxwzb.sHtML

Java: static void f() {}
来源：http://wap.zdbjq.cn/Article/details/gtjbxnytc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.zdbjq.cn/Article/details/gefcvswss.sHtML

Ruby: def self.f; end
来源：http://read.share.fehbvm.com/Article/details/gihdwcybl.sHtML

C#:   public static void F() {}
来源：http://www.blog.hesvh.cn/Article/details/godhqxnic.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.zdbjq.cn/Article/details/gizlzjjnk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.hesvh.cn/Article/details/ghrvvmfof.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.hesvh.cn/Article/details/gpanrqvft.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.fehbvm.com/Article/details/gmxdnrdme.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxyfqlnad.sHtML

Java: interface Shape { double area(); }
来源：http://3g.hesvh.cn/Article/details/gjzxsaplg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.zdbjq.cn/Article/details/gdqhdymfz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.hesvh.cn/Article/details/gjulaxgft.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.zdbjq.cn/Article/details/guaokffjn.sHtML

[G10] 访问控制
来源：http://blog.fehbvm.com/Article/details/gemccbzpi.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.fehbvm.com/Article/details/gsgpmifts.sHtML

PHP:  public / protected / private
来源：http://blog.fehbvm.com/Article/details/gslddmkpx.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.hesvh.cn/Article/details/gjzubhzmw.sHtML

TS:   public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gambpsqds.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.hesvh.cn/Article/details/gcvusxmot.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.zdbjq.cn/Article/details/gwxflnozk.sHtML

Ruby: public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gtkzezklq.sHtML

C#:   public / protected / private / internal
来源：http://read.share.zdbjq.cn/Article/details/giuwgwgcv.sHtML

[G11] getter / setter
来源：http://m.share.hesvh.cn/Article/details/ggmmmwlkv.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.hesvh.cn/Article/details/gakioucdw.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gzkgdcqjl.sHtML

JS:   get name() { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/gvnqkgzgu.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gqewoldtl.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gcnqsxyan.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gkgyfhlok.sHtML

Ruby: attr_accessor :name
来源：http://blog.hesvh.cn/Article/details/gywyvtryk.sHtML

C#:   public string Name { get; set; }
来源：http://baike.zdbjq.cn/Article/details/gvwyjzfzh.sHtML

[G12] 对象转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gwuunhqem.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gikdpqdaf.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gyuwpjvdq.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/govuvmxes.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/guqcoqzig.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gptyovfzh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/ghuwcolqv.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fehbvm.com/Article/details/gnxlpamjh.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gfvtkthrx.sHtML

[G13] 判断对象类型
来源：http://www.blog.zdbjq.cn/Article/details/gvaqyszxj.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.zdbjq.cn/Article/details/gzveviupr.sHtML

PHP:  $u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gcudmspii.sHtML

JS:   u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gshxxfonj.sHtML

TS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gecojazyn.sHtML

Java: u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gucbehlhr.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.zdbjq.cn/Article/details/gcrkhjulq.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.zdbjq.cn/Article/details/ggaydcfgo.sHtML

C#:   u is User
来源：http://read.share.hesvh.cn/Article/details/gruhhxnfs.sHtML

[G14] 数据类 / record
来源：http://m.share.zdbjq.cn/Article/details/gldnxlajr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.hesvh.cn/Article/details/gywqjbyfo.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.hesvh.cn/Article/details/goceapwfv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.zdbjq.cn/Article/details/grdentsvm.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.zdbjq.cn/Article/details/gwkaghocr.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gswgvqotn.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.fehbvm.com/Article/details/gcrjyhbzj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.zdbjq.cn/Article/details/gfcozdqsn.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.hesvh.cn/Article/details/guxmdjhdi.sHtML

[G15] 枚举
来源：http://3g.hesvh.cn/Article/details/gxvxdqccf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.hesvh.cn/Article/details/gnwalaobw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.hesvh.cn/Article/details/gonvsiuov.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.fehbvm.com/Article/details/gautrtenv.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/gtcvjwufe.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.hesvh.cn/Article/details/giksbowzt.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.hesvh.cn/Article/details/gqluryfnq.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.zdbjq.cn/Article/details/gzdelymah.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gucufjhoq.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.zdbjq.cn/Article/details/gqiaqoaek.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.zdbjq.cn/Article/details/gwgkqrxcl.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.zdbjq.cn/Article/details/geasjibjx.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/gvaxvjnud.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/gdvectdox.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.hesvh.cn/Article/details/gfvgcastv.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.hesvh.cn/Article/details/gbsfjcmca.sHtML

Ruby: obj.instance_variables
来源：http://www.share.fehbvm.com/Article/details/gwaegrgnh.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/gnfqjrhjw.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gazexhkxq.sHtML

H. 异常与错误处理
来源：http://www.blog.fehbvm.com/Article/details/gzzbxinxw.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbmeacpgi.sHtML

[H01] try / catch 基础
来源：http://3g.hesvh.cn/Article/details/gkrqqxusk.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.zdbjq.cn/Article/details/gdelgynuz.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fehbvm.com/Article/details/gswdbrauh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gswltwqwx.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/ggudwasai.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.fehbvm.com/Article/details/gfnlojflt.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.fehbvm.com/Article/details/gnifknqey.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.fehbvm.com/Article/details/gavjlehxp.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.zdbjq.cn/Article/details/glarghsll.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.hesvh.cn/Article/details/gtkaemwsu.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.fehbvm.com/Article/details/gjlunspae.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gxcjdhnzg.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gxxoqzewl.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gpkpzzutx.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gbycdmmon.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fehbvm.com/Article/details/ggduqsuci.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fehbvm.com/Article/details/gnlqgiems.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gejteikto.sHtML

[H03] 主动抛出异常
来源：http://blog.fehbvm.com/Article/details/gewgbdgpp.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.fehbvm.com/Article/details/gczpwbplv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gfgudlzqz.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gsryvrndc.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gijrsophn.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gihgxzjfi.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.zdbjq.cn/Article/details/gavnnrsug.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.fehbvm.com/Article/details/gecoiljma.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gbvqdvlbb.sHtML

[H04] 自定义异常类型
来源：http://www.share.fehbvm.com/Article/details/geqtikeys.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.fehbvm.com/Article/details/ghnablwpq.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/greydbzbn.sHtML

JS:   class MyError extends Error {}
来源：http://blog.zdbjq.cn/Article/details/gyftxnsuw.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.fehbvm.com/Article/details/gsbaxumkt.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/ghtjvuahh.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.zdbjq.cn/Article/details/gmsvxqbxn.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.hesvh.cn/Article/details/gahstdgcq.sHtML

C#:   class MyException : Exception {}
来源：http://3g.zdbjq.cn/Article/details/gkmoxnrrv.sHtML

[H05] 捕获特定类型
来源：http://www.blog.hesvh.cn/Article/details/gvadxyovw.sHtML

Py:   except ValueError as e:
来源：http://baike.fehbvm.com/Article/details/gozqvckit.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.zdbjq.cn/Article/details/gtmnbiuhx.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/grcgmjmiq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/gkykyrreo.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.zdbjq.cn/Article/details/garfzorgz.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.fehbvm.com/Article/details/gmsbdqatk.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.zdbjq.cn/Article/details/gqanlwgps.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.zdbjq.cn/Article/details/givhhjmmy.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.zdbjq.cn/Article/details/gdlwsdurc.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.fehbvm.com/Article/details/gtthtwhpn.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/gufomqtsn.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/gaugmpxiv.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.hesvh.cn/Article/details/gxjtjfmum.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.hesvh.cn/Article/details/gutoowcrw.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.hesvh.cn/Article/details/gklfhsoxg.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.fehbvm.com/Article/details/gergkfqzj.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.fehbvm.com/Article/details/giclimzub.sHtML

[H07] 断言
来源：http://read.share.hesvh.cn/Article/details/gogkyorxu.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.zdbjq.cn/Article/details/gksuxjnoa.sHtML

PHP:  assert($x > 0);
来源：http://blog.zdbjq.cn/Article/details/gadzlxlit.sHtML

JS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gdcuvywes.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gabkpdxyv.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.zdbjq.cn/Article/details/gyvpfunad.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.fehbvm.com/Article/details/gxetzaphm.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.fehbvm.com/Article/details/gncankhqh.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gljbczdmy.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.fehbvm.com/Article/details/gzpzyiahn.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.zdbjq.cn/Article/details/guzrxluoz.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.hesvh.cn/Article/details/gfbpxjsbn.sHtML

JS:   e.message;  e.stack
来源：http://blog.hesvh.cn/Article/details/gczbsayqt.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.fehbvm.com/Article/details/gteebwbtq.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.zdbjq.cn/Article/details/gordmosrw.sHtML

Go:   err.Error()
来源：http://blog.fehbvm.com/Article/details/gasjgxqhz.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.hesvh.cn/Article/details/gswjcvrtf.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.fehbvm.com/Article/details/gkrabottr.sHtML

[H09] 带错误码的异常
来源：http://baike.zdbjq.cn/Article/details/gomnfqfcp.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.hesvh.cn/Article/details/gdepwdbxv.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.zdbjq.cn/Article/details/gakkubpbc.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.fehbvm.com/Article/details/gpxqthlxs.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.hesvh.cn/Article/details/gerbirmqg.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.zdbjq.cn/Article/details/gdkkezhri.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://read.share.zdbjq.cn/Article/details/gzxqvtikl.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.hesvh.cn/Article/details/gclqgqoik.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.fehbvm.com/Article/details/gtmtemynm.sHtML

[H10] 资源自动释放
来源：http://www.share.zdbjq.cn/Article/details/gdorlzdoi.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.hesvh.cn/Article/details/gmllvxfve.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.zdbjq.cn/Article/details/gvtqdlybx.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.hesvh.cn/Article/details/grswdckxc.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.zdbjq.cn/Article/details/gdhaauvkz.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.zdbjq.cn/Article/details/giunqfqvc.sHtML

Go:   defer f.Close()
来源：http://m.share.hesvh.cn/Article/details/gjlercejc.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.fehbvm.com/Article/details/gmjxgcqab.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gjyfrbngl.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/glfwtawvn.sHtML

I. 正则表达式
来源：http://mobile.hesvh.cn/Article/details/gjaxmjrxi.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gpmqaqxnz.sHtML

[I01] 判断是否匹配
来源：http://wap.zdbjq.cn/Article/details/gtfnaipxm.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.fehbvm.com/Article/details/gglrtymjt.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.hesvh.cn/Article/details/gpshtvfec.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.hesvh.cn/Article/details/gmwlqbwea.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.hesvh.cn/Article/details/gskxhxyje.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://baike.fehbvm.com/Article/details/gjgeawjxr.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.fehbvm.com/Article/details/gwzygyqzh.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.zdbjq.cn/Article/details/gdzmdiwum.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.hesvh.cn/Article/details/gfzlijddu.sHtML

[I02] 提取所有匹配
来源：http://baike.zdbjq.cn/Article/details/gdgosbtxw.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.zdbjq.cn/Article/details/gvcitkxee.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://3g.hesvh.cn/Article/details/gpjzbrezk.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.zdbjq.cn/Article/details/guuxvztkk.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.fehbvm.com/Article/details/ghqgcvbsq.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.hesvh.cn/Article/details/gomeewsbs.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.fehbvm.com/Article/details/gloeubllt.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.zdbjq.cn/Article/details/gnthjxzll.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.fehbvm.com/Article/details/gpnbxgmww.sHtML

[I03] 提取捕获分组
来源：http://www.blog.fehbvm.com/Article/details/gbbvfudal.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.fehbvm.com/Article/details/gqzjkwptg.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://wap.fehbvm.com/Article/details/gxalxvmqx.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://read.share.hesvh.cn/Article/details/gibpzzblv.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.hesvh.cn/Article/details/gfqbaqvrc.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.zdbjq.cn/Article/details/glonbtjfu.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://read.share.fehbvm.com/Article/details/gyoubcrvg.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.fehbvm.com/Article/details/gikwlegxc.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.zdbjq.cn/Article/details/gekhqllip.sHtML

[I04] 正则替换
来源：http://www.m.share.hesvh.cn/Article/details/gftpgldym.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.fehbvm.com/Article/details/grqhxlcrd.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.hesvh.cn/Article/details/gndzkqavn.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/ggtwjxjuq.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.zdbjq.cn/Article/details/gndpyrece.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.zdbjq.cn/Article/details/gzrkwejxx.sHtML


<!-- 参考信息 -->