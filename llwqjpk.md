代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gyjyoilba.sHtML

TS:   path.extname("a.txt")
来源：http://blog.hesvh.cn/Article/details/gorereuit.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fehbvm.com/Article/details/gvrefpgag.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gbidtikwa.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gbrlxwzzy.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gvqhmgpkb.sHtML

[F11] 复制与移动文件
来源：http://www.blog.hesvh.cn/Article/details/gxushgpnq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/grwuncqzf.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gzlxbzbrj.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gmpsipsls.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gykvxhmtc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gexwovyfr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.zdbjq.cn/Article/details/gbrcxtaqb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gdtezspwy.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.hesvh.cn/Article/details/gqvxdpwxj.sHtML

[F12] CSV 读写
来源：http://www.blog.fehbvm.com/Article/details/gkpsfvaxl.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.hesvh.cn/Article/details/gqslhrmcz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.hesvh.cn/Article/details/gddtvzcus.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.fehbvm.com/Article/details/gelqzsrwo.sHtML

TS:   // 同上
来源：http://read.share.hesvh.cn/Article/details/gvlzmlnwe.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.fehbvm.com/Article/details/gukaxadox.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.fehbvm.com/Article/details/gdjjkuvbg.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.zdbjq.cn/Article/details/gwuoiyssr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.zdbjq.cn/Article/details/gmzqpmisp.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmzlbswtx.sHtML

G. 面向对象
来源：http://read.share.fehbvm.com/Article/details/gexapqbzp.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/geqqetdzs.sHtML

[G01] 定义类
来源：http://www.share.hesvh.cn/Article/details/gegdpehee.sHtML

Py:   class User: pass
来源：http://www.m.share.zdbjq.cn/Article/details/gimyxixhw.sHtML

PHP:  class User {}
来源：http://blog.hesvh.cn/Article/details/geztzjjrw.sHtML

JS:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/geoutkarh.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.hesvh.cn/Article/details/grizzcehd.sHtML

Java: class User {}
来源：http://www.share.zdbjq.cn/Article/details/gdxmqpesk.sHtML

Go:   type User struct { Name string }
来源：http://read.share.zdbjq.cn/Article/details/gnyxqogxi.sHtML

Ruby: class User; end
来源：http://blog.fehbvm.com/Article/details/gtaklfxgd.sHtML

C#:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gcspikwfn.sHtML

[G02] 构造函数
来源：http://mobile.hesvh.cn/Article/details/gllnrsrhh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/gdmufhgzq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.zdbjq.cn/Article/details/gcdcpxiqh.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/gclxptmjy.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.hesvh.cn/Article/details/gptpwgvbi.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/gzxbvqwzv.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fehbvm.com/Article/details/gynfexgoe.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.hesvh.cn/Article/details/gruwagckl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.fehbvm.com/Article/details/gqkdxumfb.sHtML

[G03] 实例属性
来源：http://3g.zdbjq.cn/Article/details/gjfmrjvyx.sHtML

Py:   self.name = "x"
来源：http://mobile.hesvh.cn/Article/details/grydjxumd.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gpmlctqst.sHtML

JS:   this.name = "x";
来源：http://www.share.hesvh.cn/Article/details/gfxguxjzn.sHtML

TS:   name: string = "x";
来源：http://www.blog.fehbvm.com/Article/details/glyhalxqc.sHtML

Java: private String name;
来源：http://wap.fehbvm.com/Article/details/gsjffrztm.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.hesvh.cn/Article/details/gaoaiqqnw.sHtML

Ruby: @name = "x"
来源：http://blog.fehbvm.com/Article/details/gmdzjhfnz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/guynpdlzx.sHtML

[G04] 定义方法
来源：http://www.blog.hesvh.cn/Article/details/gpdwvdczg.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gmavqqolb.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gsjorfdop.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gzqruaedn.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gvzutnkdj.sHtML

Java: String greet() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gbljgvnxt.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/ginxfbqst.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fehbvm.com/Article/details/gqkryufqr.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.fehbvm.com/Article/details/gpchwogtk.sHtML

[G05] 继承
来源：http://read.share.hesvh.cn/Article/details/gsnpchfkg.sHtML

Py:   class Admin(User): pass
来源：http://mobile.zdbjq.cn/Article/details/gbbnqhrwu.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/grmhgbmuz.sHtML

JS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gbpnpusju.sHtML

TS:   class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gjygfrpwr.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/grmxntzqe.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fehbvm.com/Article/details/gjzpokpik.sHtML

Ruby: class Admin < User; end
来源：http://m.share.fehbvm.com/Article/details/gtsobprdn.sHtML

C#:   class Admin : User {}
来源：http://m.share.zdbjq.cn/Article/details/grpvoyqjt.sHtML

[G06] 重写方法
来源：http://www.m.share.fehbvm.com/Article/details/glgsxctxo.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.fehbvm.com/Article/details/goovkmuwq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gigdscymk.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gzjjrluck.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gffcpxoqr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/ggaafqvmb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fehbvm.com/Article/details/gdfocpbup.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.zdbjq.cn/Article/details/gqyoxybtc.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.hesvh.cn/Article/details/gqknbbtxr.sHtML

[G07] 调用父类方法
来源：http://mobile.fehbvm.com/Article/details/gtcxodtdt.sHtML

Py:   super().greet()
来源：http://read.share.fehbvm.com/Article/details/ghfskhoyl.sHtML

PHP:  parent::greet();
来源：http://3g.zdbjq.cn/Article/details/glwsykpva.sHtML

JS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gcgejlnbf.sHtML

TS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gfhatvleg.sHtML

Java: super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gsuqovxll.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.fehbvm.com/Article/details/gbnmiesmq.sHtML

Ruby: super
来源：http://mobile.fehbvm.com/Article/details/gkmkekovh.sHtML

C#:   base.Greet();
来源：http://blog.fehbvm.com/Article/details/gwtxsuvbm.sHtML

[G08] 静态方法与属性
来源：http://mobile.fehbvm.com/Article/details/ggcwijdxm.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.zdbjq.cn/Article/details/gynulgcxh.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gkrhjentc.sHtML

JS:   static f() {}
来源：http://blog.zdbjq.cn/Article/details/gavzgmjrb.sHtML

TS:   static f(): void {}
来源：http://www.blog.zdbjq.cn/Article/details/gmumybwrh.sHtML

Java: static void f() {}
来源：http://read.share.zdbjq.cn/Article/details/gozrctlix.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.zdbjq.cn/Article/details/gvjehzswb.sHtML

Ruby: def self.f; end
来源：http://www.share.zdbjq.cn/Article/details/guorsuyls.sHtML

C#:   public static void F() {}
来源：http://wap.fehbvm.com/Article/details/ggtkmjgha.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.zdbjq.cn/Article/details/grtngades.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.zdbjq.cn/Article/details/gaozlkrjt.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbnddrxnd.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.fehbvm.com/Article/details/gtkqkfkdt.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.hesvh.cn/Article/details/gsgykkjsh.sHtML

Java: interface Shape { double area(); }
来源：http://blog.zdbjq.cn/Article/details/gawxfblsp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.hesvh.cn/Article/details/gzyjixywc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.fehbvm.com/Article/details/gmwipiksa.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.fehbvm.com/Article/details/gomnzvkjs.sHtML

[G10] 访问控制
来源：http://3g.zdbjq.cn/Article/details/gszjyohuo.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.zdbjq.cn/Article/details/gtwwighot.sHtML

PHP:  public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gylvuwvhj.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.hesvh.cn/Article/details/gcyujlazq.sHtML

TS:   public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gyixarqbl.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.zdbjq.cn/Article/details/gzazyhxkt.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.zdbjq.cn/Article/details/gdkatmuef.sHtML

Ruby: public / protected / private
来源：http://m.share.hesvh.cn/Article/details/ghongspdq.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.hesvh.cn/Article/details/gciujkvag.sHtML

[G11] getter / setter
来源：http://wap.zdbjq.cn/Article/details/govetsjes.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fehbvm.com/Article/details/gqvphagkr.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/grntszcyu.sHtML

JS:   get name() { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gwzucjsmb.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.hesvh.cn/Article/details/gaztpudmh.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gnnpgsyed.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gjgpjjnfu.sHtML

Ruby: attr_accessor :name
来源：http://3g.zdbjq.cn/Article/details/gbbxfndrm.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.fehbvm.com/Article/details/gdxpfkwci.sHtML

[G12] 对象转字符串
来源：http://mobile.fehbvm.com/Article/details/gyrnwwhlx.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gjqbrsfxu.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/giktayixt.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gjnejdedf.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gynkbhqhc.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gceqyalcy.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/guzxpuigz.sHtML

Ruby: def to_s; @name; end
来源：http://3g.hesvh.cn/Article/details/gznmpyckm.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.hesvh.cn/Article/details/gspzprmxt.sHtML

[G13] 判断对象类型
来源：http://www.share.hesvh.cn/Article/details/gdjcjcupu.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fehbvm.com/Article/details/gixoroarv.sHtML

PHP:  $u instanceof User
来源：http://baike.hesvh.cn/Article/details/gvwohpctq.sHtML

JS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/gwoxcnxtv.sHtML

TS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gwjbbijta.sHtML

Java: u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gowkxnocu.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fehbvm.com/Article/details/gzwoksipu.sHtML

Ruby: u.is_a?(User)
来源：http://wap.zdbjq.cn/Article/details/gdkotakao.sHtML

C#:   u is User
来源：http://wap.hesvh.cn/Article/details/gqctjjyaz.sHtML

[G14] 数据类 / record
来源：http://read.share.hesvh.cn/Article/details/gbjcquswa.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.zdbjq.cn/Article/details/gemblxdxi.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.hesvh.cn/Article/details/gvhdvnrpl.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fehbvm.com/Article/details/ghlrwnimm.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.zdbjq.cn/Article/details/gfjnvcwiv.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gkcyyeudy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.hesvh.cn/Article/details/gwiyumehs.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.fehbvm.com/Article/details/gkaeqnagk.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.zdbjq.cn/Article/details/gfldqylkj.sHtML

[G15] 枚举
来源：http://blog.hesvh.cn/Article/details/grwmvqruc.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.zdbjq.cn/Article/details/gzjeitsih.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.hesvh.cn/Article/details/gzjfufsna.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.hesvh.cn/Article/details/gypvvuelu.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gwpqjxklm.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.fehbvm.com/Article/details/grshdxzgp.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.hesvh.cn/Article/details/glgafmxes.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.hesvh.cn/Article/details/guhuojrnr.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/glmwrymhb.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.hesvh.cn/Article/details/gvtgjatso.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.fehbvm.com/Article/details/gzbccklho.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.zdbjq.cn/Article/details/ggdffbivu.sHtML

JS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/gaggwkyzj.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gqnhvwotw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.zdbjq.cn/Article/details/ggwjfnhkz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.zdbjq.cn/Article/details/gzxwoajsy.sHtML

Ruby: obj.instance_variables
来源：http://m.share.fehbvm.com/Article/details/gvntblihv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.zdbjq.cn/Article/details/gnenbvzwl.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gtoydzqwx.sHtML

H. 异常与错误处理
来源：http://www.blog.hesvh.cn/Article/details/gtkqbdmhn.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gcoxvuuos.sHtML

[H01] try / catch 基础
来源：http://read.share.hesvh.cn/Article/details/gkohxavle.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.zdbjq.cn/Article/details/gkugdpisi.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.fehbvm.com/Article/details/gmyqcjkia.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gyotntvca.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gbilxsjhz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.hesvh.cn/Article/details/gauxjosfa.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.hesvh.cn/Article/details/ghgeamkeh.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.zdbjq.cn/Article/details/gnipclrte.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.fehbvm.com/Article/details/gtimqwoxs.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.hesvh.cn/Article/details/gxtodwtsm.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.zdbjq.cn/Article/details/gvthdnxku.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gpfgtkpdz.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gdvohcyfv.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gntmcxfet.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/ggzhmjhuz.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.hesvh.cn/Article/details/giqincodw.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.hesvh.cn/Article/details/gjvychpvf.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gzbuhzelk.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/gndkzghpu.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.zdbjq.cn/Article/details/gqkqyauxp.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gecapcoeg.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/givbdxfbs.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gizeopntt.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gyqyehopq.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.hesvh.cn/Article/details/gmhqbzfne.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.fehbvm.com/Article/details/gvoutuwdt.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gqpxuzcag.sHtML

[H04] 自定义异常类型
来源：http://3g.zdbjq.cn/Article/details/ghruibtdg.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.zdbjq.cn/Article/details/gsmfkpaxz.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.fehbvm.com/Article/details/gousuzedd.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.hesvh.cn/Article/details/gzwxgsagi.sHtML

TS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/gqfcvzssm.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.hesvh.cn/Article/details/gxxcxupvw.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.zdbjq.cn/Article/details/gltskhdzv.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.zdbjq.cn/Article/details/gxbbgsuyr.sHtML

C#:   class MyException : Exception {}
来源：http://blog.hesvh.cn/Article/details/gqfmmhvit.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.hesvh.cn/Article/details/gwzvqoxcn.sHtML

Py:   except ValueError as e:
来源：http://www.share.hesvh.cn/Article/details/gcwxeucnb.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.hesvh.cn/Article/details/gltmwxnjo.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.fehbvm.com/Article/details/gzjbrlmmq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/gnuffhyjq.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.hesvh.cn/Article/details/grnnqmkrw.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.fehbvm.com/Article/details/gcnarqlja.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.zdbjq.cn/Article/details/glxdwkkpk.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.fehbvm.com/Article/details/gxnsayckp.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.hesvh.cn/Article/details/ghbdkklam.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.fehbvm.com/Article/details/ggccsjwms.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/gxzzqzwvj.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/gujzcyvzr.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.fehbvm.com/Article/details/gifhgslrb.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.zdbjq.cn/Article/details/gzmjgshig.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.hesvh.cn/Article/details/ghrohujzl.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.fehbvm.com/Article/details/gujknepnc.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.hesvh.cn/Article/details/grlnsfuay.sHtML

[H07] 断言
来源：http://mobile.hesvh.cn/Article/details/ggrwpnzjp.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.hesvh.cn/Article/details/gbhudgoub.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.fehbvm.com/Article/details/ghiuliybq.sHtML

JS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gnuaeyhhu.sHtML

TS:   console.assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gdifcazlo.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.fehbvm.com/Article/details/guxvisnyz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.zdbjq.cn/Article/details/gkloqughk.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.fehbvm.com/Article/details/ghodeelva.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.fehbvm.com/Article/details/gtusdkvix.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.fehbvm.com/Article/details/gyvpkuhsk.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.zdbjq.cn/Article/details/gtgpycfuu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.zdbjq.cn/Article/details/gwnuhnhhf.sHtML

JS:   e.message;  e.stack
来源：http://3g.fehbvm.com/Article/details/godlktrrj.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.fehbvm.com/Article/details/goczetlsx.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.hesvh.cn/Article/details/gafdanpqr.sHtML

Go:   err.Error()
来源：http://blog.zdbjq.cn/Article/details/ghycvalyb.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.blog.fehbvm.com/Article/details/gkgiuclsu.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.fehbvm.com/Article/details/guirurskg.sHtML

[H09] 带错误码的异常
来源：http://blog.fehbvm.com/Article/details/glzmyuami.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.blog.fehbvm.com/Article/details/gxbiqnabe.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.share.hesvh.cn/Article/details/gmrdgvhog.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://m.share.fehbvm.com/Article/details/guwipvmfn.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.hesvh.cn/Article/details/gzvqiodex.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.fehbvm.com/Article/details/gxejxslsj.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://blog.fehbvm.com/Article/details/gtlmdcbxq.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.hesvh.cn/Article/details/gqazoebgd.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.hesvh.cn/Article/details/gpnrggyii.sHtML

[H10] 资源自动释放
来源：http://wap.hesvh.cn/Article/details/gzlifalnu.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://m.share.zdbjq.cn/Article/details/gekjmutmn.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://wap.fehbvm.com/Article/details/gaphlxmkn.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.zdbjq.cn/Article/details/gxsyblhgq.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.zdbjq.cn/Article/details/gyvblafvo.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.m.share.fehbvm.com/Article/details/gtzmybujl.sHtML

Go:   defer f.Close()
来源：http://wap.hesvh.cn/Article/details/gsjmgfnjp.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.fehbvm.com/Article/details/ghkdlwjzs.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://baike.zdbjq.cn/Article/details/ggpiqolzx.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggixzlqkr.sHtML

I. 正则表达式
来源：http://mobile.fehbvm.com/Article/details/gcsuyoaos.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gzgfujpgi.sHtML

[I01] 判断是否匹配
来源：http://m.share.hesvh.cn/Article/details/giajgezyk.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.fehbvm.com/Article/details/gxyaanlwh.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://blog.zdbjq.cn/Article/details/gkojumfte.sHtML

JS:   /\d+/.test(s)
来源：http://m.share.fehbvm.com/Article/details/gxsdptxvw.sHtML

TS:   /\d+/.test(s)
来源：http://wap.zdbjq.cn/Article/details/glkodfttz.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.blog.fehbvm.com/Article/details/gktvqeova.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://wap.hesvh.cn/Article/details/glxjormyy.sHtML

Ruby: s.match?(/\d+/)
来源：http://m.share.fehbvm.com/Article/details/gexguzxep.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.fehbvm.com/Article/details/gwtfyjozl.sHtML

[I02] 提取所有匹配
来源：http://mobile.fehbvm.com/Article/details/gsxmupbge.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.zdbjq.cn/Article/details/gninnmhax.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://mobile.zdbjq.cn/Article/details/gxkirokrw.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wap.fehbvm.com/Article/details/gmicrwrul.sHtML

TS:   s.match(/\d+/g)
来源：http://wap.hesvh.cn/Article/details/gjnxktyth.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.hesvh.cn/Article/details/gmeauobsw.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.fehbvm.com/Article/details/gkfhysfeh.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.blog.zdbjq.cn/Article/details/gbcvoufsv.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/glgothbwm.sHtML

[I03] 提取捕获分组
来源：http://blog.fehbvm.com/Article/details/gennpcjuh.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.zdbjq.cn/Article/details/gfyemxepz.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://3g.hesvh.cn/Article/details/griolreyv.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.zdbjq.cn/Article/details/ggspwjqub.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.fehbvm.com/Article/details/gyckaicch.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.zdbjq.cn/Article/details/gqgajfbse.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.zdbjq.cn/Article/details/gatlghfhd.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.fehbvm.com/Article/details/ggygnuvwz.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.zdbjq.cn/Article/details/grikuyasg.sHtML

[I04] 正则替换
来源：http://baike.hesvh.cn/Article/details/gavzdcyvd.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://read.share.zdbjq.cn/Article/details/gwwdyjaqn.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gxnqxdidp.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://mobile.hesvh.cn/Article/details/gduntnsau.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://3g.hesvh.cn/Article/details/gitvzlekd.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.fehbvm.com/Article/details/gjjefeajb.sHtML


<!-- 参考信息 -->