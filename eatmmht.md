代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gvueehrzn.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gzftlnzvg.sHtML

[F11] 复制与移动文件
来源：http://m.share.fehbvm.com/Article/details/giaecyljj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gohkqtcdn.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.zdbjq.cn/Article/details/gqkbakeen.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/ghtyallxn.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/glrtknesp.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.hesvh.cn/Article/details/gjsyzvdbo.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.hesvh.cn/Article/details/ggotdejtj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gkppzriju.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.zdbjq.cn/Article/details/gveksbcqv.sHtML

[F12] CSV 读写
来源：http://www.m.share.zdbjq.cn/Article/details/gxdyjkevj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.fehbvm.com/Article/details/gycpcnrbg.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.hesvh.cn/Article/details/gsiifnzkh.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.fehbvm.com/Article/details/gnavpbtgn.sHtML

TS:   // 同上
来源：http://3g.fehbvm.com/Article/details/grbmpcpit.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.zdbjq.cn/Article/details/gjabrceui.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.fehbvm.com/Article/details/ggemrqwun.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.hesvh.cn/Article/details/glokqdxft.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fehbvm.com/Article/details/gfoaxbjug.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqxsabslg.sHtML

G. 面向对象
来源：http://www.blog.zdbjq.cn/Article/details/gybbdcunl.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gtkohghoq.sHtML

[G01] 定义类
来源：http://mobile.zdbjq.cn/Article/details/gztesnclv.sHtML

Py:   class User: pass
来源：http://wap.zdbjq.cn/Article/details/gbpgxkfcz.sHtML

PHP:  class User {}
来源：http://m.share.zdbjq.cn/Article/details/gktpendlz.sHtML

JS:   class User {}
来源：http://wap.zdbjq.cn/Article/details/ggtzskisi.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.zdbjq.cn/Article/details/gacivwmum.sHtML

Java: class User {}
来源：http://blog.fehbvm.com/Article/details/gsguhquyh.sHtML

Go:   type User struct { Name string }
来源：http://read.share.hesvh.cn/Article/details/gxzufptyk.sHtML

Ruby: class User; end
来源：http://baike.fehbvm.com/Article/details/gnzpjqmpe.sHtML

C#:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gcguisstu.sHtML

[G02] 构造函数
来源：http://www.m.share.fehbvm.com/Article/details/ghjdbxzfu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.zdbjq.cn/Article/details/ggeaqrout.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.hesvh.cn/Article/details/gladzhnjv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gzglopaaq.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.hesvh.cn/Article/details/gzthmtifv.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/ggdukkpog.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.zdbjq.cn/Article/details/gvndhwopw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fehbvm.com/Article/details/gaogivkmw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.fehbvm.com/Article/details/gujxefcay.sHtML

[G03] 实例属性
来源：http://wap.fehbvm.com/Article/details/gsoqdnzcv.sHtML

Py:   self.name = "x"
来源：http://3g.fehbvm.com/Article/details/gkfxdujbj.sHtML

PHP:  public string $name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gkjesydli.sHtML

JS:   this.name = "x";
来源：http://m.share.fehbvm.com/Article/details/gkhsuvgdf.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/gldvxdnmm.sHtML

Java: private String name;
来源：http://wap.hesvh.cn/Article/details/gbjqhvmzo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fehbvm.com/Article/details/gijskoity.sHtML

Ruby: @name = "x"
来源：http://baike.fehbvm.com/Article/details/ghvzotxqh.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.zdbjq.cn/Article/details/gyfasfvwa.sHtML

[G04] 定义方法
来源：http://www.blog.hesvh.cn/Article/details/ggevifyei.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/ggerknaba.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gcwslnyow.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gigojdsni.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gkhhlneug.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnmrghfij.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gasyzgbhl.sHtML

Ruby: def greet; @name; end
来源：http://m.share.hesvh.cn/Article/details/gcdlbzedc.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.hesvh.cn/Article/details/ggbauwmca.sHtML

[G05] 继承
来源：http://baike.zdbjq.cn/Article/details/gmafvjxih.sHtML

Py:   class Admin(User): pass
来源：http://baike.zdbjq.cn/Article/details/gzapfzpiq.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gtjmbalmm.sHtML

JS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gpnnfaxwe.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gwvoptxpq.sHtML

Java: class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gdrwkcqwp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.hesvh.cn/Article/details/gfifyxgmh.sHtML

Ruby: class Admin < User; end
来源：http://3g.fehbvm.com/Article/details/gdudhgxqs.sHtML

C#:   class Admin : User {}
来源：http://mobile.hesvh.cn/Article/details/gwsuvusll.sHtML

[G06] 重写方法
来源：http://blog.fehbvm.com/Article/details/gwfriqmvv.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.hesvh.cn/Article/details/gruarossh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gdsdhdtpv.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gxtgbsqnz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gawtlxvak.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gwthqomes.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.hesvh.cn/Article/details/gikdkrevc.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.hesvh.cn/Article/details/gpenzocxa.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fehbvm.com/Article/details/ghqrljuxo.sHtML

[G07] 调用父类方法
来源：http://baike.hesvh.cn/Article/details/gxvhnzjez.sHtML

Py:   super().greet()
来源：http://read.share.fehbvm.com/Article/details/gknmmrvad.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fehbvm.com/Article/details/giufvtnhw.sHtML

JS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gvvpdtsaa.sHtML

TS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/ghkghlpsa.sHtML

Java: super.greet();
来源：http://blog.fehbvm.com/Article/details/ghryrvapx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.zdbjq.cn/Article/details/gtvtnbaca.sHtML

Ruby: super
来源：http://baike.fehbvm.com/Article/details/gaajjhqol.sHtML

C#:   base.Greet();
来源：http://3g.zdbjq.cn/Article/details/gneiiaqkp.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.hesvh.cn/Article/details/gdchnvzyv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.zdbjq.cn/Article/details/gcmnvmhag.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fehbvm.com/Article/details/gacpnofba.sHtML

JS:   static f() {}
来源：http://baike.fehbvm.com/Article/details/glczgtujk.sHtML

TS:   static f(): void {}
来源：http://3g.fehbvm.com/Article/details/grkzltxai.sHtML

Java: static void f() {}
来源：http://read.share.fehbvm.com/Article/details/gwrtlynhb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.hesvh.cn/Article/details/gbgjnzybk.sHtML

Ruby: def self.f; end
来源：http://blog.hesvh.cn/Article/details/gmxwzuhgq.sHtML

C#:   public static void F() {}
来源：http://mobile.fehbvm.com/Article/details/golpawohf.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.fehbvm.com/Article/details/gpfztungq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.fehbvm.com/Article/details/glfbjezem.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.hesvh.cn/Article/details/gjaxgzpae.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.zdbjq.cn/Article/details/gfolfxaqz.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fehbvm.com/Article/details/gxsskjxwr.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.hesvh.cn/Article/details/gibhbisbr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fehbvm.com/Article/details/gpbnpcdim.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.hesvh.cn/Article/details/gwneanddu.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.zdbjq.cn/Article/details/gurtwebhu.sHtML

[G10] 访问控制
来源：http://www.blog.hesvh.cn/Article/details/ggpjnfufq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.zdbjq.cn/Article/details/gthjtdaav.sHtML

PHP:  public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gqdydcbmn.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.zdbjq.cn/Article/details/gqfaoyaqk.sHtML

TS:   public / protected / private
来源：http://blog.hesvh.cn/Article/details/gdcoecqzv.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.hesvh.cn/Article/details/ghqqdxpme.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.zdbjq.cn/Article/details/gtdlejmsh.sHtML

Ruby: public / protected / private
来源：http://wap.fehbvm.com/Article/details/gdrmbgxre.sHtML

C#:   public / protected / private / internal
来源：http://mobile.zdbjq.cn/Article/details/gcymwmxbc.sHtML

[G11] getter / setter
来源：http://blog.fehbvm.com/Article/details/gpdxfwmtq.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.zdbjq.cn/Article/details/gbadtlpts.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gmgdnvnyl.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gtjyajcfl.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/guwcacoux.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gktnxfsgr.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gdljmcnzg.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.fehbvm.com/Article/details/gnvrpbggx.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.hesvh.cn/Article/details/ghuacfykb.sHtML

[G12] 对象转字符串
来源：http://www.blog.hesvh.cn/Article/details/gvyxbziih.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gqyusonfj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gtmlgoheb.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/glsjsejiy.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/grbgblgwn.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/giwggvkud.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gmyehdfrv.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fehbvm.com/Article/details/ggkspbhzk.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gmvkcmlwf.sHtML

[G13] 判断对象类型
来源：http://www.share.zdbjq.cn/Article/details/geabblknj.sHtML

Py:   isinstance(u, User)
来源：http://blog.hesvh.cn/Article/details/gpkbozobi.sHtML

PHP:  $u instanceof User
来源：http://3g.hesvh.cn/Article/details/gegygaihk.sHtML

JS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gmepvhypm.sHtML

TS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gkohzqxrq.sHtML

Java: u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gdillcolp.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.fehbvm.com/Article/details/gukgwrxrr.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.zdbjq.cn/Article/details/gihbhhves.sHtML

C#:   u is User
来源：http://www.blog.fehbvm.com/Article/details/gadoqbrco.sHtML

[G14] 数据类 / record
来源：http://3g.fehbvm.com/Article/details/geeygfxse.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.hesvh.cn/Article/details/gzxicldxp.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.fehbvm.com/Article/details/gjnigurwr.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.hesvh.cn/Article/details/gldibyiwa.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.fehbvm.com/Article/details/gvtskvqhk.sHtML

Java: record User(String name, int age) {}
来源：http://blog.hesvh.cn/Article/details/gbrffmlmq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.hesvh.cn/Article/details/gfjlbbkyl.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.hesvh.cn/Article/details/gqpadyrar.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.zdbjq.cn/Article/details/gcopszpro.sHtML

[G15] 枚举
来源：http://www.blog.fehbvm.com/Article/details/gllmwtfqd.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.hesvh.cn/Article/details/gvbdwqfnx.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.m.share.fehbvm.com/Article/details/gcakmbqqp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.zdbjq.cn/Article/details/gesldapyw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/glyyijrte.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.hesvh.cn/Article/details/gfwtjpyfi.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.fehbvm.com/Article/details/gkjailtqw.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fehbvm.com/Article/details/ghxfxezgh.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/gzjxacoar.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.zdbjq.cn/Article/details/guunjjhoy.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.hesvh.cn/Article/details/gtkctugqk.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.zdbjq.cn/Article/details/gfgyomhuo.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.fehbvm.com/Article/details/gedalyxip.sHtML

TS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/goaxahbey.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.fehbvm.com/Article/details/ggehtljev.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.fehbvm.com/Article/details/gaqzsvmbf.sHtML

Ruby: obj.instance_variables
来源：http://blog.hesvh.cn/Article/details/gctacqndb.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.hesvh.cn/Article/details/gznmfmmri.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gnvmianqp.sHtML

H. 异常与错误处理
来源：http://read.share.zdbjq.cn/Article/details/gyztldetg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxswsyqdl.sHtML

[H01] try / catch 基础
来源：http://3g.zdbjq.cn/Article/details/godquizge.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.fehbvm.com/Article/details/gzvwoaema.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.zdbjq.cn/Article/details/gytdrorva.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/grxrnxmgn.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.fehbvm.com/Article/details/ghoraksdk.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.hesvh.cn/Article/details/gepftuolk.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.fehbvm.com/Article/details/goyotbofp.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.zdbjq.cn/Article/details/glhujszzm.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.zdbjq.cn/Article/details/gfxptqpru.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.fehbvm.com/Article/details/gwmhkrvvr.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.zdbjq.cn/Article/details/gujcdklnp.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gmazyhtro.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gcmsfgimj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gbyqrcahf.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/grbjzojkm.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.zdbjq.cn/Article/details/gcuwjioxf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.hesvh.cn/Article/details/gxkeitidt.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gzhezfqpd.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/gzvhvrqnq.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.zdbjq.cn/Article/details/gnmecjqkv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/genkbwobj.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/ghzjlsqoy.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/gmazqyeyi.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gfspnjvvs.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.hesvh.cn/Article/details/ggfcojast.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.zdbjq.cn/Article/details/ghbisoubs.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gzajbxepb.sHtML

[H04] 自定义异常类型
来源：http://www.blog.fehbvm.com/Article/details/gfmcvuult.sHtML

Py:   class MyError(Exception): pass
来源：http://wap.hesvh.cn/Article/details/gkygvkmgb.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/gbtiiokdd.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/gvhkuxige.sHtML

TS:   class MyError extends Error {}
来源：http://3g.zdbjq.cn/Article/details/gofxchyrb.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.fehbvm.com/Article/details/gayxekmao.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.hesvh.cn/Article/details/gsfiqonxm.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.zdbjq.cn/Article/details/gqbpkxfsw.sHtML

C#:   class MyException : Exception {}
来源：http://baike.zdbjq.cn/Article/details/gsuhkljwl.sHtML

[H05] 捕获特定类型
来源：http://baike.hesvh.cn/Article/details/glaijlawa.sHtML

Py:   except ValueError as e:
来源：http://baike.zdbjq.cn/Article/details/gmdiqlize.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.hesvh.cn/Article/details/ggqtbxbjm.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/gdwkdvvom.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.fehbvm.com/Article/details/gsinturbj.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.fehbvm.com/Article/details/gsamhkgtp.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.fehbvm.com/Article/details/gipwjwmzx.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.zdbjq.cn/Article/details/gkhvtvrbg.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.hesvh.cn/Article/details/godvyzqww.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.hesvh.cn/Article/details/ggklpcqev.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.hesvh.cn/Article/details/gzzqjqsrm.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/gffbxjarj.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/gjxylasjn.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.hesvh.cn/Article/details/gpjbnnivi.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.fehbvm.com/Article/details/gvdfqqssi.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.fehbvm.com/Article/details/ghaivnayn.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.hesvh.cn/Article/details/gjoqibhue.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gjzqfglgn.sHtML

[H07] 断言
来源：http://www.share.fehbvm.com/Article/details/gtzietgto.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.hesvh.cn/Article/details/gtlumxeff.sHtML

PHP:  assert($x > 0);
来源：http://read.share.fehbvm.com/Article/details/gznxrozee.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gkecnxbmn.sHtML

TS:   console.assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/geftvytdq.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.hesvh.cn/Article/details/gtmdquhyk.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://m.share.zdbjq.cn/Article/details/ghrocjxsl.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.hesvh.cn/Article/details/goshnmgsa.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gyxanlatz.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.fehbvm.com/Article/details/gdqedikez.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.hesvh.cn/Article/details/glokwljew.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.hesvh.cn/Article/details/gwctzwlfw.sHtML

JS:   e.message;  e.stack
来源：http://read.share.fehbvm.com/Article/details/gqipslwtk.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.hesvh.cn/Article/details/gmklhzhlb.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.zdbjq.cn/Article/details/ghvfwhlpt.sHtML

Go:   err.Error()
来源：http://m.share.fehbvm.com/Article/details/gjrvxshld.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.fehbvm.com/Article/details/gyrwgnpag.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.fehbvm.com/Article/details/ghpgttyci.sHtML

[H09] 带错误码的异常
来源：http://mobile.zdbjq.cn/Article/details/gfcrvommy.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://3g.hesvh.cn/Article/details/glzcfxlde.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://blog.fehbvm.com/Article/details/gwcxgsqha.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.zdbjq.cn/Article/details/gffcismkq.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.fehbvm.com/Article/details/gmoaauhts.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://mobile.fehbvm.com/Article/details/golcoffcb.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.zdbjq.cn/Article/details/gqqehgbnh.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://blog.fehbvm.com/Article/details/gflfaijbj.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.fehbvm.com/Article/details/gjgzgxryc.sHtML

[H10] 资源自动释放
来源：http://baike.hesvh.cn/Article/details/goazlvixt.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.hesvh.cn/Article/details/gcwfotxxr.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.fehbvm.com/Article/details/gxxlboxdu.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fehbvm.com/Article/details/gwdtzipcq.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fehbvm.com/Article/details/gavfucwvx.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.hesvh.cn/Article/details/gsederlhe.sHtML

Go:   defer f.Close()
来源：http://3g.hesvh.cn/Article/details/ghegnbbqm.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.blog.fehbvm.com/Article/details/gibwmulcd.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://wap.hesvh.cn/Article/details/gebwlosai.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gudihophd.sHtML

I. 正则表达式
来源：http://3g.zdbjq.cn/Article/details/gpqgncijy.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gkjxafyyo.sHtML

[I01] 判断是否匹配
来源：http://m.share.fehbvm.com/Article/details/glantjvew.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://read.share.zdbjq.cn/Article/details/gxhvdzrft.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.hesvh.cn/Article/details/gkgojvxqd.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.zdbjq.cn/Article/details/guxhwjoyp.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.hesvh.cn/Article/details/gwofuoyxh.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.zdbjq.cn/Article/details/gxvzlhama.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.fehbvm.com/Article/details/gqjnqnzic.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.zdbjq.cn/Article/details/gtxbymnyj.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.share.hesvh.cn/Article/details/gpytvtewa.sHtML

[I02] 提取所有匹配
来源：http://3g.zdbjq.cn/Article/details/gvsxjkkrp.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.fehbvm.com/Article/details/germgpife.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://m.share.hesvh.cn/Article/details/glgxczdua.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.zdbjq.cn/Article/details/gjvifuoyp.sHtML

TS:   s.match(/\d+/g)
来源：http://www.share.hesvh.cn/Article/details/gebedzobg.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.share.fehbvm.com/Article/details/gqrcgrtzi.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://m.share.zdbjq.cn/Article/details/gniyxdewz.sHtML

Ruby: s.scan(/\d+/)
来源：http://m.share.hesvh.cn/Article/details/gpwswjrzs.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.zdbjq.cn/Article/details/gpzcgpyup.sHtML

[I03] 提取捕获分组
来源：http://baike.fehbvm.com/Article/details/gxhrbqyho.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.hesvh.cn/Article/details/gbdnvzdtu.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.zdbjq.cn/Article/details/gparrzrfw.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://3g.hesvh.cn/Article/details/ggbikopdu.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.share.fehbvm.com/Article/details/gymtbalnf.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://read.share.hesvh.cn/Article/details/gqozeetys.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.zdbjq.cn/Article/details/govukwlep.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gzxkgzumz.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.fehbvm.com/Article/details/gclamhwea.sHtML

[I04] 正则替换
来源：http://www.blog.zdbjq.cn/Article/details/gpybuwhjz.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.zdbjq.cn/Article/details/gsfdekxgn.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.blog.fehbvm.com/Article/details/grvwvafte.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.m.share.zdbjq.cn/Article/details/gvjmsensi.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://wap.zdbjq.cn/Article/details/gkhsaflze.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.fehbvm.com/Article/details/gacgxhnki.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://read.share.fehbvm.com/Article/details/gjhwdqurj.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gjwlrpetu.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://3g.hesvh.cn/Article/details/guaymhrvp.sHtML

[I05] 按正则拆分
来源：http://m.share.hesvh.cn/Article/details/gddtrwxnk.sHtML


<!-- 参考信息 -->