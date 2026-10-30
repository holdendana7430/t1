代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gdkxqqcbo.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gewexegve.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fehbvm.com/Article/details/googpjtmq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gvggdhato.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gqlyehtdz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gvzstfqrv.sHtML

[F11] 复制与移动文件
来源：http://blog.fehbvm.com/Article/details/goihykplv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gnugrflsv.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.zdbjq.cn/Article/details/gneplfdtn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/glxrvblqr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gfofldgyr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.zdbjq.cn/Article/details/gcxqmmvnz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.fehbvm.com/Article/details/gnpjwlmdp.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gwpglqpro.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fehbvm.com/Article/details/gyuhsqyrs.sHtML

[F12] CSV 读写
来源：http://wap.fehbvm.com/Article/details/gqnvrmaqh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.zdbjq.cn/Article/details/gniwqfwxz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.hesvh.cn/Article/details/gzlmwaztq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.zdbjq.cn/Article/details/gqrdfucxp.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/grzenhkjm.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.hesvh.cn/Article/details/gxhcodxqu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.zdbjq.cn/Article/details/gltwmkojd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.zdbjq.cn/Article/details/geigbxkvi.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.zdbjq.cn/Article/details/gldjefjkv.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/grmwohoax.sHtML

G. 面向对象
来源：http://www.share.hesvh.cn/Article/details/grqipujjl.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gycvwqztf.sHtML

[G01] 定义类
来源：http://baike.zdbjq.cn/Article/details/gsayoljha.sHtML

Py:   class User: pass
来源：http://baike.zdbjq.cn/Article/details/grrfdaive.sHtML

PHP:  class User {}
来源：http://www.share.zdbjq.cn/Article/details/gwoyxppio.sHtML

JS:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gbtrgogmw.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.fehbvm.com/Article/details/gydekatcn.sHtML

Java: class User {}
来源：http://baike.fehbvm.com/Article/details/gpxvchtmf.sHtML

Go:   type User struct { Name string }
来源：http://3g.hesvh.cn/Article/details/ghucwehrj.sHtML

Ruby: class User; end
来源：http://wap.fehbvm.com/Article/details/gatqdgaks.sHtML

C#:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gopmyhzmx.sHtML

[G02] 构造函数
来源：http://wap.fehbvm.com/Article/details/ggelyfqeh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.zdbjq.cn/Article/details/gcuffxgiy.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fehbvm.com/Article/details/gihlrfrlp.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gmpbivzhn.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.zdbjq.cn/Article/details/gapmhslic.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gfsnknexp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.fehbvm.com/Article/details/gdnfcpvql.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.zdbjq.cn/Article/details/glaciotko.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.fehbvm.com/Article/details/gcxmzfwjf.sHtML

[G03] 实例属性
来源：http://blog.zdbjq.cn/Article/details/glgyqqvtv.sHtML

Py:   self.name = "x"
来源：http://3g.hesvh.cn/Article/details/gyepqzabh.sHtML

PHP:  public string $name = "x";
来源：http://www.share.fehbvm.com/Article/details/ghfewdkjr.sHtML

JS:   this.name = "x";
来源：http://baike.zdbjq.cn/Article/details/gccolwzvo.sHtML

TS:   name: string = "x";
来源：http://wap.hesvh.cn/Article/details/gntimayiz.sHtML

Java: private String name;
来源：http://www.blog.zdbjq.cn/Article/details/gildsxxvw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.fehbvm.com/Article/details/gcvjckhdi.sHtML

Ruby: @name = "x"
来源：http://wap.fehbvm.com/Article/details/goahobiap.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.hesvh.cn/Article/details/gxsdtjcdu.sHtML

[G04] 定义方法
来源：http://m.share.fehbvm.com/Article/details/gnavffdjb.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/ggswtavcj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gohjkvfve.sHtML

JS:   greet() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gvyzjgmhi.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gmtgaquzu.sHtML

Java: String greet() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gvsaxxjat.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gegewgewc.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gmgghybey.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.fehbvm.com/Article/details/gridemeuo.sHtML

[G05] 继承
来源：http://www.blog.zdbjq.cn/Article/details/gumzsyjoh.sHtML

Py:   class Admin(User): pass
来源：http://read.share.zdbjq.cn/Article/details/gfqdrigaf.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gquopjklq.sHtML

JS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gkxevimia.sHtML

TS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gpgxyjiew.sHtML

Java: class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gbhukztzj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.zdbjq.cn/Article/details/glnomoeql.sHtML

Ruby: class Admin < User; end
来源：http://3g.zdbjq.cn/Article/details/gafrfqwsx.sHtML

C#:   class Admin : User {}
来源：http://3g.fehbvm.com/Article/details/gmfanoake.sHtML

[G06] 重写方法
来源：http://baike.fehbvm.com/Article/details/gfqfokbhz.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fehbvm.com/Article/details/gekjbedgt.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/giiohxvql.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gvizamjsz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gltxmwkij.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gkoeqsswn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.fehbvm.com/Article/details/gmpmkjzci.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fehbvm.com/Article/details/grsfplpdc.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.hesvh.cn/Article/details/gzaiixyes.sHtML

[G07] 调用父类方法
来源：http://mobile.zdbjq.cn/Article/details/gcmenodab.sHtML

Py:   super().greet()
来源：http://mobile.zdbjq.cn/Article/details/gavysprjg.sHtML

PHP:  parent::greet();
来源：http://www.blog.hesvh.cn/Article/details/gykfducmm.sHtML

JS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gekpvugnt.sHtML

TS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gyjlmqeus.sHtML

Java: super.greet();
来源：http://m.share.fehbvm.com/Article/details/gkkyzqxme.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.fehbvm.com/Article/details/gfthdkerv.sHtML

Ruby: super
来源：http://baike.fehbvm.com/Article/details/gyjrbmozf.sHtML

C#:   base.Greet();
来源：http://www.share.fehbvm.com/Article/details/guzewoofr.sHtML

[G08] 静态方法与属性
来源：http://www.blog.zdbjq.cn/Article/details/gkmsijzkc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.fehbvm.com/Article/details/grhohscjl.sHtML

PHP:  public static function f() {}
来源：http://3g.hesvh.cn/Article/details/gdvvhgipg.sHtML

JS:   static f() {}
来源：http://m.share.fehbvm.com/Article/details/gvkawetqx.sHtML

TS:   static f(): void {}
来源：http://blog.hesvh.cn/Article/details/ggzmzdcyc.sHtML

Java: static void f() {}
来源：http://baike.fehbvm.com/Article/details/glgdjbwfk.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.hesvh.cn/Article/details/gwxcqplts.sHtML

Ruby: def self.f; end
来源：http://baike.hesvh.cn/Article/details/gfjlkijrf.sHtML

C#:   public static void F() {}
来源：http://www.blog.hesvh.cn/Article/details/gkstjqcnz.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.fehbvm.com/Article/details/gpbnpxmpy.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.hesvh.cn/Article/details/gmzjagpjd.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.hesvh.cn/Article/details/gehfudxso.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.hesvh.cn/Article/details/grbdbjzqh.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.hesvh.cn/Article/details/goedsleqy.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gtfcafkcp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.zdbjq.cn/Article/details/gordpxxll.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.zdbjq.cn/Article/details/gchqiksfm.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.zdbjq.cn/Article/details/gmaeljzyy.sHtML

[G10] 访问控制
来源：http://mobile.fehbvm.com/Article/details/gypajspgh.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.hesvh.cn/Article/details/gvgqifkgv.sHtML

PHP:  public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gnsgodwcn.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fehbvm.com/Article/details/gvdhyecrq.sHtML

TS:   public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gynbobhrl.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.zdbjq.cn/Article/details/gzfraqvgo.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fehbvm.com/Article/details/gdcerbesl.sHtML

Ruby: public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gaeubtoyv.sHtML

C#:   public / protected / private / internal
来源：http://baike.fehbvm.com/Article/details/greyeegeq.sHtML

[G11] getter / setter
来源：http://baike.zdbjq.cn/Article/details/gglzgblcn.sHtML

Py:   @property 与 @x.setter
来源：http://blog.zdbjq.cn/Article/details/gjwhhlspm.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/guilmfjcw.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gdczocdwv.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/gmzpcnfld.sHtML

Java: public String getName() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gyfimfqfw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gyysajbqu.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.fehbvm.com/Article/details/gibqbgnfn.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.zdbjq.cn/Article/details/gbynjhfhc.sHtML

[G12] 对象转字符串
来源：http://www.blog.fehbvm.com/Article/details/gnxwrcwav.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gglvkhzbo.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gifoaxonx.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gsskslbss.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/ghlpizuxn.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.fehbvm.com/Article/details/gszuvnwkd.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gewaemjaj.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.fehbvm.com/Article/details/gdpqmnghl.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gwehhtcpg.sHtML

[G13] 判断对象类型
来源：http://wap.zdbjq.cn/Article/details/gcpicvusi.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.hesvh.cn/Article/details/gtqgfnmjx.sHtML

PHP:  $u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gozxvfzpw.sHtML

JS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gusguqwqp.sHtML

TS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/ghtmqozzc.sHtML

Java: u instanceof User
来源：http://3g.hesvh.cn/Article/details/gguofyhnj.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.zdbjq.cn/Article/details/gbwcsemva.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.fehbvm.com/Article/details/gijjlbkib.sHtML

C#:   u is User
来源：http://wap.fehbvm.com/Article/details/gqfrdmktl.sHtML

[G14] 数据类 / record
来源：http://baike.zdbjq.cn/Article/details/gcigwrlgl.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.zdbjq.cn/Article/details/gncuktozr.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.zdbjq.cn/Article/details/gdoikfzmh.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.fehbvm.com/Article/details/gsgeueiyr.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.zdbjq.cn/Article/details/ghwtvsusr.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.hesvh.cn/Article/details/gqjdvhqdz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.hesvh.cn/Article/details/gxdfpxjwj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.hesvh.cn/Article/details/gwkkdmbkz.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.fehbvm.com/Article/details/gzmayihau.sHtML

[G15] 枚举
来源：http://www.m.share.hesvh.cn/Article/details/gxyljfpde.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.zdbjq.cn/Article/details/gcyprvrhj.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fehbvm.com/Article/details/gxqmltthm.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.fehbvm.com/Article/details/gfnsakzfl.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.fehbvm.com/Article/details/gcryvsbmk.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.fehbvm.com/Article/details/gddzfnytc.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.fehbvm.com/Article/details/gtxvtdhku.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.zdbjq.cn/Article/details/guwxeicns.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fehbvm.com/Article/details/gdecdekwm.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.fehbvm.com/Article/details/ggvtkrhpw.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fehbvm.com/Article/details/gezyckdst.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.fehbvm.com/Article/details/gaqgmieoo.sHtML

JS:   Object.entries(obj)
来源：http://www.share.zdbjq.cn/Article/details/geiyikkpi.sHtML

TS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gxqpgiwef.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.hesvh.cn/Article/details/gabtjdjrx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.zdbjq.cn/Article/details/gjjfkubyl.sHtML

Ruby: obj.instance_variables
来源：http://www.share.zdbjq.cn/Article/details/gmhqobman.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/gotsjvjzl.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/goznvfukc.sHtML

H. 异常与错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gvlezjndy.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/godwpglaw.sHtML

[H01] try / catch 基础
来源：http://wap.zdbjq.cn/Article/details/gubkcxncm.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.hesvh.cn/Article/details/grsziggfw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.hesvh.cn/Article/details/gqceudzzy.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gtrsiqziz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gmveoazsk.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.hesvh.cn/Article/details/gjgshxuoi.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.zdbjq.cn/Article/details/gwgjkwson.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.fehbvm.com/Article/details/gzefyqugm.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.hesvh.cn/Article/details/gxfdhjlgg.sHtML

[H02] finally / ensure 收尾
来源：http://blog.hesvh.cn/Article/details/gwolgmasp.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.fehbvm.com/Article/details/grsebnkqq.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gqzmkmuio.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gcqulqpbm.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gegrwzfaf.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/guyexfffk.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.fehbvm.com/Article/details/gpsoojlsj.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.zdbjq.cn/Article/details/guixnaxcc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gvzghdnrr.sHtML

[H03] 主动抛出异常
来源：http://m.share.fehbvm.com/Article/details/gknnsgqcr.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.fehbvm.com/Article/details/gruvfrcyh.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/ggkpkedbb.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gbjrvurxm.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gmgsksgub.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gzednvngh.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.zdbjq.cn/Article/details/gcwxblbrm.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.fehbvm.com/Article/details/ghsftzdqz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/guznefsfr.sHtML

[H04] 自定义异常类型
来源：http://3g.fehbvm.com/Article/details/gftykekzt.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.fehbvm.com/Article/details/gppozjyob.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/gnftddqna.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/goesqospl.sHtML

TS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/gykrfapxv.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/gjovdnvdv.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.zdbjq.cn/Article/details/ggugwcfbp.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.fehbvm.com/Article/details/gtxlfrwes.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.zdbjq.cn/Article/details/gifwnxtjm.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.zdbjq.cn/Article/details/gknrncano.sHtML

Py:   except ValueError as e:
来源：http://mobile.zdbjq.cn/Article/details/gjcllhonx.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.zdbjq.cn/Article/details/ghppmflpx.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.hesvh.cn/Article/details/gqevctvog.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.hesvh.cn/Article/details/gmzrnqgjc.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.fehbvm.com/Article/details/girbyfufd.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.hesvh.cn/Article/details/geqoboajk.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.hesvh.cn/Article/details/gmkjorsdo.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.zdbjq.cn/Article/details/gdxosgeit.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.hesvh.cn/Article/details/gqxstolxo.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.fehbvm.com/Article/details/gzgighfvc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.hesvh.cn/Article/details/gryaybckd.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.hesvh.cn/Article/details/grpveibkm.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.hesvh.cn/Article/details/gvwamsqpu.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.hesvh.cn/Article/details/gqfbwdhgm.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.hesvh.cn/Article/details/gqfufytir.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.hesvh.cn/Article/details/gtvecdack.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.hesvh.cn/Article/details/gytuqqdzt.sHtML

[H07] 断言
来源：http://3g.zdbjq.cn/Article/details/gvykmgisc.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.hesvh.cn/Article/details/gzvjqjrim.sHtML

PHP:  assert($x > 0);
来源：http://blog.zdbjq.cn/Article/details/gxwrylqrc.sHtML

JS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gcjtwkikx.sHtML

TS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gwkvneqju.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.hesvh.cn/Article/details/gwzvcxpti.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.fehbvm.com/Article/details/gtjrwxanl.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.zdbjq.cn/Article/details/gwlomagzs.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.fehbvm.com/Article/details/gzzoqqofp.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.hesvh.cn/Article/details/gcnyblaqk.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.fehbvm.com/Article/details/grurpkknr.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.hesvh.cn/Article/details/gtcglyswu.sHtML

JS:   e.message;  e.stack
来源：http://wap.zdbjq.cn/Article/details/gswmwohrg.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://wap.hesvh.cn/Article/details/gqxmcsfrj.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.hesvh.cn/Article/details/gzxgcqdvf.sHtML

Go:   err.Error()
来源：http://3g.zdbjq.cn/Article/details/gazdvtjaf.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.fehbvm.com/Article/details/gxqlrgooq.sHtML

C#:   e.Message;  e.StackTrace
来源：http://blog.hesvh.cn/Article/details/gosxvqxnr.sHtML

[H09] 带错误码的异常
来源：http://www.share.fehbvm.com/Article/details/gzqrbhnlm.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.share.hesvh.cn/Article/details/gheakijml.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://read.share.hesvh.cn/Article/details/gkakekais.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://wap.zdbjq.cn/Article/details/gnudntago.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.zdbjq.cn/Article/details/girmtkjgy.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.fehbvm.com/Article/details/gsvfowlvh.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.zdbjq.cn/Article/details/gvnghkebw.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://mobile.hesvh.cn/Article/details/gwpxbrvcu.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.hesvh.cn/Article/details/grquzvelv.sHtML

[H10] 资源自动释放
来源：http://wap.fehbvm.com/Article/details/glmuolcok.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.hesvh.cn/Article/details/gbvymdoxx.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://read.share.zdbjq.cn/Article/details/geidgensn.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.hesvh.cn/Article/details/ghaalkdte.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.zdbjq.cn/Article/details/gbxrrlsjv.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://m.share.hesvh.cn/Article/details/gbiomivqw.sHtML

Go:   defer f.Close()
来源：http://wap.zdbjq.cn/Article/details/gcqqfrvju.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.hesvh.cn/Article/details/ghjkvpuho.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.hesvh.cn/Article/details/gcbtwadbu.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gyusipked.sHtML

I. 正则表达式
来源：http://blog.fehbvm.com/Article/details/gmgaebyod.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gvboqsuin.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.hesvh.cn/Article/details/gcgsrmukz.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.zdbjq.cn/Article/details/gefpzeyyy.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gutlvdljn.sHtML

JS:   /\d+/.test(s)
来源：http://wap.zdbjq.cn/Article/details/gozpufyfq.sHtML

TS:   /\d+/.test(s)
来源：http://baike.hesvh.cn/Article/details/gsjaprhyo.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.zdbjq.cn/Article/details/gbicjhfjh.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.zdbjq.cn/Article/details/grvabacjs.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.fehbvm.com/Article/details/gqehurnid.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://blog.hesvh.cn/Article/details/gtpbfbynm.sHtML

[I02] 提取所有匹配
来源：http://mobile.fehbvm.com/Article/details/gyqgsylbj.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.fehbvm.com/Article/details/gumtfloaz.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.hesvh.cn/Article/details/ggaqgnvks.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.fehbvm.com/Article/details/gqqrrfeyc.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.hesvh.cn/Article/details/gjpnclmzx.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.fehbvm.com/Article/details/gbeiashzb.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.fehbvm.com/Article/details/glwbuayhj.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.share.hesvh.cn/Article/details/geffakavq.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.zdbjq.cn/Article/details/gdhijolia.sHtML

[I03] 提取捕获分组
来源：http://read.share.zdbjq.cn/Article/details/gpgsmazfv.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.fehbvm.com/Article/details/gfevkaiqa.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.zdbjq.cn/Article/details/ganpjvicx.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.fehbvm.com/Article/details/gyhpuewyd.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.zdbjq.cn/Article/details/gjhgvdjad.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://wap.zdbjq.cn/Article/details/gfnbsirqf.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.fehbvm.com/Article/details/gkhqjjosi.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.hesvh.cn/Article/details/giyylbhit.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://mobile.hesvh.cn/Article/details/gjmrdtcql.sHtML

[I04] 正则替换
来源：http://m.share.hesvh.cn/Article/details/gbplngcxy.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://baike.hesvh.cn/Article/details/gkeoqwbwz.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://m.share.zdbjq.cn/Article/details/gvzplhyep.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.zdbjq.cn/Article/details/gojjojlha.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fehbvm.com/Article/details/gqqttuzut.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.fehbvm.com/Article/details/ginwixkov.sHtML


<!-- 参考信息 -->