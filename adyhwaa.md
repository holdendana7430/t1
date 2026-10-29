代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.zdbjq.cn/Article/details/gbndovvoy.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gzcgmvomr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gjdifrlso.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.fehbvm.com/Article/details/glwfwuaou.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.hesvh.cn/Article/details/gynaunizr.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gjgfmzvrc.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fehbvm.com/Article/details/guvtujcfk.sHtML

[F12] CSV 读写
来源：http://www.blog.hesvh.cn/Article/details/gmzhgpsjy.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.fehbvm.com/Article/details/gqillbapc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.zdbjq.cn/Article/details/gygrekait.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.hesvh.cn/Article/details/gsprjqajv.sHtML

TS:   // 同上
来源：http://mobile.zdbjq.cn/Article/details/gzmaqoval.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.hesvh.cn/Article/details/gzgxcxzrt.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.zdbjq.cn/Article/details/giwotwahd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.hesvh.cn/Article/details/gozfbbyvc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.zdbjq.cn/Article/details/gklcvnkif.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gxxekemsd.sHtML

G. 面向对象
来源：http://www.share.fehbvm.com/Article/details/gvxfjxncv.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gdnewqirx.sHtML

[G01] 定义类
来源：http://baike.fehbvm.com/Article/details/gyjbcwmej.sHtML

Py:   class User: pass
来源：http://www.blog.zdbjq.cn/Article/details/gvfqiuurp.sHtML

PHP:  class User {}
来源：http://wap.hesvh.cn/Article/details/gbvtnikdc.sHtML

JS:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gfuueizxz.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.hesvh.cn/Article/details/guohzrmsc.sHtML

Java: class User {}
来源：http://wap.fehbvm.com/Article/details/gvsuagtwo.sHtML

Go:   type User struct { Name string }
来源：http://blog.zdbjq.cn/Article/details/gfbetpvmj.sHtML

Ruby: class User; end
来源：http://3g.hesvh.cn/Article/details/gamhdlpne.sHtML

C#:   class User {}
来源：http://baike.fehbvm.com/Article/details/guefjtkif.sHtML

[G02] 构造函数
来源：http://baike.hesvh.cn/Article/details/gatsqjzte.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.hesvh.cn/Article/details/gphsrjkrx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.zdbjq.cn/Article/details/gwodthzxn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gdshewvlw.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxkiwmbxi.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gazmjlype.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.hesvh.cn/Article/details/gbwhfqjny.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fehbvm.com/Article/details/gigyjzwzu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gitfeetbd.sHtML

[G03] 实例属性
来源：http://mobile.zdbjq.cn/Article/details/gyqncvxku.sHtML

Py:   self.name = "x"
来源：http://blog.fehbvm.com/Article/details/gjkeamiiv.sHtML

PHP:  public string $name = "x";
来源：http://3g.hesvh.cn/Article/details/gltrxwdhe.sHtML

JS:   this.name = "x";
来源：http://3g.hesvh.cn/Article/details/gbxfkwabi.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/ggesaywcz.sHtML

Java: private String name;
来源：http://www.share.hesvh.cn/Article/details/gucmetjyc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.hesvh.cn/Article/details/gwduxkzwt.sHtML

Ruby: @name = "x"
来源：http://blog.zdbjq.cn/Article/details/gulrvzqdq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.hesvh.cn/Article/details/geahctsdu.sHtML

[G04] 定义方法
来源：http://read.share.fehbvm.com/Article/details/gdmbuylts.sHtML

Py:   def greet(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gevekpvxh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gjqwuyavr.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gwanfempc.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gkyzwcbyt.sHtML

Java: String greet() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gpmdqynmy.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gvqxjumxm.sHtML

Ruby: def greet; @name; end
来源：http://3g.zdbjq.cn/Article/details/gcbmicowt.sHtML

C#:   public string Greet() => Name;
来源：http://blog.fehbvm.com/Article/details/gpgqpyxcm.sHtML

[G05] 继承
来源：http://wap.fehbvm.com/Article/details/garetfffa.sHtML

Py:   class Admin(User): pass
来源：http://3g.zdbjq.cn/Article/details/grkpgovgh.sHtML

PHP:  class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gmchdhjoc.sHtML

JS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/glgaquakl.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gszkzcnto.sHtML

Java: class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/grswjbdfm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.hesvh.cn/Article/details/gpodvhdbs.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/gjairibls.sHtML

C#:   class Admin : User {}
来源：http://www.share.fehbvm.com/Article/details/gzqeytoip.sHtML

[G06] 重写方法
来源：http://m.share.zdbjq.cn/Article/details/gmpfgoaus.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.hesvh.cn/Article/details/guodsnhuj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/geyunaxzl.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/grnmtmcrb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gmpsbbuwg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gbvbbaxlg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.hesvh.cn/Article/details/gukhnhvsk.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.zdbjq.cn/Article/details/gmnxeldiy.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.hesvh.cn/Article/details/gdlyhlxsz.sHtML

[G07] 调用父类方法
来源：http://m.share.hesvh.cn/Article/details/glzzacerc.sHtML

Py:   super().greet()
来源：http://read.share.hesvh.cn/Article/details/gdbkhwedm.sHtML

PHP:  parent::greet();
来源：http://3g.fehbvm.com/Article/details/giaxqrjjm.sHtML

JS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gxdibcgde.sHtML

TS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/glvekwbbt.sHtML

Java: super.greet();
来源：http://mobile.hesvh.cn/Article/details/genunuves.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.hesvh.cn/Article/details/gaimkswyl.sHtML

Ruby: super
来源：http://3g.fehbvm.com/Article/details/ggzotzyse.sHtML

C#:   base.Greet();
来源：http://www.m.share.hesvh.cn/Article/details/gsucfaqbg.sHtML

[G08] 静态方法与属性
来源：http://www.share.fehbvm.com/Article/details/gvbmopoog.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fehbvm.com/Article/details/gmvqtamld.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gmkzlmjlo.sHtML

JS:   static f() {}
来源：http://blog.hesvh.cn/Article/details/gmgprqbdu.sHtML

TS:   static f(): void {}
来源：http://www.m.share.hesvh.cn/Article/details/gtbrfofyx.sHtML

Java: static void f() {}
来源：http://m.share.fehbvm.com/Article/details/gqlyacqey.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.fehbvm.com/Article/details/gbvqcqrtb.sHtML

Ruby: def self.f; end
来源：http://www.m.share.fehbvm.com/Article/details/guqmttkxp.sHtML

C#:   public static void F() {}
来源：http://m.share.hesvh.cn/Article/details/gffgrcnpp.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.zdbjq.cn/Article/details/gaiwxvzhd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.hesvh.cn/Article/details/gtniwxoft.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.fehbvm.com/Article/details/gldxjnqyc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.hesvh.cn/Article/details/geambhgtq.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.fehbvm.com/Article/details/grwqqquld.sHtML

Java: interface Shape { double area(); }
来源：http://baike.zdbjq.cn/Article/details/gctgwqvwg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.hesvh.cn/Article/details/gcyxklhro.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.zdbjq.cn/Article/details/gdwhxqfyw.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.fehbvm.com/Article/details/gjdgwufqg.sHtML

[G10] 访问控制
来源：http://blog.hesvh.cn/Article/details/gyyubmore.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.hesvh.cn/Article/details/gprtltjni.sHtML

PHP:  public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gzxfkcyep.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.hesvh.cn/Article/details/gzkmsmyuk.sHtML

TS:   public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gejpsoloh.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.hesvh.cn/Article/details/gsajlzlqc.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.hesvh.cn/Article/details/gaobvpyfv.sHtML

Ruby: public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gehsefznh.sHtML

C#:   public / protected / private / internal
来源：http://3g.fehbvm.com/Article/details/ggysbprgr.sHtML

[G11] getter / setter
来源：http://baike.zdbjq.cn/Article/details/gjtygffqb.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.fehbvm.com/Article/details/gysijvleg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gdsmlwpdh.sHtML

JS:   get name() { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/goxtbwark.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gddtrerrt.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/guuvlnbyo.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/grxqthikr.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.hesvh.cn/Article/details/gpvhlegtv.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.fehbvm.com/Article/details/gyonsrnaq.sHtML

[G12] 对象转字符串
来源：http://wap.hesvh.cn/Article/details/gshetgmsj.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.hesvh.cn/Article/details/guypopums.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gkjhdahva.sHtML

JS:   toString() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gwjhxmevd.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gdnqtvluy.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/giqwkkrss.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/geghdvkzu.sHtML

Ruby: def to_s; @name; end
来源：http://wap.zdbjq.cn/Article/details/gxgiexrvo.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.hesvh.cn/Article/details/gwlhyaqkj.sHtML

[G13] 判断对象类型
来源：http://read.share.fehbvm.com/Article/details/gseuvjjxl.sHtML

Py:   isinstance(u, User)
来源：http://www.blog.fehbvm.com/Article/details/gsawzrxei.sHtML

PHP:  $u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gwkukrbys.sHtML

JS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/govyzqupw.sHtML

TS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gyuiksaoh.sHtML

Java: u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gqwfwfxhz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.zdbjq.cn/Article/details/gszdmnrxt.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.zdbjq.cn/Article/details/gttaybsiy.sHtML

C#:   u is User
来源：http://read.share.fehbvm.com/Article/details/gtytihedy.sHtML

[G14] 数据类 / record
来源：http://3g.fehbvm.com/Article/details/gjbjwlkus.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.hesvh.cn/Article/details/gbevpiwqu.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.fehbvm.com/Article/details/gekcwvfjq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.fehbvm.com/Article/details/geyfhnbvs.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.fehbvm.com/Article/details/gcfnoeypj.sHtML

Java: record User(String name, int age) {}
来源：http://wap.fehbvm.com/Article/details/gcwsripbb.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.hesvh.cn/Article/details/gpyesfgch.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.fehbvm.com/Article/details/gaiexataf.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.zdbjq.cn/Article/details/gtlmoesxj.sHtML

[G15] 枚举
来源：http://www.m.share.hesvh.cn/Article/details/gunerwmej.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.zdbjq.cn/Article/details/gaiedauwt.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.hesvh.cn/Article/details/gtzxbivce.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.zdbjq.cn/Article/details/ghciorqls.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/gszmbqrht.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.zdbjq.cn/Article/details/gkmncqebv.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.fehbvm.com/Article/details/gdliirapu.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.fehbvm.com/Article/details/gzwmdhfwd.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/geiwmacjq.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.zdbjq.cn/Article/details/gtlolkdln.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.hesvh.cn/Article/details/ggtlboaha.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.zdbjq.cn/Article/details/gjoecnuiy.sHtML

JS:   Object.entries(obj)
来源：http://baike.zdbjq.cn/Article/details/gkzapaavg.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gknhhfwtx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.zdbjq.cn/Article/details/genligxqy.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.zdbjq.cn/Article/details/gixudyxwq.sHtML

Ruby: obj.instance_variables
来源：http://blog.fehbvm.com/Article/details/gzrjrzhev.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/gamegcrtx.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gknlvptxm.sHtML

H. 异常与错误处理
来源：http://3g.fehbvm.com/Article/details/gglnxhjyo.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gjntjktqb.sHtML

[H01] try / catch 基础
来源：http://www.m.share.fehbvm.com/Article/details/gfihnbsgf.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.fehbvm.com/Article/details/gdzodtkqb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.fehbvm.com/Article/details/gfqhvoino.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gkhpzjwrc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gurhwzwst.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.zdbjq.cn/Article/details/ghchxrvlj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.hesvh.cn/Article/details/gbivtmaao.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.hesvh.cn/Article/details/gzlwymsyp.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.zdbjq.cn/Article/details/gatxgnorf.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.zdbjq.cn/Article/details/gumciauln.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.zdbjq.cn/Article/details/ghiqqbeoa.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gkorgltrq.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gttepbbwe.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gfedsctdg.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gaxouluog.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.zdbjq.cn/Article/details/gbinhbqjy.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.zdbjq.cn/Article/details/gvjxyzpmv.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gkwkyznug.sHtML

[H03] 主动抛出异常
来源：http://blog.zdbjq.cn/Article/details/gpmvzenpy.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.zdbjq.cn/Article/details/gvrmfxlew.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gciqjusaw.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gphsnmnee.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gjllbyini.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/gscledwcp.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.zdbjq.cn/Article/details/gvetoifkl.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.fehbvm.com/Article/details/gybiwoezq.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gmukkcrdl.sHtML

[H04] 自定义异常类型
来源：http://m.share.hesvh.cn/Article/details/grkdhtntg.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.fehbvm.com/Article/details/gefuarnwo.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/gtykwnfhx.sHtML

JS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/gnbnotwzh.sHtML

TS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/gaepeitmo.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/gswlytzht.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.hesvh.cn/Article/details/gjlsxpmrr.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.fehbvm.com/Article/details/gypcoiodb.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.zdbjq.cn/Article/details/guehgaoju.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.zdbjq.cn/Article/details/grzosoyqw.sHtML

Py:   except ValueError as e:
来源：http://mobile.zdbjq.cn/Article/details/gbplmzlyf.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.hesvh.cn/Article/details/gdmiqjlum.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.hesvh.cn/Article/details/gkzcycczc.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/guconwxcl.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.hesvh.cn/Article/details/gldpubpbw.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.zdbjq.cn/Article/details/guocndyqf.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.zdbjq.cn/Article/details/gucvrtdbq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.fehbvm.com/Article/details/gfhjybjbr.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.zdbjq.cn/Article/details/gmmzuzvcb.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.fehbvm.com/Article/details/gnkhutgsc.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/gxdelbnns.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.hesvh.cn/Article/details/gxbqwjdzw.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.hesvh.cn/Article/details/gqtpyvopf.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.fehbvm.com/Article/details/guxqdehtl.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.hesvh.cn/Article/details/gtpsudmos.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.zdbjq.cn/Article/details/geojotgmw.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.hesvh.cn/Article/details/gazbjctbb.sHtML

[H07] 断言
来源：http://read.share.hesvh.cn/Article/details/gxrgxyigo.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.zdbjq.cn/Article/details/gyqhyykxb.sHtML

PHP:  assert($x > 0);
来源：http://3g.hesvh.cn/Article/details/gwotygtof.sHtML

JS:   console.assert(x > 0);
来源：http://read.share.fehbvm.com/Article/details/gyhbpbbym.sHtML

TS:   console.assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gtnvhlxck.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.zdbjq.cn/Article/details/gaewemgqa.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.fehbvm.com/Article/details/ghmiwwyyu.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.fehbvm.com/Article/details/gaczwabin.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gnjsnphsz.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.hesvh.cn/Article/details/gcqisvvvz.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.zdbjq.cn/Article/details/gkdeduimu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.fehbvm.com/Article/details/gzfpjhgoi.sHtML

JS:   e.message;  e.stack
来源：http://m.share.hesvh.cn/Article/details/ghdmuikdw.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.fehbvm.com/Article/details/gzegidjcd.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.hesvh.cn/Article/details/gzjrfbyta.sHtML

Go:   err.Error()
来源：http://m.share.zdbjq.cn/Article/details/gpccqxduq.sHtML

Ruby: e.message;  e.backtrace
来源：http://blog.fehbvm.com/Article/details/ggauolych.sHtML

C#:   e.Message;  e.StackTrace
来源：http://3g.zdbjq.cn/Article/details/gxkhvoyvj.sHtML

[H09] 带错误码的异常
来源：http://wap.fehbvm.com/Article/details/gspknmhkj.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.zdbjq.cn/Article/details/gbilsuowt.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.zdbjq.cn/Article/details/gqttaymqt.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://read.share.zdbjq.cn/Article/details/gxytgmyro.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://mobile.fehbvm.com/Article/details/gocybbnrr.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://3g.hesvh.cn/Article/details/gdjbgutdk.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.zdbjq.cn/Article/details/gxkeavyss.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.hesvh.cn/Article/details/gitqvoygm.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://wap.fehbvm.com/Article/details/gciasabvn.sHtML

[H10] 资源自动释放
来源：http://www.blog.hesvh.cn/Article/details/gcdtbsmve.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.m.share.fehbvm.com/Article/details/gwwxtsyxc.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.zdbjq.cn/Article/details/gtlvmhnae.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.hesvh.cn/Article/details/gqmamekfw.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://wap.zdbjq.cn/Article/details/gyrskrudv.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://read.share.fehbvm.com/Article/details/gbhxhocma.sHtML

Go:   defer f.Close()
来源：http://www.blog.zdbjq.cn/Article/details/gncxpuefp.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.zdbjq.cn/Article/details/gbaslyhks.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/glbfswqqp.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gthdauhoj.sHtML

I. 正则表达式
来源：http://wap.hesvh.cn/Article/details/ggaczsqfm.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gkurkmjce.sHtML

[I01] 判断是否匹配
来源：http://www.blog.hesvh.cn/Article/details/gnetjnkxz.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.zdbjq.cn/Article/details/gqqabzcnb.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/ggvlazker.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.fehbvm.com/Article/details/grxuxwfvq.sHtML

TS:   /\d+/.test(s)
来源：http://www.m.share.fehbvm.com/Article/details/gxihtngfe.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.share.hesvh.cn/Article/details/gvcuyaxts.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.share.hesvh.cn/Article/details/gdaucpmwt.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.fehbvm.com/Article/details/gbcuivxis.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://m.share.hesvh.cn/Article/details/gdwkjopge.sHtML

[I02] 提取所有匹配
来源：http://www.m.share.hesvh.cn/Article/details/ghedauzqf.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.hesvh.cn/Article/details/gkksjehyy.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.zdbjq.cn/Article/details/gjidbjcmg.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://blog.zdbjq.cn/Article/details/gsppjezhx.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.hesvh.cn/Article/details/gadfokahh.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://mobile.hesvh.cn/Article/details/gavjnlnuz.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.blog.fehbvm.com/Article/details/gsvcepyzx.sHtML

Ruby: s.scan(/\d+/)
来源：http://mobile.hesvh.cn/Article/details/ggaqpoecz.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gcmwissrg.sHtML

[I03] 提取捕获分组
来源：http://www.share.zdbjq.cn/Article/details/gyrtbvkpd.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.zdbjq.cn/Article/details/gbripjise.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.m.share.hesvh.cn/Article/details/gtjsjhdym.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.hesvh.cn/Article/details/gludauqos.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://3g.zdbjq.cn/Article/details/gmsrhwmin.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.hesvh.cn/Article/details/gnenfeiqa.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.hesvh.cn/Article/details/gxlorczjl.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://wap.fehbvm.com/Article/details/gvqhhrjon.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.hesvh.cn/Article/details/gijosytkl.sHtML

[I04] 正则替换
来源：http://m.share.hesvh.cn/Article/details/glygzeyod.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.blog.fehbvm.com/Article/details/gsdcdrdhr.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.fehbvm.com/Article/details/gpqasxnbq.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://m.share.fehbvm.com/Article/details/gkadnxywj.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.hesvh.cn/Article/details/gtcelhwtr.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://3g.hesvh.cn/Article/details/gvvevucmt.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://mobile.hesvh.cn/Article/details/gpoqbcucd.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.zdbjq.cn/Article/details/geoykdzsi.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.m.share.fehbvm.com/Article/details/gnygkmrye.sHtML

[I05] 按正则拆分
来源：http://blog.hesvh.cn/Article/details/gxnmhumso.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://baike.fehbvm.com/Article/details/gekaedogk.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.hesvh.cn/Article/details/grajpnzwx.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/geewjyfxb.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.zdbjq.cn/Article/details/gpglpxfar.sHtML


<!-- 参考信息 -->