代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gvxaaizzf.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fehbvm.com/Article/details/geqirqjbp.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.hesvh.cn/Article/details/gyjjrfmto.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gehzhmppt.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gdrloldon.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gmxeycgxm.sHtML

[F11] 复制与移动文件
来源：http://mobile.fehbvm.com/Article/details/gfrcjdqch.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gtedtzqbw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.hesvh.cn/Article/details/gqadkkkyh.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gwobpgdnl.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gqmiibgrh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.zdbjq.cn/Article/details/gsbymsryd.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.hesvh.cn/Article/details/gqkghthwv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gcgoszfwn.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.hesvh.cn/Article/details/gwbwipjyw.sHtML

[F12] CSV 读写
来源：http://blog.hesvh.cn/Article/details/guvbstwpt.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.hesvh.cn/Article/details/gxvbpakjt.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.hesvh.cn/Article/details/gdjxrqgvm.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.zdbjq.cn/Article/details/grydpsrig.sHtML

TS:   // 同上
来源：http://www.blog.fehbvm.com/Article/details/gqqycpezp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.hesvh.cn/Article/details/gdrmczipf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.zdbjq.cn/Article/details/gpgqdcnrp.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.zdbjq.cn/Article/details/glgobnkwb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fehbvm.com/Article/details/gilhdoove.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gotyqowhl.sHtML

G. 面向对象
来源：http://www.m.share.zdbjq.cn/Article/details/gcotabafi.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/guugxexsb.sHtML

[G01] 定义类
来源：http://www.m.share.fehbvm.com/Article/details/gezlxuigg.sHtML

Py:   class User: pass
来源：http://baike.zdbjq.cn/Article/details/gpmkgqznv.sHtML

PHP:  class User {}
来源：http://blog.fehbvm.com/Article/details/goqtcmtjf.sHtML

JS:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gvmvghjxr.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.hesvh.cn/Article/details/gbaixhqfj.sHtML

Java: class User {}
来源：http://wap.hesvh.cn/Article/details/gblyrmtyq.sHtML

Go:   type User struct { Name string }
来源：http://blog.fehbvm.com/Article/details/gdccmabsy.sHtML

Ruby: class User; end
来源：http://m.share.zdbjq.cn/Article/details/gjdhizhdy.sHtML

C#:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gzozieozt.sHtML

[G02] 构造函数
来源：http://m.share.hesvh.cn/Article/details/gdiecwllg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fehbvm.com/Article/details/gquqwyjgy.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.hesvh.cn/Article/details/gxmhgxrxq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gfnmikcpx.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.hesvh.cn/Article/details/gxqpmmjpv.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gqwlazfpk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.hesvh.cn/Article/details/gechajrfb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.hesvh.cn/Article/details/gbhioyvgk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gvuziedlo.sHtML

[G03] 实例属性
来源：http://www.blog.fehbvm.com/Article/details/gectbkhbd.sHtML

Py:   self.name = "x"
来源：http://baike.hesvh.cn/Article/details/gcwgkiity.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gyqkmnscd.sHtML

JS:   this.name = "x";
来源：http://m.share.fehbvm.com/Article/details/gfakbjqdy.sHtML

TS:   name: string = "x";
来源：http://www.blog.zdbjq.cn/Article/details/goszublqe.sHtML

Java: private String name;
来源：http://mobile.fehbvm.com/Article/details/gxwwyluhf.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.hesvh.cn/Article/details/goehjqbbf.sHtML

Ruby: @name = "x"
来源：http://3g.fehbvm.com/Article/details/glrhnhreh.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.hesvh.cn/Article/details/gvmdgobsd.sHtML

[G04] 定义方法
来源：http://mobile.zdbjq.cn/Article/details/gnnwwbrmw.sHtML

Py:   def greet(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gvkhjfqmu.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gbyvuevxj.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gxpryskmm.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gibvzffbs.sHtML

Java: String greet() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gtavyvydq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gmhydhezd.sHtML

Ruby: def greet; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gtkrhizna.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gfztbojlz.sHtML

[G05] 继承
来源：http://baike.hesvh.cn/Article/details/grejoqotp.sHtML

Py:   class Admin(User): pass
来源：http://blog.fehbvm.com/Article/details/gpabuqrlt.sHtML

PHP:  class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/glxeyzogp.sHtML

JS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gqnqpkuav.sHtML

TS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gixqpzurt.sHtML

Java: class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gachkcwwz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.fehbvm.com/Article/details/gswnwwmru.sHtML

Ruby: class Admin < User; end
来源：http://mobile.hesvh.cn/Article/details/gdwwjfdps.sHtML

C#:   class Admin : User {}
来源：http://m.share.hesvh.cn/Article/details/ggxmpsica.sHtML

[G06] 重写方法
来源：http://blog.zdbjq.cn/Article/details/gfhmzcnge.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fehbvm.com/Article/details/gnlcvwzex.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gexgegkvy.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gmkxynzoz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gkjcferda.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gpjhrduqt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fehbvm.com/Article/details/gkifowask.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.hesvh.cn/Article/details/ggemgpxbd.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.fehbvm.com/Article/details/givfdhsqn.sHtML

[G07] 调用父类方法
来源：http://www.blog.fehbvm.com/Article/details/gfguogrqr.sHtML

Py:   super().greet()
来源：http://baike.zdbjq.cn/Article/details/gacovxhgz.sHtML

PHP:  parent::greet();
来源：http://blog.hesvh.cn/Article/details/gzbtczzdw.sHtML

JS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gfmyinmjd.sHtML

TS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gcalgpzxl.sHtML

Java: super.greet();
来源：http://3g.hesvh.cn/Article/details/gxjzdfqwb.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.hesvh.cn/Article/details/gdsxugtuw.sHtML

Ruby: super
来源：http://blog.zdbjq.cn/Article/details/gdxdckigv.sHtML

C#:   base.Greet();
来源：http://3g.fehbvm.com/Article/details/gqadlqgzi.sHtML

[G08] 静态方法与属性
来源：http://mobile.hesvh.cn/Article/details/guetyvabu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.fehbvm.com/Article/details/gftppalzr.sHtML

PHP:  public static function f() {}
来源：http://3g.zdbjq.cn/Article/details/gtiaymsfd.sHtML

JS:   static f() {}
来源：http://3g.zdbjq.cn/Article/details/ghagkttfv.sHtML

TS:   static f(): void {}
来源：http://read.share.zdbjq.cn/Article/details/gzwivmvus.sHtML

Java: static void f() {}
来源：http://read.share.hesvh.cn/Article/details/gonerawmm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.zdbjq.cn/Article/details/glxdkzntt.sHtML

Ruby: def self.f; end
来源：http://blog.hesvh.cn/Article/details/gtrxvwexd.sHtML

C#:   public static void F() {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggusdbvlt.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.hesvh.cn/Article/details/grlnloltp.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.hesvh.cn/Article/details/gsnwdvpjh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.zdbjq.cn/Article/details/gljywizyk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.hesvh.cn/Article/details/gamostfvp.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fehbvm.com/Article/details/gjdgwerhe.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.zdbjq.cn/Article/details/gtdpvmlsm.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.hesvh.cn/Article/details/gtrwndfle.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.hesvh.cn/Article/details/gnnnxpxrr.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gjqlbzhvy.sHtML

[G10] 访问控制
来源：http://www.m.share.fehbvm.com/Article/details/gdxosvxtl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.zdbjq.cn/Article/details/gwmxkyfpl.sHtML

PHP:  public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gdhtibhbr.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.zdbjq.cn/Article/details/grwjpvnwd.sHtML

TS:   public / protected / private
来源：http://read.share.hesvh.cn/Article/details/ghbpqxtyi.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.hesvh.cn/Article/details/gdkmkdhgq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.hesvh.cn/Article/details/gdpjiimht.sHtML

Ruby: public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gxxltxfbt.sHtML

C#:   public / protected / private / internal
来源：http://wap.hesvh.cn/Article/details/gnzbluaqc.sHtML

[G11] getter / setter
来源：http://read.share.zdbjq.cn/Article/details/gbmmppmiy.sHtML

Py:   @property 与 @x.setter
来源：http://blog.hesvh.cn/Article/details/gqlnfhzrz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gplngbqhn.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gyboexfrf.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.hesvh.cn/Article/details/gbfbilwoj.sHtML

Java: public String getName() { return name; }
来源：http://3g.hesvh.cn/Article/details/geteujrua.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gihnfzglx.sHtML

Ruby: attr_accessor :name
来源：http://baike.hesvh.cn/Article/details/gpxsnzorm.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.fehbvm.com/Article/details/gnujeoyow.sHtML

[G12] 对象转字符串
来源：http://3g.zdbjq.cn/Article/details/gezyptdzs.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gulczwtfs.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gnpghufjc.sHtML

JS:   toString() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gjrnuvhum.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gfbrkfosq.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gokkdtuur.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gisadedir.sHtML

Ruby: def to_s; @name; end
来源：http://wap.zdbjq.cn/Article/details/gcmddfbgy.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.hesvh.cn/Article/details/gjyqkvqwa.sHtML

[G13] 判断对象类型
来源：http://read.share.zdbjq.cn/Article/details/gyqgtiqwg.sHtML

Py:   isinstance(u, User)
来源：http://wap.fehbvm.com/Article/details/gnjtwexub.sHtML

PHP:  $u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gmlsjtjvw.sHtML

JS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gxnawfodj.sHtML

TS:   u instanceof User
来源：http://3g.hesvh.cn/Article/details/gdobdiler.sHtML

Java: u instanceof User
来源：http://baike.hesvh.cn/Article/details/gtglsmdjb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fehbvm.com/Article/details/gxqjgezdf.sHtML

Ruby: u.is_a?(User)
来源：http://3g.fehbvm.com/Article/details/ggjthicdx.sHtML

C#:   u is User
来源：http://wap.hesvh.cn/Article/details/gmimcmbzm.sHtML

[G14] 数据类 / record
来源：http://www.blog.zdbjq.cn/Article/details/glvlnsdyx.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.fehbvm.com/Article/details/gxfushgru.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.fehbvm.com/Article/details/gvcltrurg.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.fehbvm.com/Article/details/gemxiwofi.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.fehbvm.com/Article/details/gnoevstvv.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.hesvh.cn/Article/details/gqbeztujy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.fehbvm.com/Article/details/gcwzgletk.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.fehbvm.com/Article/details/gylzxxcjh.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fehbvm.com/Article/details/gncopiegh.sHtML

[G15] 枚举
来源：http://mobile.hesvh.cn/Article/details/gqgsqituy.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fehbvm.com/Article/details/gxmpevnki.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.hesvh.cn/Article/details/gyyflwchn.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.fehbvm.com/Article/details/gkonskqvk.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.fehbvm.com/Article/details/gvlhwitaw.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fehbvm.com/Article/details/gemqcxqkh.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.hesvh.cn/Article/details/ggwbffhqj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fehbvm.com/Article/details/gkxaudsab.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/gcnnvzcrr.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.hesvh.cn/Article/details/gvnfhpjxj.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.zdbjq.cn/Article/details/gkqucaqqk.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.zdbjq.cn/Article/details/gkoanbrmy.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/gsahyxfpn.sHtML

TS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/gkqddvzhy.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.fehbvm.com/Article/details/gcaadmsjl.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.hesvh.cn/Article/details/grkkluoil.sHtML

Ruby: obj.instance_variables
来源：http://blog.hesvh.cn/Article/details/gsncijtgt.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/gtjlqcgzp.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gfrdevjow.sHtML

H. 异常与错误处理
来源：http://wap.zdbjq.cn/Article/details/gauuryfst.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/godiveflb.sHtML

[H01] try / catch 基础
来源：http://www.m.share.fehbvm.com/Article/details/gsxczflsb.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.hesvh.cn/Article/details/gwgignyvs.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.zdbjq.cn/Article/details/gzripajio.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gaszmyaqj.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gesunpafc.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.zdbjq.cn/Article/details/gzugqwgyr.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.zdbjq.cn/Article/details/gsrcqsmyg.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.zdbjq.cn/Article/details/gcskiiqes.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.fehbvm.com/Article/details/gueaaatqf.sHtML

[H02] finally / ensure 收尾
来源：http://3g.hesvh.cn/Article/details/gthdircju.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.fehbvm.com/Article/details/grcjznoay.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gbvkqhzlr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gsroxhush.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gkensllzc.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gnmsctnrs.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.fehbvm.com/Article/details/gymlmwqdw.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.fehbvm.com/Article/details/gnachspun.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gfdzlqdvy.sHtML

[H03] 主动抛出异常
来源：http://www.share.fehbvm.com/Article/details/gwkiwqkcn.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.hesvh.cn/Article/details/gnoiotdoh.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gzzevnfqa.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gufjkkcfi.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gfcmpqihr.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/glbcqweds.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.hesvh.cn/Article/details/gikavpdfe.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.zdbjq.cn/Article/details/gjyipwqhe.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gjadrrtpc.sHtML

[H04] 自定义异常类型
来源：http://read.share.hesvh.cn/Article/details/gwzdqalgd.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.hesvh.cn/Article/details/geizlkmiq.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.fehbvm.com/Article/details/grujcmrqo.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/gnvkihlzl.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/guvtwuwfp.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/gwlwdliip.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.zdbjq.cn/Article/details/gwcjezswd.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.zdbjq.cn/Article/details/gscwpjrei.sHtML

C#:   class MyException : Exception {}
来源：http://wap.zdbjq.cn/Article/details/gdgdfpxho.sHtML

[H05] 捕获特定类型
来源：http://mobile.fehbvm.com/Article/details/gbgokrndk.sHtML

Py:   except ValueError as e:
来源：http://m.share.hesvh.cn/Article/details/gtkbzgidb.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.fehbvm.com/Article/details/gmofsqpms.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/gooioweso.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.hesvh.cn/Article/details/ghgxfgtut.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.zdbjq.cn/Article/details/gpcgbaqxi.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.hesvh.cn/Article/details/gtjiftxju.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.hesvh.cn/Article/details/gytlpeykz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.fehbvm.com/Article/details/glzobyltz.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.fehbvm.com/Article/details/ghzcczjwn.sHtML

Py:   value = d.get("k") or default
来源：http://baike.hesvh.cn/Article/details/gbtyslqne.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.fehbvm.com/Article/details/glhwzengk.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.fehbvm.com/Article/details/goxhumxrg.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/gwxyfkzrs.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.hesvh.cn/Article/details/ggthsgbwd.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.hesvh.cn/Article/details/ggtagvrrz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.fehbvm.com/Article/details/gzfqikytj.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.zdbjq.cn/Article/details/gjrozmkhp.sHtML

[H07] 断言
来源：http://blog.fehbvm.com/Article/details/ggaykqvce.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.zdbjq.cn/Article/details/grtxuzioy.sHtML

PHP:  assert($x > 0);
来源：http://m.share.fehbvm.com/Article/details/grtebbdfe.sHtML

JS:   console.assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gwszpghfz.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/girpxrmxn.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.zdbjq.cn/Article/details/grkuugkfp.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.fehbvm.com/Article/details/gyuzhowfz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.hesvh.cn/Article/details/grzlszggl.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gmvvcucfi.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.fehbvm.com/Article/details/gshqghbty.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.hesvh.cn/Article/details/gpkrvfufe.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.fehbvm.com/Article/details/ghbiftnkh.sHtML

JS:   e.message;  e.stack
来源：http://www.share.fehbvm.com/Article/details/gghiwuevw.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://m.share.hesvh.cn/Article/details/gcmjdjpjl.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.fehbvm.com/Article/details/gjctdecia.sHtML

Go:   err.Error()
来源：http://baike.hesvh.cn/Article/details/gndkatesk.sHtML

Ruby: e.message;  e.backtrace
来源：http://read.share.fehbvm.com/Article/details/glhrxkuan.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.fehbvm.com/Article/details/gcxcwwghd.sHtML

[H09] 带错误码的异常
来源：http://www.share.zdbjq.cn/Article/details/gscseiduf.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://baike.zdbjq.cn/Article/details/gkgtfkdik.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.zdbjq.cn/Article/details/gtsszusbi.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.fehbvm.com/Article/details/goeihrqix.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.zdbjq.cn/Article/details/gucfzioly.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://baike.hesvh.cn/Article/details/gnklkxftb.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.hesvh.cn/Article/details/gdbtdayec.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://baike.fehbvm.com/Article/details/ggravdelm.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://m.share.fehbvm.com/Article/details/gumutjazb.sHtML

[H10] 资源自动释放
来源：http://baike.fehbvm.com/Article/details/gkfprpzwn.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.zdbjq.cn/Article/details/gdhnrxghh.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.zdbjq.cn/Article/details/gncohdoop.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fehbvm.com/Article/details/gqrahpflm.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.fehbvm.com/Article/details/gsqljmkxf.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.fehbvm.com/Article/details/gigztzsdy.sHtML

Go:   defer f.Close()
来源：http://www.m.share.zdbjq.cn/Article/details/gndkpttzs.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://blog.hesvh.cn/Article/details/ghqggmkug.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.fehbvm.com/Article/details/gghqqczsr.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ggkibudtv.sHtML

I. 正则表达式
来源：http://baike.fehbvm.com/Article/details/gijjconwj.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbmnqfrin.sHtML

[I01] 判断是否匹配
来源：http://www.m.share.zdbjq.cn/Article/details/goffjxtao.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.blog.zdbjq.cn/Article/details/ginnnsxxl.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/giyodacwe.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.fehbvm.com/Article/details/gdpprotei.sHtML

TS:   /\d+/.test(s)
来源：http://m.share.fehbvm.com/Article/details/grjqumcei.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.fehbvm.com/Article/details/gvjbnkqbs.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.zdbjq.cn/Article/details/gqhaoijep.sHtML

Ruby: s.match?(/\d+/)
来源：http://read.share.fehbvm.com/Article/details/gthuaimii.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://read.share.zdbjq.cn/Article/details/gyrplvgsu.sHtML

[I02] 提取所有匹配
来源：http://read.share.zdbjq.cn/Article/details/gednezmhy.sHtML

Py:   re.findall(r"\d+", s)
来源：http://mobile.zdbjq.cn/Article/details/gdobhbjlm.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://blog.hesvh.cn/Article/details/glbwyprxa.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://3g.zdbjq.cn/Article/details/gcvzpgjan.sHtML

TS:   s.match(/\d+/g)
来源：http://mobile.fehbvm.com/Article/details/glmimtpib.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.zdbjq.cn/Article/details/goczmdgqh.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.hesvh.cn/Article/details/gebrrscuj.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.fehbvm.com/Article/details/gkoavjmpb.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://baike.hesvh.cn/Article/details/gmgbbtava.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.fehbvm.com/Article/details/gkzhmauys.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://mobile.fehbvm.com/Article/details/gdxuemnyc.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.blog.fehbvm.com/Article/details/ggagfugeo.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.zdbjq.cn/Article/details/gdafljifw.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wap.zdbjq.cn/Article/details/gqbycfoos.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.m.share.fehbvm.com/Article/details/gnvtsmcgs.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.hesvh.cn/Article/details/gprffzfzf.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://baike.fehbvm.com/Article/details/goxwlgryc.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.hesvh.cn/Article/details/gbfquudmh.sHtML

[I04] 正则替换
来源：http://read.share.zdbjq.cn/Article/details/gecytalty.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gyeuyiyyh.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.zdbjq.cn/Article/details/gioivcgia.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://blog.fehbvm.com/Article/details/gclwneoae.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.blog.fehbvm.com/Article/details/gelupchur.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.hesvh.cn/Article/details/gtpzzjfbl.sHtML


<!-- 参考信息 -->