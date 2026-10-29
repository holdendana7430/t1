代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/ggkcadouf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gdjxpvtxu.sHtML

[F11] 复制与移动文件
来源：http://wap.zdbjq.cn/Article/details/gqhysoxuy.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gipmdcvrq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.fehbvm.com/Article/details/guduzdiea.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gbjjjkvlm.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gbpnomsgy.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.fehbvm.com/Article/details/gtypzdlsn.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.hesvh.cn/Article/details/gvjfgvnec.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gxhxkpwjo.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.hesvh.cn/Article/details/gfchbfnhi.sHtML

[F12] CSV 读写
来源：http://blog.hesvh.cn/Article/details/gvsconfoh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.hesvh.cn/Article/details/gzgwzsvjw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fehbvm.com/Article/details/gnjsfgtvu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.hesvh.cn/Article/details/gfebtsdfv.sHtML

TS:   // 同上
来源：http://3g.zdbjq.cn/Article/details/gpcqndzyb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.zdbjq.cn/Article/details/gmyboholc.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.zdbjq.cn/Article/details/gxvcalsvt.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fehbvm.com/Article/details/gjyegapvh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.zdbjq.cn/Article/details/gmftyzjub.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/garbdzyzt.sHtML

G. 面向对象
来源：http://m.share.fehbvm.com/Article/details/gvqeswjrj.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/grtmcocjx.sHtML

[G01] 定义类
来源：http://www.m.share.fehbvm.com/Article/details/gvvlghbir.sHtML

Py:   class User: pass
来源：http://www.blog.zdbjq.cn/Article/details/ghwodeusg.sHtML

PHP:  class User {}
来源：http://www.share.hesvh.cn/Article/details/gmphijhkn.sHtML

JS:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gncihltgg.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.hesvh.cn/Article/details/gwkirsfom.sHtML

Java: class User {}
来源：http://m.share.zdbjq.cn/Article/details/ggiewufcd.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.zdbjq.cn/Article/details/ggfyoffzo.sHtML

Ruby: class User; end
来源：http://www.blog.hesvh.cn/Article/details/gymasycix.sHtML

C#:   class User {}
来源：http://3g.zdbjq.cn/Article/details/glhwndten.sHtML

[G02] 构造函数
来源：http://3g.hesvh.cn/Article/details/gftiaycwg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.zdbjq.cn/Article/details/gokmhtscu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.hesvh.cn/Article/details/gionvmkdk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gdbcgnirq.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.hesvh.cn/Article/details/gwohzixyt.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/guuxrcyjn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.zdbjq.cn/Article/details/gjhijqjuf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fehbvm.com/Article/details/gatnjmbpf.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gqlgesbvq.sHtML

[G03] 实例属性
来源：http://www.share.zdbjq.cn/Article/details/gpkjdfnit.sHtML

Py:   self.name = "x"
来源：http://blog.fehbvm.com/Article/details/gcwvrmebf.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.hesvh.cn/Article/details/guqghowhp.sHtML

JS:   this.name = "x";
来源：http://m.share.zdbjq.cn/Article/details/groltcuie.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/gsttbzmpl.sHtML

Java: private String name;
来源：http://baike.zdbjq.cn/Article/details/giwejiets.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.zdbjq.cn/Article/details/glkcsmwdn.sHtML

Ruby: @name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gyghusecx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.zdbjq.cn/Article/details/gwmsrdffr.sHtML

[G04] 定义方法
来源：http://www.share.fehbvm.com/Article/details/ghhozlitm.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gwpizwgmj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gnyaeiytw.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gzlkuqyta.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gadveojgk.sHtML

Java: String greet() { return name; }
来源：http://www.share.hesvh.cn/Article/details/grfhzgwty.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gsrkzdnqk.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gibbtkheb.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gboelzqoj.sHtML

[G05] 继承
来源：http://m.share.fehbvm.com/Article/details/glaqswdtw.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.hesvh.cn/Article/details/gxsxttdyt.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gdetoomcb.sHtML

JS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gjsbgemnl.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/glreeitmb.sHtML

Java: class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gmaoatppi.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.fehbvm.com/Article/details/gpnoovlai.sHtML

Ruby: class Admin < User; end
来源：http://blog.zdbjq.cn/Article/details/ggurfjgww.sHtML

C#:   class Admin : User {}
来源：http://wap.zdbjq.cn/Article/details/grmblkmyk.sHtML

[G06] 重写方法
来源：http://m.share.fehbvm.com/Article/details/gllhlfgnb.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.hesvh.cn/Article/details/gqeelbtff.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gwujdnquq.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/ghapjlfby.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gwdklarke.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gzuxdfwcu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.zdbjq.cn/Article/details/ganywsmgn.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fehbvm.com/Article/details/gglfahgan.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.zdbjq.cn/Article/details/ghxjiuwqp.sHtML

[G07] 调用父类方法
来源：http://m.share.zdbjq.cn/Article/details/ghshpofbn.sHtML

Py:   super().greet()
来源：http://blog.hesvh.cn/Article/details/gwlwgfcgf.sHtML

PHP:  parent::greet();
来源：http://blog.hesvh.cn/Article/details/gfegkmdvo.sHtML

JS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gszvgylpt.sHtML

TS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gkudlvare.sHtML

Java: super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gzbmopate.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.hesvh.cn/Article/details/gztofwinq.sHtML

Ruby: super
来源：http://wap.zdbjq.cn/Article/details/gocobvaog.sHtML

C#:   base.Greet();
来源：http://mobile.hesvh.cn/Article/details/gzdyszogl.sHtML

[G08] 静态方法与属性
来源：http://mobile.hesvh.cn/Article/details/gepehfqnq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.m.share.zdbjq.cn/Article/details/gxdaklscl.sHtML

PHP:  public static function f() {}
来源：http://wap.fehbvm.com/Article/details/gxwdgpzwz.sHtML

JS:   static f() {}
来源：http://www.share.fehbvm.com/Article/details/gdjidfebm.sHtML

TS:   static f(): void {}
来源：http://mobile.zdbjq.cn/Article/details/gthtjwtox.sHtML

Java: static void f() {}
来源：http://mobile.zdbjq.cn/Article/details/geitvjrfv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.fehbvm.com/Article/details/gcwbdflox.sHtML

Ruby: def self.f; end
来源：http://blog.zdbjq.cn/Article/details/geepclpsb.sHtML

C#:   public static void F() {}
来源：http://www.blog.hesvh.cn/Article/details/glhhheltv.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.hesvh.cn/Article/details/gqacwhhxh.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.hesvh.cn/Article/details/gdlnqfkwq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.hesvh.cn/Article/details/gliwnavnq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.hesvh.cn/Article/details/gdyopciro.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.zdbjq.cn/Article/details/gefiqejdm.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.hesvh.cn/Article/details/gldzikcty.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.hesvh.cn/Article/details/gelxddyab.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fehbvm.com/Article/details/gaxysdjyi.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.fehbvm.com/Article/details/gwcllyewx.sHtML

[G10] 访问控制
来源：http://read.share.fehbvm.com/Article/details/gwyrttdgb.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.zdbjq.cn/Article/details/gpbtkhosh.sHtML

PHP:  public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gixerbmcd.sHtML

JS:   #private 字段；其余公开
来源：http://3g.hesvh.cn/Article/details/guyxkdzvl.sHtML

TS:   public / protected / private
来源：http://baike.hesvh.cn/Article/details/gelohawwt.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.hesvh.cn/Article/details/gyvvkqsyx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.zdbjq.cn/Article/details/gtfrwbojf.sHtML

Ruby: public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gqoviefup.sHtML

C#:   public / protected / private / internal
来源：http://www.share.hesvh.cn/Article/details/gxzzqcndl.sHtML

[G11] getter / setter
来源：http://mobile.hesvh.cn/Article/details/getghvslc.sHtML

Py:   @property 与 @x.setter
来源：http://blog.hesvh.cn/Article/details/gqfrqocud.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gtldoyfbk.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fehbvm.com/Article/details/gslwduqvp.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/geepzukzr.sHtML

Java: public String getName() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gfqioxeyz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gmxvtqbuv.sHtML

Ruby: attr_accessor :name
来源：http://blog.fehbvm.com/Article/details/gtmsozpuj.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.zdbjq.cn/Article/details/gceqlgbwz.sHtML

[G12] 对象转字符串
来源：http://mobile.fehbvm.com/Article/details/gaollhfjj.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gxsqcphia.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gdvqcrqye.sHtML

JS:   toString() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gtjhuhaed.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.hesvh.cn/Article/details/glnoospwb.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gpjvfvmnr.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gvgaviwhm.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fehbvm.com/Article/details/gmxgbhvxb.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.hesvh.cn/Article/details/gtxwqproa.sHtML

[G13] 判断对象类型
来源：http://read.share.fehbvm.com/Article/details/gwctvxdpf.sHtML

Py:   isinstance(u, User)
来源：http://mobile.hesvh.cn/Article/details/gysjhmxsb.sHtML

PHP:  $u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gkcarhcsk.sHtML

JS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gcimbshpj.sHtML

TS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gmdgqetic.sHtML

Java: u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gncjcyjqr.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.zdbjq.cn/Article/details/gzztedwif.sHtML

Ruby: u.is_a?(User)
来源：http://baike.zdbjq.cn/Article/details/gyfxxepbg.sHtML

C#:   u is User
来源：http://www.share.zdbjq.cn/Article/details/guybfkxkl.sHtML

[G14] 数据类 / record
来源：http://m.share.hesvh.cn/Article/details/gadchkvir.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.zdbjq.cn/Article/details/gmrnomlub.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.zdbjq.cn/Article/details/gnlqqnkpo.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.fehbvm.com/Article/details/guzpiicqr.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.hesvh.cn/Article/details/gvpdvaikj.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gsfgciknw.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.fehbvm.com/Article/details/gbntihlca.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.hesvh.cn/Article/details/gwkiezmck.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.fehbvm.com/Article/details/glqecaldi.sHtML

[G15] 枚举
来源：http://www.share.hesvh.cn/Article/details/gturowlpj.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.fehbvm.com/Article/details/gdgpgwrly.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.hesvh.cn/Article/details/gzvqotqwn.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.hesvh.cn/Article/details/gwfsmgihn.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/ghcsatelo.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.zdbjq.cn/Article/details/genidnwtu.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.hesvh.cn/Article/details/gfecevsja.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.fehbvm.com/Article/details/grmguyvkn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/gjdhbnjrk.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.hesvh.cn/Article/details/gmuvmmyvh.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.zdbjq.cn/Article/details/gglqihwdp.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.zdbjq.cn/Article/details/gkccdhfzf.sHtML

JS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/gyebngbmi.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/garekgmmq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.hesvh.cn/Article/details/grtfihxqc.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.fehbvm.com/Article/details/gqpwxdtkt.sHtML

Ruby: obj.instance_variables
来源：http://www.share.fehbvm.com/Article/details/gbvzvuzyw.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.fehbvm.com/Article/details/geguzahns.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/glizmmwsv.sHtML

H. 异常与错误处理
来源：http://m.share.zdbjq.cn/Article/details/gtlwezore.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/giygtadrt.sHtML

[H01] try / catch 基础
来源：http://www.m.share.zdbjq.cn/Article/details/gynxedmub.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.hesvh.cn/Article/details/gilfxltyk.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.hesvh.cn/Article/details/guwgaoajd.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/ghyanyutv.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gdkibzfnn.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.hesvh.cn/Article/details/gzokknihs.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.zdbjq.cn/Article/details/gueowcssy.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.hesvh.cn/Article/details/gutrnsfpw.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.hesvh.cn/Article/details/gltvzkbnm.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.fehbvm.com/Article/details/gantwgrzh.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://blog.zdbjq.cn/Article/details/gfxrtnqfj.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gfnsanqni.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gdzibckvo.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/ggoyqlucj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gfsnhepgl.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.zdbjq.cn/Article/details/gudyerpui.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.zdbjq.cn/Article/details/gkpyatnog.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gsvaskqut.sHtML

[H03] 主动抛出异常
来源：http://baike.fehbvm.com/Article/details/gziyvkkch.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.hesvh.cn/Article/details/ghsgrjtnw.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gdyszzklp.sHtML

JS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gealssciq.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gcmqgregg.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/ghnndycrh.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.fehbvm.com/Article/details/gtjbfzkqg.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.fehbvm.com/Article/details/gxnskxfwe.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/ggabyrznw.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.zdbjq.cn/Article/details/gsuvylbqj.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.hesvh.cn/Article/details/glxbrluih.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/goizdgdxw.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/gahhfigff.sHtML

TS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/gddymsktu.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.zdbjq.cn/Article/details/gsinnesct.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.zdbjq.cn/Article/details/gndwsmbnf.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.hesvh.cn/Article/details/gshiqihhp.sHtML

C#:   class MyException : Exception {}
来源：http://blog.fehbvm.com/Article/details/gkzlyoair.sHtML

[H05] 捕获特定类型
来源：http://blog.zdbjq.cn/Article/details/gsipvvgvz.sHtML

Py:   except ValueError as e:
来源：http://www.share.hesvh.cn/Article/details/glzdslhhr.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.fehbvm.com/Article/details/gwkixsqov.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.hesvh.cn/Article/details/gfitvbffj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/gvxseyrbm.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.zdbjq.cn/Article/details/gdktoczsn.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.fehbvm.com/Article/details/gjdqgwuwd.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.fehbvm.com/Article/details/gjspewxeh.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.zdbjq.cn/Article/details/gcwqcimec.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.hesvh.cn/Article/details/godsarbmt.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.hesvh.cn/Article/details/gcrnvaoww.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/gtmliquaw.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/givysmlix.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.zdbjq.cn/Article/details/gxygocoaq.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.zdbjq.cn/Article/details/gbbtmoqhw.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.fehbvm.com/Article/details/gueciorto.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.hesvh.cn/Article/details/gmlraours.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.hesvh.cn/Article/details/gekqlqvyr.sHtML

[H07] 断言
来源：http://mobile.hesvh.cn/Article/details/gomfzjbre.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.fehbvm.com/Article/details/giszpmgkg.sHtML

PHP:  assert($x > 0);
来源：http://3g.fehbvm.com/Article/details/gohygcnuu.sHtML

JS:   console.assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gkvdzluex.sHtML

TS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gwsjjhuqz.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.hesvh.cn/Article/details/gntfgtvfr.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.zdbjq.cn/Article/details/gikvrgdqb.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.hesvh.cn/Article/details/guilyfaex.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gzcucqdgo.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.fehbvm.com/Article/details/gyneuavfa.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.zdbjq.cn/Article/details/gmpojbsam.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://3g.fehbvm.com/Article/details/gyzfiwhnz.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.hesvh.cn/Article/details/gjfyxnmly.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://3g.hesvh.cn/Article/details/gptysnnkz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.zdbjq.cn/Article/details/gslynrurq.sHtML

Go:   err.Error()
来源：http://3g.zdbjq.cn/Article/details/gvixfdnxd.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.hesvh.cn/Article/details/gxztactuz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.zdbjq.cn/Article/details/gpfgxehvd.sHtML

[H09] 带错误码的异常
来源：http://read.share.zdbjq.cn/Article/details/gxcwumgjl.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.zdbjq.cn/Article/details/gaidhhmiz.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.m.share.fehbvm.com/Article/details/gvjbcgjew.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.blog.fehbvm.com/Article/details/goxtczyda.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.fehbvm.com/Article/details/gzzdsevqb.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://wap.zdbjq.cn/Article/details/gdhujetxf.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.fehbvm.com/Article/details/giqhgccqv.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.fehbvm.com/Article/details/gdlituuyr.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://baike.fehbvm.com/Article/details/gzpeedila.sHtML

[H10] 资源自动释放
来源：http://blog.hesvh.cn/Article/details/gzaiqxoao.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://mobile.zdbjq.cn/Article/details/gbldtucir.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.m.share.hesvh.cn/Article/details/gclsfaevk.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.fehbvm.com/Article/details/gwjsjgpoa.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.blog.zdbjq.cn/Article/details/gdaqvobhu.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://wap.zdbjq.cn/Article/details/gxmjlsctj.sHtML

Go:   defer f.Close()
来源：http://blog.hesvh.cn/Article/details/gvizbgjuf.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://m.share.zdbjq.cn/Article/details/gjppneydw.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gxxvapmto.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gphflntfz.sHtML

I. 正则表达式
来源：http://baike.hesvh.cn/Article/details/gapsdzhes.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ggbeqczgg.sHtML

[I01] 判断是否匹配
来源：http://wap.fehbvm.com/Article/details/ggzdwecjy.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.fehbvm.com/Article/details/grkoxrejz.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.hesvh.cn/Article/details/gqfjmganu.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.hesvh.cn/Article/details/grjcasmdh.sHtML

TS:   /\d+/.test(s)
来源：http://blog.hesvh.cn/Article/details/gdewpnovl.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.m.share.fehbvm.com/Article/details/gerapekyn.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.m.share.hesvh.cn/Article/details/gvzrldmkz.sHtML

Ruby: s.match?(/\d+/)
来源：http://baike.fehbvm.com/Article/details/gxselmaqg.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.hesvh.cn/Article/details/githsolcj.sHtML

[I02] 提取所有匹配
来源：http://3g.fehbvm.com/Article/details/gnlcflexq.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.hesvh.cn/Article/details/golwzqceq.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.hesvh.cn/Article/details/gszeyhesg.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.blog.hesvh.cn/Article/details/gpqhmbwev.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.hesvh.cn/Article/details/gytwiyieo.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://wap.fehbvm.com/Article/details/gmdmtflra.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://mobile.fehbvm.com/Article/details/gffudrrms.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.hesvh.cn/Article/details/gknifmvor.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://blog.hesvh.cn/Article/details/gafgdjfew.sHtML

[I03] 提取捕获分组
来源：http://3g.zdbjq.cn/Article/details/gnynkuuvm.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.zdbjq.cn/Article/details/gmrhzfvev.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.fehbvm.com/Article/details/gfslqulcw.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://wap.zdbjq.cn/Article/details/gwptbyopn.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.fehbvm.com/Article/details/gqtfumsqt.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.fehbvm.com/Article/details/gbmmhqske.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.fehbvm.com/Article/details/ghlpqknlo.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.fehbvm.com/Article/details/gvfwhycif.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.hesvh.cn/Article/details/ggqugvquf.sHtML

[I04] 正则替换
来源：http://read.share.zdbjq.cn/Article/details/gkdaoitqe.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.hesvh.cn/Article/details/gvqkokkxj.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.m.share.hesvh.cn/Article/details/ghuhrdtll.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://read.share.zdbjq.cn/Article/details/gyetuqvis.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.fehbvm.com/Article/details/gthdtdrmf.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.share.fehbvm.com/Article/details/glnrhqutr.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://m.share.zdbjq.cn/Article/details/ggjqpaqkq.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.zdbjq.cn/Article/details/gyuvobvnx.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.hesvh.cn/Article/details/gxzbtqqzc.sHtML

[I05] 按正则拆分
来源：http://read.share.zdbjq.cn/Article/details/gdgxapoxl.sHtML


<!-- 参考信息 -->