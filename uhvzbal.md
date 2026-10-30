代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gnqhirrdz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gjzmeqgpc.sHtML

[F11] 复制与移动文件
来源：http://wap.fehbvm.com/Article/details/gtxnxptmt.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gdulrgbmg.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.fehbvm.com/Article/details/gydqtinnn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/ggkhbvtua.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gydoqnzer.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.hesvh.cn/Article/details/gpxxxveoz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fehbvm.com/Article/details/gifxnlboi.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gbgvrspdj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.zdbjq.cn/Article/details/glktmmeig.sHtML

[F12] CSV 读写
来源：http://www.m.share.zdbjq.cn/Article/details/gywfbbgsy.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.zdbjq.cn/Article/details/gcnlgbqyj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.zdbjq.cn/Article/details/gfrkynoiu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.zdbjq.cn/Article/details/gebiyxrea.sHtML

TS:   // 同上
来源：http://www.blog.fehbvm.com/Article/details/gnfcbqwnm.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.hesvh.cn/Article/details/gdpsqctnx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.hesvh.cn/Article/details/ghahbaxdw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.zdbjq.cn/Article/details/gdurzfzlf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.fehbvm.com/Article/details/gexdqxmfv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gqoentrbq.sHtML

G. 面向对象
来源：http://blog.fehbvm.com/Article/details/gcknzlhyj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwtjlzpgs.sHtML

[G01] 定义类
来源：http://blog.hesvh.cn/Article/details/geyqxvnyt.sHtML

Py:   class User: pass
来源：http://www.m.share.hesvh.cn/Article/details/gvsyvolle.sHtML

PHP:  class User {}
来源：http://www.share.hesvh.cn/Article/details/glbgxqzmb.sHtML

JS:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gopunggef.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.hesvh.cn/Article/details/gogrbxplh.sHtML

Java: class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gugurylch.sHtML

Go:   type User struct { Name string }
来源：http://m.share.fehbvm.com/Article/details/gezecnblc.sHtML

Ruby: class User; end
来源：http://m.share.hesvh.cn/Article/details/goqhnrnvn.sHtML

C#:   class User {}
来源：http://3g.fehbvm.com/Article/details/gbcfsqppt.sHtML

[G02] 构造函数
来源：http://read.share.hesvh.cn/Article/details/gtyxmmsik.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.hesvh.cn/Article/details/gqxylclbs.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fehbvm.com/Article/details/gvetzkepa.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gigvyjcff.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.zdbjq.cn/Article/details/gkktkzzfo.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gtkpcruor.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fehbvm.com/Article/details/gfflkxjiu.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.zdbjq.cn/Article/details/gutbfjaby.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.zdbjq.cn/Article/details/gtpyrpzme.sHtML

[G03] 实例属性
来源：http://3g.zdbjq.cn/Article/details/gisjxfbuz.sHtML

Py:   self.name = "x"
来源：http://read.share.fehbvm.com/Article/details/gpplcpfpp.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fehbvm.com/Article/details/goejihyiu.sHtML

JS:   this.name = "x";
来源：http://mobile.hesvh.cn/Article/details/grzvaeivd.sHtML

TS:   name: string = "x";
来源：http://www.share.hesvh.cn/Article/details/gefnccdcb.sHtML

Java: private String name;
来源：http://wap.hesvh.cn/Article/details/gfxcxmmew.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fehbvm.com/Article/details/gdicxalst.sHtML

Ruby: @name = "x"
来源：http://m.share.zdbjq.cn/Article/details/guhsbjouj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.hesvh.cn/Article/details/gupkmciqo.sHtML

[G04] 定义方法
来源：http://baike.hesvh.cn/Article/details/gvuagiyor.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/gzlrsggom.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gcagaiayw.sHtML

JS:   greet() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gefhovgkd.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gykhjnvwc.sHtML

Java: String greet() { return name; }
来源：http://blog.hesvh.cn/Article/details/gghzycslq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gmnyadhkx.sHtML

Ruby: def greet; @name; end
来源：http://www.share.hesvh.cn/Article/details/gfvetyfmx.sHtML

C#:   public string Greet() => Name;
来源：http://blog.zdbjq.cn/Article/details/gejurxyll.sHtML

[G05] 继承
来源：http://www.m.share.hesvh.cn/Article/details/gthakllbs.sHtML

Py:   class Admin(User): pass
来源：http://www.share.zdbjq.cn/Article/details/gcrvwpmov.sHtML

PHP:  class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gkbdhccrq.sHtML

JS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gchpmkxaa.sHtML

TS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gdhhoyrqo.sHtML

Java: class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gmzzndmat.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.zdbjq.cn/Article/details/gxhprcyth.sHtML

Ruby: class Admin < User; end
来源：http://read.share.hesvh.cn/Article/details/gzqqknbub.sHtML

C#:   class Admin : User {}
来源：http://mobile.hesvh.cn/Article/details/guylabbnu.sHtML

[G06] 重写方法
来源：http://wap.zdbjq.cn/Article/details/gajqsnneu.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fehbvm.com/Article/details/gspaycyne.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gppmqbaxz.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gfunnfrap.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gymbssskh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gfyullpgl.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.hesvh.cn/Article/details/gxpzjkyxk.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.hesvh.cn/Article/details/gkihwnyme.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.hesvh.cn/Article/details/gbzsxutkx.sHtML

[G07] 调用父类方法
来源：http://3g.zdbjq.cn/Article/details/gzvfklqtt.sHtML

Py:   super().greet()
来源：http://wap.zdbjq.cn/Article/details/gflxglrdi.sHtML

PHP:  parent::greet();
来源：http://www.m.share.hesvh.cn/Article/details/gohcfvytj.sHtML

JS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gndveeiyv.sHtML

TS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gwcmrkubu.sHtML

Java: super.greet();
来源：http://wap.zdbjq.cn/Article/details/guvnmxzwo.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.fehbvm.com/Article/details/gocrodqhc.sHtML

Ruby: super
来源：http://m.share.fehbvm.com/Article/details/gbqwtpysr.sHtML

C#:   base.Greet();
来源：http://www.blog.hesvh.cn/Article/details/ghuxlruba.sHtML

[G08] 静态方法与属性
来源：http://www.blog.zdbjq.cn/Article/details/gavbgawwc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.zdbjq.cn/Article/details/gprylbxjl.sHtML

PHP:  public static function f() {}
来源：http://mobile.zdbjq.cn/Article/details/gtcczsxuw.sHtML

JS:   static f() {}
来源：http://m.share.zdbjq.cn/Article/details/geklcteoo.sHtML

TS:   static f(): void {}
来源：http://baike.fehbvm.com/Article/details/guhtqlvhc.sHtML

Java: static void f() {}
来源：http://wap.fehbvm.com/Article/details/gyssbcvos.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.hesvh.cn/Article/details/gbppvmffz.sHtML

Ruby: def self.f; end
来源：http://read.share.fehbvm.com/Article/details/guqoupwox.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fehbvm.com/Article/details/gmbrfuupe.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.fehbvm.com/Article/details/gxjyivrbj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.hesvh.cn/Article/details/gtckalyyh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.fehbvm.com/Article/details/gekzeiebk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.hesvh.cn/Article/details/gzbmxmgzj.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.fehbvm.com/Article/details/gamvmojme.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.zdbjq.cn/Article/details/grfagitqt.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.fehbvm.com/Article/details/gixrrxbrt.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.zdbjq.cn/Article/details/gxdhfvboy.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fehbvm.com/Article/details/gkokzldpe.sHtML

[G10] 访问控制
来源：http://www.m.share.hesvh.cn/Article/details/gzmhsinuz.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.zdbjq.cn/Article/details/ggwnbufuo.sHtML

PHP:  public / protected / private
来源：http://blog.hesvh.cn/Article/details/gbvjljeud.sHtML

JS:   #private 字段；其余公开
来源：http://3g.hesvh.cn/Article/details/geurlzxgs.sHtML

TS:   public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gpzfwoydg.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.zdbjq.cn/Article/details/gnfrycftl.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.hesvh.cn/Article/details/ghtutdlrc.sHtML

Ruby: public / protected / private
来源：http://blog.fehbvm.com/Article/details/ggthiirsy.sHtML

C#:   public / protected / private / internal
来源：http://www.share.hesvh.cn/Article/details/gpdybxhia.sHtML

[G11] getter / setter
来源：http://blog.zdbjq.cn/Article/details/ghwdbxcst.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.zdbjq.cn/Article/details/gvmejgrlq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gwdrjdrkh.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/ghnfbnzsy.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/ghtfmsmsr.sHtML

Java: public String getName() { return name; }
来源：http://blog.fehbvm.com/Article/details/gwrinatej.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gkfaejpjh.sHtML

Ruby: attr_accessor :name
来源：http://wap.zdbjq.cn/Article/details/gwkehxckl.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.zdbjq.cn/Article/details/ggfjtzzyl.sHtML

[G12] 对象转字符串
来源：http://www.blog.fehbvm.com/Article/details/gpqgtuvln.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gemkifgwp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/glrukaacd.sHtML

JS:   toString() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gkxodjldo.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gpfuudiga.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.hesvh.cn/Article/details/gmkgsywcc.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gxyjqqjxw.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.fehbvm.com/Article/details/glbvrwxll.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/grsvzaonx.sHtML

[G13] 判断对象类型
来源：http://www.blog.zdbjq.cn/Article/details/gqnlipeeb.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.hesvh.cn/Article/details/gvkjlvept.sHtML

PHP:  $u instanceof User
来源：http://wap.zdbjq.cn/Article/details/guqjbqkdx.sHtML

JS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gpyujssgq.sHtML

TS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/glumfamjo.sHtML

Java: u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gylumvzyx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.zdbjq.cn/Article/details/gehamnhnr.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.zdbjq.cn/Article/details/gripfbxsk.sHtML

C#:   u is User
来源：http://www.share.zdbjq.cn/Article/details/gqebrddtq.sHtML

[G14] 数据类 / record
来源：http://www.m.share.hesvh.cn/Article/details/gamslcfiu.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.zdbjq.cn/Article/details/gnamfvmie.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.zdbjq.cn/Article/details/gkmiiumoa.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.hesvh.cn/Article/details/gipyqdztp.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.hesvh.cn/Article/details/ghjzvmbea.sHtML

Java: record User(String name, int age) {}
来源：http://blog.hesvh.cn/Article/details/gizkdfddl.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.fehbvm.com/Article/details/gxmghqryy.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.fehbvm.com/Article/details/gwyqemkdl.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fehbvm.com/Article/details/gfrxjxgdh.sHtML

[G15] 枚举
来源：http://mobile.zdbjq.cn/Article/details/gvywlsgso.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.fehbvm.com/Article/details/gghxoiqwu.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.hesvh.cn/Article/details/gufdzlbyh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.hesvh.cn/Article/details/gnhtlwqvd.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/ggpayqpvm.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fehbvm.com/Article/details/gfnvtikka.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.fehbvm.com/Article/details/gzrqfvmqt.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.fehbvm.com/Article/details/gydfncdsk.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/gpwkexscd.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.zdbjq.cn/Article/details/gajupspde.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.hesvh.cn/Article/details/ghzygfsel.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.zdbjq.cn/Article/details/glimadjuf.sHtML

JS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gpndbejve.sHtML

TS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/gsbgtsyrr.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.fehbvm.com/Article/details/gudijifhp.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.hesvh.cn/Article/details/gjcuuskqs.sHtML

Ruby: obj.instance_variables
来源：http://3g.zdbjq.cn/Article/details/gxlevysld.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/gwzyaxxab.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ggguhxeel.sHtML

H. 异常与错误处理
来源：http://www.blog.hesvh.cn/Article/details/gwuyhuzuf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/glvfigzel.sHtML

[H01] try / catch 基础
来源：http://blog.hesvh.cn/Article/details/glzzsrgvz.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.hesvh.cn/Article/details/gzrzhaayv.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.fehbvm.com/Article/details/gvaktsdws.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gofmqdoqx.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gkclvejnc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.hesvh.cn/Article/details/gtalowcfi.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.fehbvm.com/Article/details/gxxnhyumx.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.zdbjq.cn/Article/details/gbndargmt.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.zdbjq.cn/Article/details/gwkpwjqag.sHtML

[H02] finally / ensure 收尾
来源：http://3g.hesvh.cn/Article/details/gxxijtjyu.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.zdbjq.cn/Article/details/gquhkoyke.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gpqfidaxf.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gokjgjbpe.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gcqkqecrb.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gncdtoorf.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.zdbjq.cn/Article/details/gsitzdlyy.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.zdbjq.cn/Article/details/gqvzwakgo.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gfpzokhkf.sHtML

[H03] 主动抛出异常
来源：http://wap.zdbjq.cn/Article/details/gcizmeazn.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.fehbvm.com/Article/details/ginvhujum.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gahbnhiko.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gfapwmzpq.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gjbxdyqby.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gpnrdyvqi.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.fehbvm.com/Article/details/gqxozjtut.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.fehbvm.com/Article/details/glsoalppk.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gbcvhufcb.sHtML

[H04] 自定义异常类型
来源：http://baike.zdbjq.cn/Article/details/glrklkuwj.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.fehbvm.com/Article/details/gexfezhld.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.zdbjq.cn/Article/details/grtjcypeh.sHtML

JS:   class MyError extends Error {}
来源：http://wap.hesvh.cn/Article/details/grfdjujkd.sHtML

TS:   class MyError extends Error {}
来源：http://wap.hesvh.cn/Article/details/gwwoegikr.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.fehbvm.com/Article/details/gligymaky.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.zdbjq.cn/Article/details/gnfzwgbrf.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.zdbjq.cn/Article/details/gpnfxfrix.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.fehbvm.com/Article/details/giedosvfk.sHtML

[H05] 捕获特定类型
来源：http://www.share.fehbvm.com/Article/details/gjskbnelx.sHtML

Py:   except ValueError as e:
来源：http://blog.hesvh.cn/Article/details/gobafywac.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.hesvh.cn/Article/details/gqqmakiwo.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.zdbjq.cn/Article/details/gdfelwigh.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/gdwfjzezp.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.hesvh.cn/Article/details/gdvnegyww.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.zdbjq.cn/Article/details/ggafungnl.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.zdbjq.cn/Article/details/gjxwvwmsn.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.hesvh.cn/Article/details/giidorlru.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.hesvh.cn/Article/details/glzgxosty.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.fehbvm.com/Article/details/gcgutblpv.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.fehbvm.com/Article/details/gswymrdog.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.fehbvm.com/Article/details/gyownlrrc.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/gqzccvghc.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.fehbvm.com/Article/details/gxtuaqcjg.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.zdbjq.cn/Article/details/gtdkptxjc.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.zdbjq.cn/Article/details/gpwjwczeo.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.fehbvm.com/Article/details/gpgxquihh.sHtML

[H07] 断言
来源：http://3g.zdbjq.cn/Article/details/gwmwatyas.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.zdbjq.cn/Article/details/gotincbvb.sHtML

PHP:  assert($x > 0);
来源：http://www.share.fehbvm.com/Article/details/gonfbbwyw.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gxtmpecbg.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gucvjnbqa.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.fehbvm.com/Article/details/gydmcqlhv.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.hesvh.cn/Article/details/gtqngxtsk.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.fehbvm.com/Article/details/gljvwyilx.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gvycdseqc.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.fehbvm.com/Article/details/gdyzjtlhd.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.hesvh.cn/Article/details/gstwosivt.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.zdbjq.cn/Article/details/ghtzqgvbi.sHtML

JS:   e.message;  e.stack
来源：http://read.share.hesvh.cn/Article/details/gmhrpsicn.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://read.share.fehbvm.com/Article/details/gwcztjbvl.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.fehbvm.com/Article/details/gpndsrxyc.sHtML

Go:   err.Error()
来源：http://www.m.share.fehbvm.com/Article/details/gsoymqlhj.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.hesvh.cn/Article/details/glbqgtgyc.sHtML

C#:   e.Message;  e.StackTrace
来源：http://mobile.hesvh.cn/Article/details/gsilunuky.sHtML

[H09] 带错误码的异常
来源：http://wap.zdbjq.cn/Article/details/gdswklhrm.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.fehbvm.com/Article/details/gdsbmkgdu.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://m.share.hesvh.cn/Article/details/gxonashbq.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://blog.zdbjq.cn/Article/details/gwzbwbjcy.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.m.share.hesvh.cn/Article/details/gtfvjgeiq.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.zdbjq.cn/Article/details/ggeovojvh.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.zdbjq.cn/Article/details/grhaexjjf.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.zdbjq.cn/Article/details/gerhmmvgx.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.zdbjq.cn/Article/details/gorxnatjq.sHtML

[H10] 资源自动释放
来源：http://baike.fehbvm.com/Article/details/gbplyjyuj.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.blog.zdbjq.cn/Article/details/gegwqeobq.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://blog.fehbvm.com/Article/details/ggsrckfyl.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.hesvh.cn/Article/details/ghilrgfjy.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.zdbjq.cn/Article/details/gmyzjrrtt.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.hesvh.cn/Article/details/gnhgctssm.sHtML

Go:   defer f.Close()
来源：http://m.share.fehbvm.com/Article/details/gzwyxhqof.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.fehbvm.com/Article/details/gdbsuukoy.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.hesvh.cn/Article/details/gprqlnaso.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gfyhfugqt.sHtML

I. 正则表达式
来源：http://mobile.zdbjq.cn/Article/details/gqgeyxnpc.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gwttyavdf.sHtML

[I01] 判断是否匹配
来源：http://read.share.zdbjq.cn/Article/details/gbiwpmdux.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://baike.zdbjq.cn/Article/details/gedzzmiri.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.hesvh.cn/Article/details/gckbgjbwa.sHtML

JS:   /\d+/.test(s)
来源：http://baike.hesvh.cn/Article/details/ghbynmbzn.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.fehbvm.com/Article/details/gamnfpafy.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.zdbjq.cn/Article/details/gsxxllbch.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.hesvh.cn/Article/details/ghpzcmjde.sHtML

Ruby: s.match?(/\d+/)
来源：http://wap.hesvh.cn/Article/details/gynmainsv.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.hesvh.cn/Article/details/gomhcmxsb.sHtML

[I02] 提取所有匹配
来源：http://www.share.hesvh.cn/Article/details/gdgaabknh.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.hesvh.cn/Article/details/gpvwtwvax.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://baike.hesvh.cn/Article/details/gyvywpawl.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.hesvh.cn/Article/details/gpxfmkbql.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.zdbjq.cn/Article/details/gfvcchmzc.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.fehbvm.com/Article/details/gblbvquok.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.zdbjq.cn/Article/details/gxgdgygmr.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.fehbvm.com/Article/details/givfiltyg.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://wap.zdbjq.cn/Article/details/gbamgcsvz.sHtML

[I03] 提取捕获分组
来源：http://wap.zdbjq.cn/Article/details/gcdosftny.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.zdbjq.cn/Article/details/grtfoqjxk.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://read.share.fehbvm.com/Article/details/gaximtapd.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://baike.hesvh.cn/Article/details/gyiexogcs.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.zdbjq.cn/Article/details/gcyhiugqm.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.zdbjq.cn/Article/details/gnrcjpsif.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.hesvh.cn/Article/details/giupcabgu.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gyqdoroyv.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.fehbvm.com/Article/details/grvzopdyq.sHtML

[I04] 正则替换
来源：http://www.m.share.fehbvm.com/Article/details/gmqjvptud.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://mobile.hesvh.cn/Article/details/gkxqumkpq.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://3g.fehbvm.com/Article/details/gzxmplnqs.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gukbiwdgd.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://read.share.hesvh.cn/Article/details/gqurelwsu.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.fehbvm.com/Article/details/gwggxhttg.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.fehbvm.com/Article/details/giwtrszjy.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://wap.zdbjq.cn/Article/details/gvkzjeizw.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.hesvh.cn/Article/details/gksgqcnqb.sHtML

[I05] 按正则拆分
来源：http://mobile.zdbjq.cn/Article/details/gqoyofdir.sHtML


<!-- 参考信息 -->