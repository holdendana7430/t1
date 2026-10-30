代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.zdbjq.cn/Article/details/glpjzudph.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.fehbvm.com/Article/details/gpdycowva.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gaqrbhbtp.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gewinsdut.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gicnmzion.sHtML

TS:   path.extname("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gijazcbqn.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.zdbjq.cn/Article/details/gtpfmddxa.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gorcebavx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/glbimlijw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gwsdfrnpl.sHtML

[F11] 复制与移动文件
来源：http://wap.fehbvm.com/Article/details/guxvgdete.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gqkybhejo.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.fehbvm.com/Article/details/gvpobpoav.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gleqdpazf.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gqvrncqsh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fehbvm.com/Article/details/giespudsr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.hesvh.cn/Article/details/ghemfzzir.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gciblgalu.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.zdbjq.cn/Article/details/gxiaokkad.sHtML

[F12] CSV 读写
来源：http://mobile.hesvh.cn/Article/details/gvhhviodg.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.zdbjq.cn/Article/details/gobsfkbki.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.zdbjq.cn/Article/details/gjpmmvujb.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.hesvh.cn/Article/details/gimpszwym.sHtML

TS:   // 同上
来源：http://3g.fehbvm.com/Article/details/gvbifqvdm.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fehbvm.com/Article/details/guxqxyoju.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.fehbvm.com/Article/details/gbrepppyn.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.zdbjq.cn/Article/details/ghdmxjkzg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.zdbjq.cn/Article/details/ggajeyshx.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gzzvldykm.sHtML

G. 面向对象
来源：http://wap.fehbvm.com/Article/details/gjrrflvzj.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gvrtksccn.sHtML

[G01] 定义类
来源：http://www.share.hesvh.cn/Article/details/gzyaghzes.sHtML

Py:   class User: pass
来源：http://blog.zdbjq.cn/Article/details/gkixdbumh.sHtML

PHP:  class User {}
来源：http://m.share.zdbjq.cn/Article/details/gsowkgapo.sHtML

JS:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gjgetxuuv.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.hesvh.cn/Article/details/gsyrngfmg.sHtML

Java: class User {}
来源：http://www.share.hesvh.cn/Article/details/gwfxpirux.sHtML

Go:   type User struct { Name string }
来源：http://blog.hesvh.cn/Article/details/grwnwlflq.sHtML

Ruby: class User; end
来源：http://read.share.fehbvm.com/Article/details/gflkyxqui.sHtML

C#:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gwbwwmung.sHtML

[G02] 构造函数
来源：http://m.share.hesvh.cn/Article/details/gykvxggju.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.zdbjq.cn/Article/details/gvbhuvxmk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.fehbvm.com/Article/details/gbdhuryxy.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gygfnvwhp.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.hesvh.cn/Article/details/gpvbslmgh.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/geweayxzd.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fehbvm.com/Article/details/giplagykl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fehbvm.com/Article/details/gzqzgbuvb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.hesvh.cn/Article/details/gbbqifdzo.sHtML

[G03] 实例属性
来源：http://read.share.hesvh.cn/Article/details/gnzfszisc.sHtML

Py:   self.name = "x"
来源：http://blog.fehbvm.com/Article/details/gecmlqjlt.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gvauniacx.sHtML

JS:   this.name = "x";
来源：http://baike.fehbvm.com/Article/details/gaqvtoitd.sHtML

TS:   name: string = "x";
来源：http://wap.hesvh.cn/Article/details/gexdcdwzc.sHtML

Java: private String name;
来源：http://baike.fehbvm.com/Article/details/gzxgxkxei.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.zdbjq.cn/Article/details/gbtqqnamc.sHtML

Ruby: @name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gvgbzymqq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fehbvm.com/Article/details/gmfdwjiwq.sHtML

[G04] 定义方法
来源：http://wap.fehbvm.com/Article/details/gqicoyxqk.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gxbedbtcl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gvqlwhbsw.sHtML

JS:   greet() { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gijexrdaw.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gmhyongmy.sHtML

Java: String greet() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gagatjexr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gpgzkaixf.sHtML

Ruby: def greet; @name; end
来源：http://blog.zdbjq.cn/Article/details/grvqzfclz.sHtML

C#:   public string Greet() => Name;
来源：http://3g.zdbjq.cn/Article/details/gniqljgif.sHtML

[G05] 继承
来源：http://baike.fehbvm.com/Article/details/gatctdfbp.sHtML

Py:   class Admin(User): pass
来源：http://blog.zdbjq.cn/Article/details/gulgzctej.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/guxnqomuj.sHtML

JS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gmtcmqrod.sHtML

TS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gvlxykfew.sHtML

Java: class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gpufagnca.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.zdbjq.cn/Article/details/gpdmcnnoc.sHtML

Ruby: class Admin < User; end
来源：http://baike.hesvh.cn/Article/details/gzibyosay.sHtML

C#:   class Admin : User {}
来源：http://blog.hesvh.cn/Article/details/gwhreodql.sHtML

[G06] 重写方法
来源：http://wap.fehbvm.com/Article/details/gebordvxt.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.hesvh.cn/Article/details/gpyuozexz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gvyeumqzf.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gahmfdpwv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/glrhxosvc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gdlhfvjmc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.zdbjq.cn/Article/details/gkrgfhqbf.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.zdbjq.cn/Article/details/ggdzfjauf.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fehbvm.com/Article/details/gdtipiieg.sHtML

[G07] 调用父类方法
来源：http://wap.zdbjq.cn/Article/details/gwnqfvhxp.sHtML

Py:   super().greet()
来源：http://read.share.zdbjq.cn/Article/details/gfankljes.sHtML

PHP:  parent::greet();
来源：http://www.blog.zdbjq.cn/Article/details/gvvylctln.sHtML

JS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gwdqjfvgn.sHtML

TS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/goptcytcz.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/guzjakjmq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.fehbvm.com/Article/details/gqozsadjf.sHtML

Ruby: super
来源：http://www.blog.zdbjq.cn/Article/details/gtnwrlbwk.sHtML

C#:   base.Greet();
来源：http://read.share.hesvh.cn/Article/details/guswbhruj.sHtML

[G08] 静态方法与属性
来源：http://blog.hesvh.cn/Article/details/ggflguhrk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.hesvh.cn/Article/details/gtfrgjdiu.sHtML

PHP:  public static function f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gbzpqrhbg.sHtML

JS:   static f() {}
来源：http://3g.hesvh.cn/Article/details/graxfamce.sHtML

TS:   static f(): void {}
来源：http://mobile.zdbjq.cn/Article/details/ghuuecmtc.sHtML

Java: static void f() {}
来源：http://wap.hesvh.cn/Article/details/glljyeywu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fehbvm.com/Article/details/gzeayvzeg.sHtML

Ruby: def self.f; end
来源：http://www.blog.hesvh.cn/Article/details/glunkwusw.sHtML

C#:   public static void F() {}
来源：http://read.share.zdbjq.cn/Article/details/gmnyveuru.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.zdbjq.cn/Article/details/gspoqmkua.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.hesvh.cn/Article/details/gfbpvprrl.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.fehbvm.com/Article/details/gqwsgfpmr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.hesvh.cn/Article/details/gohvjitvz.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.zdbjq.cn/Article/details/gpbjachsg.sHtML

Java: interface Shape { double area(); }
来源：http://blog.hesvh.cn/Article/details/gykwumymq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.zdbjq.cn/Article/details/gxpfszunb.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.zdbjq.cn/Article/details/gnemvepoa.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.hesvh.cn/Article/details/gmojnyyga.sHtML

[G10] 访问控制
来源：http://m.share.hesvh.cn/Article/details/grgdqstvf.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.zdbjq.cn/Article/details/gujovlmyn.sHtML

PHP:  public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gsajkjyfs.sHtML

JS:   #private 字段；其余公开
来源：http://baike.fehbvm.com/Article/details/gxazpqcpq.sHtML

TS:   public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gqfkkveow.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.zdbjq.cn/Article/details/gojnpbzlu.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fehbvm.com/Article/details/gmfssmziv.sHtML

Ruby: public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gbajltugu.sHtML

C#:   public / protected / private / internal
来源：http://blog.fehbvm.com/Article/details/gzwgdeues.sHtML

[G11] getter / setter
来源：http://3g.fehbvm.com/Article/details/gnaklcefm.sHtML

Py:   @property 与 @x.setter
来源：http://baike.zdbjq.cn/Article/details/gpoerwstj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gburctseh.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/gncajbams.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gpwlopkjm.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gejgxawlf.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gqedvetpq.sHtML

Ruby: attr_accessor :name
来源：http://baike.fehbvm.com/Article/details/gfcscsrow.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.hesvh.cn/Article/details/gqqpmnlfh.sHtML

[G12] 对象转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gzkvckora.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/gnfclqxpm.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gpgeuoffk.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gjjkkqflx.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gkbayjpbd.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gymbskkke.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/ghwzhuana.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gmxurheii.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fehbvm.com/Article/details/grdxzvbmb.sHtML

[G13] 判断对象类型
来源：http://www.share.zdbjq.cn/Article/details/gedrpvwwz.sHtML

Py:   isinstance(u, User)
来源：http://wap.zdbjq.cn/Article/details/gsppmyckd.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gfpkrhfcs.sHtML

JS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gmgjwdlmo.sHtML

TS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gmgbkoywo.sHtML

Java: u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gvxgldyfh.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.hesvh.cn/Article/details/genfiyjla.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.zdbjq.cn/Article/details/guhpixrjo.sHtML

C#:   u is User
来源：http://wap.fehbvm.com/Article/details/gbxrrqeeh.sHtML

[G14] 数据类 / record
来源：http://www.share.hesvh.cn/Article/details/gfnisamyv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.zdbjq.cn/Article/details/gjotxdunr.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.fehbvm.com/Article/details/gflegihmq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.hesvh.cn/Article/details/gxyjiyomf.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.fehbvm.com/Article/details/gdoguimow.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.hesvh.cn/Article/details/gudrbgvlj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.blog.hesvh.cn/Article/details/glxpfngvu.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.hesvh.cn/Article/details/gphuetxxn.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.fehbvm.com/Article/details/gnogygddr.sHtML

[G15] 枚举
来源：http://www.blog.zdbjq.cn/Article/details/gfuveviim.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.fehbvm.com/Article/details/gvoujtzdm.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fehbvm.com/Article/details/gvpwrabme.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.hesvh.cn/Article/details/gpgtqxdis.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/gzgbnipcn.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.fehbvm.com/Article/details/gzqvypmhk.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.m.share.hesvh.cn/Article/details/gwmvzrosi.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.hesvh.cn/Article/details/ggkcemguu.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/gdnxyogud.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.hesvh.cn/Article/details/gvvycmhwt.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.hesvh.cn/Article/details/grwumxuni.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.zdbjq.cn/Article/details/gcjgjmwho.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/gdlpmobdt.sHtML

TS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/gcnefsoua.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.hesvh.cn/Article/details/gcexjkhrd.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.fehbvm.com/Article/details/gekettkie.sHtML

Ruby: obj.instance_variables
来源：http://3g.zdbjq.cn/Article/details/gzitnpqji.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.fehbvm.com/Article/details/gxhfbsnkx.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gpnlqqzoq.sHtML

H. 异常与错误处理
来源：http://mobile.hesvh.cn/Article/details/gtxiegdqe.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gbrxvkuhf.sHtML

[H01] try / catch 基础
来源：http://read.share.zdbjq.cn/Article/details/gabbfnyvt.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.fehbvm.com/Article/details/gsvvhjuew.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.zdbjq.cn/Article/details/givsqmafu.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gulkfggmo.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.hesvh.cn/Article/details/guwxxjtnf.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.hesvh.cn/Article/details/gkalotjhz.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.zdbjq.cn/Article/details/gymwtikma.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.zdbjq.cn/Article/details/gkvjneiwd.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.fehbvm.com/Article/details/gwfchmidj.sHtML

[H02] finally / ensure 收尾
来源：http://wap.fehbvm.com/Article/details/gfyivvmvn.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.fehbvm.com/Article/details/gpoiwikux.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/geaqqjklk.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/ghhtllphd.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gruvjopzc.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gfsyjrtpx.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.fehbvm.com/Article/details/gulsmoojf.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fehbvm.com/Article/details/gjiqpkxyv.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gksrxmzpl.sHtML

[H03] 主动抛出异常
来源：http://3g.fehbvm.com/Article/details/grtglzodk.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.fehbvm.com/Article/details/gblsxxlrj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gddviyskk.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gratkspqm.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gkvtrijru.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gusapcltu.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.hesvh.cn/Article/details/gmhhgucfv.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.hesvh.cn/Article/details/gazllvmsp.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gurqzuhvk.sHtML

[H04] 自定义异常类型
来源：http://baike.zdbjq.cn/Article/details/gcplzjzxq.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.hesvh.cn/Article/details/geauwpydi.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.zdbjq.cn/Article/details/gbrfjnkki.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/gqnlrsufn.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.hesvh.cn/Article/details/ggedzvikp.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.fehbvm.com/Article/details/gvhggpujj.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.zdbjq.cn/Article/details/gayqcvtjg.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.hesvh.cn/Article/details/gjhxqmhmj.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.zdbjq.cn/Article/details/gybkdidzh.sHtML

[H05] 捕获特定类型
来源：http://www.blog.zdbjq.cn/Article/details/grpmfwquw.sHtML

Py:   except ValueError as e:
来源：http://m.share.zdbjq.cn/Article/details/gmfschohm.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.hesvh.cn/Article/details/grphswttx.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.hesvh.cn/Article/details/gzefseywl.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.hesvh.cn/Article/details/gvccpkgzy.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.zdbjq.cn/Article/details/gkihllzou.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.zdbjq.cn/Article/details/gycwkkhfo.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.fehbvm.com/Article/details/ggsoyvoxl.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.fehbvm.com/Article/details/gymisaktw.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.zdbjq.cn/Article/details/glcfbwsoa.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.fehbvm.com/Article/details/gyaprwyvd.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/guidwvcxw.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.zdbjq.cn/Article/details/gvovxctkc.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.fehbvm.com/Article/details/gprbkzjlq.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.fehbvm.com/Article/details/gpahmloxi.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.zdbjq.cn/Article/details/gtdvqusgh.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.hesvh.cn/Article/details/gigbdpvsc.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.hesvh.cn/Article/details/gbzcervet.sHtML

[H07] 断言
来源：http://baike.zdbjq.cn/Article/details/gkpiqmmpe.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.hesvh.cn/Article/details/gwyrgtlbv.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gpxolgwma.sHtML

JS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gaxajgyxn.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gemsphvai.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.fehbvm.com/Article/details/gfwlhkjrm.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.fehbvm.com/Article/details/grlrhnals.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://wap.zdbjq.cn/Article/details/geygaswnn.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/gjwpkdmmx.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.fehbvm.com/Article/details/ghbijoqyh.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.hesvh.cn/Article/details/gpupuizid.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.fehbvm.com/Article/details/goqqiqsih.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.fehbvm.com/Article/details/gybziyemv.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.share.fehbvm.com/Article/details/gxqalgewl.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://blog.fehbvm.com/Article/details/gtmmbxxxk.sHtML

Go:   err.Error()
来源：http://read.share.zdbjq.cn/Article/details/gkuyjvsbx.sHtML

Ruby: e.message;  e.backtrace
来源：http://baike.hesvh.cn/Article/details/gvmdvkmzz.sHtML

C#:   e.Message;  e.StackTrace
来源：http://m.share.fehbvm.com/Article/details/gdydwwdiz.sHtML

[H09] 带错误码的异常
来源：http://read.share.hesvh.cn/Article/details/gjrghozqt.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.fehbvm.com/Article/details/gakkdiqfs.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.hesvh.cn/Article/details/gqusrdrni.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.share.zdbjq.cn/Article/details/gauunbjif.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://baike.fehbvm.com/Article/details/gdimeikui.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.zdbjq.cn/Article/details/grfiflsdg.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.share.fehbvm.com/Article/details/gvoyixjab.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://m.share.hesvh.cn/Article/details/gohfyrrhj.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.fehbvm.com/Article/details/goefcwpos.sHtML

[H10] 资源自动释放
来源：http://www.blog.hesvh.cn/Article/details/gewrntpuf.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://baike.fehbvm.com/Article/details/gpzxdtvvn.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.hesvh.cn/Article/details/gkezhupgd.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fehbvm.com/Article/details/gelywyjyg.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.fehbvm.com/Article/details/gyuonbvln.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.fehbvm.com/Article/details/gaevmechf.sHtML

Go:   defer f.Close()
来源：http://3g.zdbjq.cn/Article/details/gzysfevxm.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.m.share.zdbjq.cn/Article/details/gwvhtiyxi.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gomzzoejk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gfzdifhzy.sHtML

I. 正则表达式
来源：http://www.blog.hesvh.cn/Article/details/gsvatzvfh.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gczccaend.sHtML

[I01] 判断是否匹配
来源：http://blog.fehbvm.com/Article/details/gfuazwzml.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.share.hesvh.cn/Article/details/ggjozycbf.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://mobile.fehbvm.com/Article/details/gtqzwllcb.sHtML

JS:   /\d+/.test(s)
来源：http://read.share.hesvh.cn/Article/details/gusnwkxrj.sHtML

TS:   /\d+/.test(s)
来源：http://3g.fehbvm.com/Article/details/gadsewemi.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.fehbvm.com/Article/details/gpxqucavo.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://3g.hesvh.cn/Article/details/grcwrptbz.sHtML

Ruby: s.match?(/\d+/)
来源：http://blog.fehbvm.com/Article/details/gugwtgqks.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://wap.fehbvm.com/Article/details/gczksajtz.sHtML

[I02] 提取所有匹配
来源：http://www.blog.fehbvm.com/Article/details/glatyqbxz.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.m.share.hesvh.cn/Article/details/gqfugohgt.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.zdbjq.cn/Article/details/ghyihyyhj.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://m.share.fehbvm.com/Article/details/gyktsxcou.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.hesvh.cn/Article/details/gxnijxicy.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://3g.zdbjq.cn/Article/details/glaaohokw.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://blog.hesvh.cn/Article/details/gkmzsxrqu.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gffihtkam.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gqxjzikvd.sHtML

[I03] 提取捕获分组
来源：http://wap.zdbjq.cn/Article/details/gobeyflzf.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://read.share.fehbvm.com/Article/details/geshbtqla.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.hesvh.cn/Article/details/gwzheyxow.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://mobile.hesvh.cn/Article/details/gsjuebozu.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.zdbjq.cn/Article/details/gybiyblcp.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.zdbjq.cn/Article/details/gfgoxvltd.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://baike.fehbvm.com/Article/details/guefjwifq.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.fehbvm.com/Article/details/guclophkc.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.m.share.hesvh.cn/Article/details/gesbodjie.sHtML

[I04] 正则替换
来源：http://www.m.share.hesvh.cn/Article/details/gfqogvoqd.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.zdbjq.cn/Article/details/gggqxycgn.sHtML


<!-- 参考信息 -->