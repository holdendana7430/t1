代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dbnonhpe.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2blfqfzdm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2wyavphkp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ucpzrrci.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wrgtitzg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nefxdwep.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2dnlisqed.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2jfippqxy.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2nzymzjta.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iyglofyh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2jixvgeqm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2maqihbno.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2oiuximgp.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dhztcywg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2zslcbwtr.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2pikylkxg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2uxzhjhlr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2ltribyvm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2rqumeuml.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2vsjdqiro.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2sjthxqcn.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2uurijnjr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2qehsnakz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2obmtrzfk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xowhuajl.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2vasjcxua.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rqvrpxbb.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2vhlrjqsu.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2kwgctdfg.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xpvubfjy.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wewnwmkx.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2ypkwzytx.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2lvjhzgit.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2rfmmsagw.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2kebqkbmn.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2vgsykokl.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2zwtjtfxo.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2ddcumzpw.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2cmaonnvw.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2fujhiukm.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rwtonbuj.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2hzzybnpm.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2iirncfdv.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2alwpixft.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yhoidocn.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2vklqxgai.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2vhbhcfbu.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2paricevb.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2vmgyldpg.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2dxqmgdkd.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2fbvmsxqn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2udynijdm.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2niztppzv.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2tvtbdbht.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2jwqhonan.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ngfwyael.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2wudzdtlm.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2pcuxwztg.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2gchxizsa.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rgialqai.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2uqxabjlj.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2tztsrhyu.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2tuvdysee.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2akilfbmg.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2mefnquxq.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2sgpzovcs.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2sxbxfmyx.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kejltryt.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2bpfwysup.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2jnkkgvlv.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2gcaxwesu.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zjgqgrdv.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2ttwxzivp.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2xsyfindv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qqxccncu.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yulntnxp.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ibdhmebu.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lczruzjg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2gtkbrsry.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2yxhfwzzl.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2ssmwlbnh.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2rqrxfrly.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2tryabatl.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2bdolgmvm.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2kpwlaouv.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2eheknals.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2umfdlyea.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2tzhwhpuu.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2fgmhwwfg.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2auadlxmn.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2oyqyghmx.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2qffvantd.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2nhqrtyxo.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hpwtevsx.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2xvobasjj.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2srdxdcoj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2erafntvq.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2wqehnwrn.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2svvvyujt.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2rqibboji.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2xfkkgtei.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2nkxqkdmt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2qcyuwiqj.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2imleeahz.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2jrlgvsmp.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2xlbycozb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2admfeljw.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2qusvpnuz.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2ecagmafo.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2hrnuajod.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2kjwibmvo.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2ondzyxgw.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ybcdiwvd.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2vwyqlomn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2pqtupete.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2guujudzk.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2njdxowli.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2zditcuqi.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2buymcglo.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2daeyzeok.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2jvcbwakn.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2bhhvtmza.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2scsomxqi.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2svmgxttg.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2arjpznic.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2dkdedglw.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2unsjutdn.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2gzpuezqo.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kdhfuvql.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2adqlyaon.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ohyevwvf.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cewtvdfa.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2qhfajvle.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2kewlujvf.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2owihkokv.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2quewqnbw.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2jbcvmrof.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2gseymwki.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2koyqcokv.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2krzesjkv.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2avkdppmp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2jwgjgnaw.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2rgnetwow.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2rfzbyxut.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2yxsaksst.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2ohqksvxl.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2hpdbpmfu.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2payznnjn.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2poswxcsk.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ieutcemo.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2rzdgyvbf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2spnxwxhp.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2ahpvhlep.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2vgyuuhxl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2tdiobdcn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2axfgczfk.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2toomjwqv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2rdiwseli.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2lwlzvufh.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2zhlhcgmd.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2mpwbfgpp.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2xjqdkvza.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2aykrrazk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2ojtizhbf.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2vdwzkwab.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2dphxoppu.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2bpzifvue.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2evoyrhur.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2ehzaizym.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2yoxkhfiu.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2vjxsceqx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cvmquxuz.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2cfacznue.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tzuhpxzf.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2vziotgda.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2axvovfko.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2yslypcup.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2gmzhfuxn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2jwaubutj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2spzylfak.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2fjsgyzum.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2yvztalyg.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2ftnfrkde.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2proiqnkv.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2dhcatvrt.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bhxaftsx.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2axluwahr.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pnjkbegn.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2fdavdpqd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2mhnorgse.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2vsuhajue.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2enrwbumu.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2esbvmzak.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2wxngulzs.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2xamjzivj.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2cearqrum.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ismixlsk.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2jcjzmgss.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2uvuatgbe.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2qubsxfmq.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2paybfknr.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2wviumouo.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2tqbhmbql.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2seilwxuw.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2olbshvge.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2ldavxchn.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2qacbyczd.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2qcerubxg.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2wyzwwskn.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2jmjzzbwg.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2gjiczqnj.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2vgucqrpt.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2imukbqjp.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yjluyarf.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2snnabdsw.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2klkjmkdr.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2kxlpiaes.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2vijuwrgd.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2xsbimnnd.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2dtvakkas.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2ysguueds.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2rzypdvcj.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2pmgnokkp.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2oaxkvjqk.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2tbvyjtwv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2bnzbhnyz.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2ddlomnlf.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2nboxxihn.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2rbkrigzy.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2nvlfacfm.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2eoffbgoy.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2deiekeje.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gutmeyvj.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2esnvaaip.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2vrkchzge.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2jjshcmzh.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2wozqlikv.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2kvqjrzxr.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2yupqgwuv.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2klvjtyvi.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2xsbxuxji.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2xibozgos.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2fxqbddab.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2awjyupjo.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2aslxfaie.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2fefcsbtl.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2lmcwsvjr.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2ekzrjrej.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2dedfekof.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2bgfavogc.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2miizxheb.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2cjsvhasg.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2zlzoytri.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2lklhgixu.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2tmquehhq.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2odpfgdkl.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2vbtlxuxd.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2tgnrcvhv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2uoeftbdp.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2plcdakpa.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2vlnfdgjv.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2gukwxdmp.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2yqvnefuz.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gkzyphqp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2avttipta.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2xdxdaefr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oyzdmsam.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2mzdbodfc.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2wbmifbjy.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ragdculn.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tcvytded.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2napqzuaa.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2dugcdqwl.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2dskypvho.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ncxvoljo.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2lejqfcmw.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2sjglncsh.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ynreungo.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2ncpfkdjl.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2dvngmllb.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2xhjmsjgz.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2vhezzrpq.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2ukovoxxa.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2ckedbmqx.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2uwxxqkuh.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2ajihgdur.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2cvhjahst.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2obbblkoa.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2fnkdyhvm.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2mxvdmwsd.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt2gyblpzqv.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2inxxvjpw.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2hjvxzkka.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2xukfbmxi.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2soteacqu.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2mdvmzujp.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2upcsnugv.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2ryhcjqvd.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2zimwneov.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2vxkutekz.html


<!-- 参考信息 -->