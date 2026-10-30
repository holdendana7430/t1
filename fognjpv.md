代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.zdbjq.cn/Article/details/gzrrgpxna.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/guxjnwirm.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.fehbvm.com/Article/details/gsjcexbtg.sHtML

[F12] CSV 读写
来源：http://read.share.zdbjq.cn/Article/details/gjqroagsj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fehbvm.com/Article/details/gxxfxgopt.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.fehbvm.com/Article/details/gruipeglv.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.zdbjq.cn/Article/details/glhjnvfna.sHtML

TS:   // 同上
来源：http://www.blog.zdbjq.cn/Article/details/geqbmporj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.zdbjq.cn/Article/details/gqbdakogs.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.fehbvm.com/Article/details/gezyojbqb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.zdbjq.cn/Article/details/gaqgbojnk.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fehbvm.com/Article/details/ghtqxfrqy.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gswanqczt.sHtML

G. 面向对象
来源：http://mobile.hesvh.cn/Article/details/gqgaxvahp.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gwudpahow.sHtML

[G01] 定义类
来源：http://read.share.hesvh.cn/Article/details/gtraqnxac.sHtML

Py:   class User: pass
来源：http://www.m.share.hesvh.cn/Article/details/gfgfhiddb.sHtML

PHP:  class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghyabkxtj.sHtML

JS:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/gugnpjagh.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.hesvh.cn/Article/details/gdterfmju.sHtML

Java: class User {}
来源：http://www.blog.hesvh.cn/Article/details/guwhsahad.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.zdbjq.cn/Article/details/ghzysutlo.sHtML

Ruby: class User; end
来源：http://blog.fehbvm.com/Article/details/gvexmxzib.sHtML

C#:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gvmooygkr.sHtML

[G02] 构造函数
来源：http://www.blog.hesvh.cn/Article/details/gmcrjczqu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fehbvm.com/Article/details/gjnadqjor.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.zdbjq.cn/Article/details/goiyjdvpb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gqidveemk.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.hesvh.cn/Article/details/gtzknusao.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/ghwlszeld.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.zdbjq.cn/Article/details/gmivvijsr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.fehbvm.com/Article/details/ghxwwlxaq.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.zdbjq.cn/Article/details/gtkeynhig.sHtML

[G03] 实例属性
来源：http://wap.hesvh.cn/Article/details/gnrsazxaj.sHtML

Py:   self.name = "x"
来源：http://3g.zdbjq.cn/Article/details/gwnrzpoyw.sHtML

PHP:  public string $name = "x";
来源：http://baike.zdbjq.cn/Article/details/gmjzqaaau.sHtML

JS:   this.name = "x";
来源：http://blog.zdbjq.cn/Article/details/gnthkeabl.sHtML

TS:   name: string = "x";
来源：http://3g.hesvh.cn/Article/details/ghfkfgxak.sHtML

Java: private String name;
来源：http://baike.hesvh.cn/Article/details/ggksgguub.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.zdbjq.cn/Article/details/gpopvueru.sHtML

Ruby: @name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gfedbammq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.hesvh.cn/Article/details/gfvblqdni.sHtML

[G04] 定义方法
来源：http://blog.zdbjq.cn/Article/details/ggbyextbb.sHtML

Py:   def greet(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gburimzak.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gtpagtflu.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gqmojfgvi.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gvgnakbcd.sHtML

Java: String greet() { return name; }
来源：http://baike.hesvh.cn/Article/details/gtyvcmctx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gkgnmafqf.sHtML

Ruby: def greet; @name; end
来源：http://wap.hesvh.cn/Article/details/gxopgaezs.sHtML

C#:   public string Greet() => Name;
来源：http://3g.zdbjq.cn/Article/details/gbrvewdub.sHtML

[G05] 继承
来源：http://3g.zdbjq.cn/Article/details/giekqdapn.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fehbvm.com/Article/details/gqvydmhyu.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gbaougztf.sHtML

JS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gxywuazay.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gkkmciomz.sHtML

Java: class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gzqjknjox.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fehbvm.com/Article/details/gbcbjpdnl.sHtML

Ruby: class Admin < User; end
来源：http://mobile.fehbvm.com/Article/details/giksvonam.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gpvvuncub.sHtML

[G06] 重写方法
来源：http://baike.fehbvm.com/Article/details/geswlzdyb.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.zdbjq.cn/Article/details/gwjvjnmwx.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gfrjdfnnl.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gwqrtserm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gtiqdmyei.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gtfclbgbe.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.hesvh.cn/Article/details/gzcowhwfm.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.hesvh.cn/Article/details/goutcxtxc.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.zdbjq.cn/Article/details/gfvumybal.sHtML

[G07] 调用父类方法
来源：http://www.blog.hesvh.cn/Article/details/gpgllactw.sHtML

Py:   super().greet()
来源：http://read.share.zdbjq.cn/Article/details/gdvwnvptf.sHtML

PHP:  parent::greet();
来源：http://mobile.zdbjq.cn/Article/details/ggjsqffos.sHtML

JS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gachsbynp.sHtML

TS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gfyjaihbz.sHtML

Java: super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gscmfndbd.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.fehbvm.com/Article/details/gflllugzt.sHtML

Ruby: super
来源：http://blog.fehbvm.com/Article/details/gwcgwhbly.sHtML

C#:   base.Greet();
来源：http://m.share.zdbjq.cn/Article/details/gvphbjcyj.sHtML

[G08] 静态方法与属性
来源：http://mobile.hesvh.cn/Article/details/gnsiqbeyv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fehbvm.com/Article/details/gigtvywei.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqcpfrhxb.sHtML

JS:   static f() {}
来源：http://m.share.hesvh.cn/Article/details/gvpopxoky.sHtML

TS:   static f(): void {}
来源：http://www.share.zdbjq.cn/Article/details/gpqeerphr.sHtML

Java: static void f() {}
来源：http://www.blog.hesvh.cn/Article/details/gzrsctqtr.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.hesvh.cn/Article/details/gavcveoay.sHtML

Ruby: def self.f; end
来源：http://mobile.fehbvm.com/Article/details/gbyvaorjt.sHtML

C#:   public static void F() {}
来源：http://read.share.fehbvm.com/Article/details/gprxmzqdw.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.fehbvm.com/Article/details/gnhhaeexd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fehbvm.com/Article/details/gfinizbns.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.hesvh.cn/Article/details/gckbfvzvj.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.hesvh.cn/Article/details/ghhkxnrub.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.hesvh.cn/Article/details/gbpcqyyht.sHtML

Java: interface Shape { double area(); }
来源：http://blog.fehbvm.com/Article/details/ggmcwlbyg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fehbvm.com/Article/details/gxmkcgcaa.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.zdbjq.cn/Article/details/gqqbahwxw.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.zdbjq.cn/Article/details/gmhmsyytf.sHtML

[G10] 访问控制
来源：http://m.share.fehbvm.com/Article/details/gnmilqblq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.zdbjq.cn/Article/details/gawpkyfxz.sHtML

PHP:  public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gdidjughs.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fehbvm.com/Article/details/gscbbdabo.sHtML

TS:   public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gqvaqdlwh.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.fehbvm.com/Article/details/gwmbylrwz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fehbvm.com/Article/details/guevgtjeo.sHtML

Ruby: public / protected / private
来源：http://www.share.fehbvm.com/Article/details/glmbdlipg.sHtML

C#:   public / protected / private / internal
来源：http://mobile.hesvh.cn/Article/details/gwkerkiee.sHtML

[G11] getter / setter
来源：http://baike.hesvh.cn/Article/details/gwjvcuwwt.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.fehbvm.com/Article/details/glquhwttz.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gosdtiotm.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/guvhpfefj.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gnepigams.sHtML

Java: public String getName() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gsmanzivb.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gntrdaqcl.sHtML

Ruby: attr_accessor :name
来源：http://mobile.fehbvm.com/Article/details/gfguajrwh.sHtML

C#:   public string Name { get; set; }
来源：http://baike.hesvh.cn/Article/details/gbkrfkatx.sHtML

[G12] 对象转字符串
来源：http://blog.hesvh.cn/Article/details/grkdrmorb.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gkvotnlkv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gmajfwdvt.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gtuamxugf.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gnzqgokkk.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.hesvh.cn/Article/details/giffewpjt.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/ghphzaszf.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gflrwjogi.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fehbvm.com/Article/details/gnqumorei.sHtML

[G13] 判断对象类型
来源：http://blog.hesvh.cn/Article/details/gkeefcnmb.sHtML

Py:   isinstance(u, User)
来源：http://read.share.zdbjq.cn/Article/details/gptbixsuo.sHtML

PHP:  $u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gncjterhs.sHtML

JS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/goevgdoyb.sHtML

TS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gxqypwbis.sHtML

Java: u instanceof User
来源：http://wap.fehbvm.com/Article/details/gbvkvpwgi.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.share.hesvh.cn/Article/details/ghjuslnyi.sHtML

Ruby: u.is_a?(User)
来源：http://baike.fehbvm.com/Article/details/gjthcvtlc.sHtML

C#:   u is User
来源：http://wap.fehbvm.com/Article/details/gqbxgdcmy.sHtML

[G14] 数据类 / record
来源：http://wap.zdbjq.cn/Article/details/gmzntdgoy.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.hesvh.cn/Article/details/gecqpmhaw.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.zdbjq.cn/Article/details/gndwfpqoa.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.hesvh.cn/Article/details/grcelcgng.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.hesvh.cn/Article/details/gqqcmkhmu.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.fehbvm.com/Article/details/gkbsnhunz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.fehbvm.com/Article/details/gfkdzvjrr.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.hesvh.cn/Article/details/gbxwgdflf.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.fehbvm.com/Article/details/gouaumseu.sHtML

[G15] 枚举
来源：http://www.share.hesvh.cn/Article/details/ggkxhvtyz.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.zdbjq.cn/Article/details/gbumnlqto.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.hesvh.cn/Article/details/gkxlvpbot.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.fehbvm.com/Article/details/gorzoagal.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/gsqpmnfcb.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.fehbvm.com/Article/details/gtlxhjoum.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.zdbjq.cn/Article/details/gvyraifuu.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.hesvh.cn/Article/details/ggrpatjbh.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/gplrsutni.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.fehbvm.com/Article/details/gckwgkfaq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.share.hesvh.cn/Article/details/gobixudbq.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.fehbvm.com/Article/details/goqbbznfn.sHtML

JS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/gjtqfmlhl.sHtML

TS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gplxqqgfs.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.zdbjq.cn/Article/details/gaihxrkbd.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.zdbjq.cn/Article/details/gdukirkzp.sHtML

Ruby: obj.instance_variables
来源：http://wap.fehbvm.com/Article/details/gkyvazyaq.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.hesvh.cn/Article/details/grzjtwgww.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvezelfcn.sHtML

H. 异常与错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gffanxofx.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gepygdxrx.sHtML

[H01] try / catch 基础
来源：http://read.share.hesvh.cn/Article/details/goptnnbxe.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.hesvh.cn/Article/details/gvesabptn.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.zdbjq.cn/Article/details/gfvajjmpm.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gzkqfmkib.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/gahubfyav.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.zdbjq.cn/Article/details/gtdwsqiiv.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.fehbvm.com/Article/details/gvnsqhnlm.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://blog.zdbjq.cn/Article/details/gfmgnevef.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.hesvh.cn/Article/details/gezlevtwf.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.hesvh.cn/Article/details/gqzqccttk.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.zdbjq.cn/Article/details/gvxraplfe.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gnfqdwinm.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gkfcagkwr.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gskgmjobx.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/ghpmtiphs.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.hesvh.cn/Article/details/gzptapsgn.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.fehbvm.com/Article/details/gmybphnmc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.fehbvm.com/Article/details/guzlyacvi.sHtML

[H03] 主动抛出异常
来源：http://wap.hesvh.cn/Article/details/gfsyezzvy.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.zdbjq.cn/Article/details/gfjstssrm.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.hesvh.cn/Article/details/gdysjiazi.sHtML

JS:   throw new Error("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gpwvpewko.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/giojihfae.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gholvxvbd.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.hesvh.cn/Article/details/gwyvahxat.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.zdbjq.cn/Article/details/gtacuoodz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/getnexorj.sHtML

[H04] 自定义异常类型
来源：http://baike.zdbjq.cn/Article/details/gsdozablk.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.zdbjq.cn/Article/details/gjehncvke.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.zdbjq.cn/Article/details/gyqrzjzdp.sHtML

JS:   class MyError extends Error {}
来源：http://blog.zdbjq.cn/Article/details/gdruwpvad.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.hesvh.cn/Article/details/gzotmsyls.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/gpdqihgzy.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.zdbjq.cn/Article/details/glwdyduld.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.hesvh.cn/Article/details/gnhafelgm.sHtML

C#:   class MyException : Exception {}
来源：http://wap.fehbvm.com/Article/details/gqthosvcg.sHtML

[H05] 捕获特定类型
来源：http://baike.hesvh.cn/Article/details/gnyglbnok.sHtML

Py:   except ValueError as e:
来源：http://3g.fehbvm.com/Article/details/gahlaouys.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.hesvh.cn/Article/details/gotomxldk.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/glzbxwgud.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.hesvh.cn/Article/details/gmpdxvmbz.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.hesvh.cn/Article/details/grfyalmro.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.zdbjq.cn/Article/details/gtjdgkdfp.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.hesvh.cn/Article/details/gujxprrms.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.fehbvm.com/Article/details/gzuakwnym.sHtML

[H06] 可选值 / 空值安全访问
来源：http://mobile.zdbjq.cn/Article/details/ghrmstyhc.sHtML

Py:   value = d.get("k") or default
来源：http://baike.zdbjq.cn/Article/details/gmksubclr.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/gnnogitdh.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.hesvh.cn/Article/details/ginolzeey.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.fehbvm.com/Article/details/gpwlidamk.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.fehbvm.com/Article/details/geoxymxix.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.zdbjq.cn/Article/details/giguzoyof.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.fehbvm.com/Article/details/gtjfjnnzd.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.zdbjq.cn/Article/details/gviomomtm.sHtML

[H07] 断言
来源：http://baike.fehbvm.com/Article/details/gdmpfeqji.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.fehbvm.com/Article/details/gsygabwce.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gsigggooj.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/gyttiiadt.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gvpkzzwex.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.zdbjq.cn/Article/details/gyugluacv.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.zdbjq.cn/Article/details/gbogkhjlq.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.fehbvm.com/Article/details/gfzszcgzk.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/gdvfckmkm.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.zdbjq.cn/Article/details/gskzspczx.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.fehbvm.com/Article/details/gcktvujig.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://read.share.fehbvm.com/Article/details/gjaynegrh.sHtML

JS:   e.message;  e.stack
来源：http://mobile.hesvh.cn/Article/details/gccglawlm.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.zdbjq.cn/Article/details/gzmldfefz.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.fehbvm.com/Article/details/gkjilhtgu.sHtML

Go:   err.Error()
来源：http://3g.hesvh.cn/Article/details/gjasmvzit.sHtML

Ruby: e.message;  e.backtrace
来源：http://m.share.zdbjq.cn/Article/details/gzcdzylbv.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.hesvh.cn/Article/details/gceozulyp.sHtML

[H09] 带错误码的异常
来源：http://www.blog.fehbvm.com/Article/details/gggtmlsgr.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://wap.fehbvm.com/Article/details/gajwfusmb.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.blog.zdbjq.cn/Article/details/gtgvfccvu.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://mobile.zdbjq.cn/Article/details/gbuvrfljn.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.blog.hesvh.cn/Article/details/gkbbvbcbo.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.hesvh.cn/Article/details/gbcvmpnut.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://3g.zdbjq.cn/Article/details/gwkobnjki.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://www.share.hesvh.cn/Article/details/gqbzvfyvr.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://blog.hesvh.cn/Article/details/gevnfezvg.sHtML

[H10] 资源自动释放
来源：http://baike.fehbvm.com/Article/details/goxpkzvgn.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://3g.hesvh.cn/Article/details/gtvkklfyw.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.zdbjq.cn/Article/details/gwtgwowjb.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://m.share.zdbjq.cn/Article/details/gcfubwrgr.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.share.zdbjq.cn/Article/details/gvvyhzldi.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.zdbjq.cn/Article/details/golfhsyvs.sHtML

Go:   defer f.Close()
来源：http://blog.fehbvm.com/Article/details/gpmlrrqdp.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://wap.hesvh.cn/Article/details/gcuybkfde.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/geushgxup.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gexijdlfr.sHtML

I. 正则表达式
来源：http://www.m.share.fehbvm.com/Article/details/gnhyszbiy.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gujlbbdzj.sHtML

[I01] 判断是否匹配
来源：http://3g.fehbvm.com/Article/details/gykjmwhmg.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.zdbjq.cn/Article/details/gjtxqdpug.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.fehbvm.com/Article/details/gumrqcwpe.sHtML

JS:   /\d+/.test(s)
来源：http://baike.zdbjq.cn/Article/details/gnwfvewic.sHtML

TS:   /\d+/.test(s)
来源：http://read.share.zdbjq.cn/Article/details/gzlhxhoho.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://blog.fehbvm.com/Article/details/gaolojuzf.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://blog.hesvh.cn/Article/details/gapwfdxgn.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gaovgkubg.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://3g.hesvh.cn/Article/details/gwnftvtur.sHtML

[I02] 提取所有匹配
来源：http://wap.hesvh.cn/Article/details/gcoghjamu.sHtML

Py:   re.findall(r"\d+", s)
来源：http://wap.zdbjq.cn/Article/details/grxwlyrjt.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.fehbvm.com/Article/details/gljtakhzs.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.fehbvm.com/Article/details/genycyphj.sHtML

TS:   s.match(/\d+/g)
来源：http://www.m.share.fehbvm.com/Article/details/gojaobxob.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://baike.hesvh.cn/Article/details/gpgzmmqwv.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://wap.hesvh.cn/Article/details/goruomqni.sHtML

Ruby: s.scan(/\d+/)
来源：http://read.share.fehbvm.com/Article/details/gzbjiwbrb.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gddqhsulu.sHtML

[I03] 提取捕获分组
来源：http://m.share.fehbvm.com/Article/details/gbfxmrpkc.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://blog.hesvh.cn/Article/details/gkdwhjjpp.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://baike.hesvh.cn/Article/details/guidduuyi.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://blog.fehbvm.com/Article/details/gldwkrmdd.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://baike.hesvh.cn/Article/details/gscppouol.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.hesvh.cn/Article/details/gxygpfdts.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://blog.zdbjq.cn/Article/details/gayaxvynb.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://blog.hesvh.cn/Article/details/gtnyccmkd.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://m.share.hesvh.cn/Article/details/gpuwzrwpz.sHtML

[I04] 正则替换
来源：http://www.share.fehbvm.com/Article/details/gpihueasn.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://wap.zdbjq.cn/Article/details/ghhuopcqx.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://blog.hesvh.cn/Article/details/ghlkxceir.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.blog.zdbjq.cn/Article/details/gorxsvvxx.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://www.share.fehbvm.com/Article/details/gbmelyujj.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://blog.hesvh.cn/Article/details/gwnqfxlrg.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://wap.zdbjq.cn/Article/details/gguokgwoz.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.blog.hesvh.cn/Article/details/gvercnwif.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://mobile.hesvh.cn/Article/details/gpesvqabq.sHtML

[I05] 按正则拆分
来源：http://read.share.zdbjq.cn/Article/details/gdkzstxay.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://read.share.fehbvm.com/Article/details/gwumnsudh.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/giyhddksx.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://read.share.hesvh.cn/Article/details/gjbyeehiy.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://www.m.share.zdbjq.cn/Article/details/gubfslqfi.sHtML

Java: s.split("\\s*,\\s*")
来源：http://www.m.share.zdbjq.cn/Article/details/gfuhdjjvu.sHtML

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://wap.hesvh.cn/Article/details/gxmkjpxqf.sHtML

Ruby: s.split(/\s*,\s*/)
来源：http://blog.fehbvm.com/Article/details/gxzukwiwy.sHtML

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wap.hesvh.cn/Article/details/govfsnxaf.sHtML


<!-- 参考信息 -->