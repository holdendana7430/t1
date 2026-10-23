代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3anmryxxh.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nhtecsxc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3dfkwbjib.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mvdtevfy.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sjrhwvtg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3esslthsq.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3zxkzynzs.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3lgovijfo.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jzovrpny.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dgenhbka.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vcyncsqw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3taoiyijl.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3kxlldavy.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3mjghakei.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3mbfqtzgw.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3pdbklhka.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3qkkltyii.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3osxdwikv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3tkvhcsrw.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3jpmefcxi.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3jkebswlr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3suuomvfb.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3ipgerwwb.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3fjmnueoj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bcqrrpil.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3ynyjzkcm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3huithsfh.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3txuzqxij.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3cutljpyl.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3gglswzfr.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3dvvczzrc.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3vzgejngp.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qjyuycss.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3lvsnhdxi.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ikltxbuk.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ymrxvfqs.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3nhbzrrnw.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3mfmkttpt.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3tcrnimhq.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3lhrgzllh.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3acdzxpbe.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3rqwrzfif.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3hhynqvut.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3nnnkhcip.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3luycntwu.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3wcbirjzs.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3wnnorfkd.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3pbeyplec.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3pgvjopgv.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3eyiiljtk.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3kihtomaf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3gsnyfgru.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3gulazkbb.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3olgkwhda.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3mfnszhnq.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3xucqpipc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3emlcxyfd.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uzeomwax.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3yahjeldk.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3cuhcmohc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3urgynzkk.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3glaefhsk.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3usiakmst.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3vuxiggva.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3sqgqrssh.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dxmwokda.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xgsuztpj.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3orlsniqe.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wylpcrzc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3krriomvq.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3sjnjhrco.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bpswiapj.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3gurydzuv.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3lbswjfam.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3piiwpeqa.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3clihqzoa.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xksprvjc.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uleoqrol.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3clwjvvha.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3fpzxtplx.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3uyftvfyn.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3fsqwwbzx.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3hynvidmi.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ogewafiw.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3okvkgbol.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3bqyjxezf.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3uxdmfooi.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3fejnfvuk.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3yvxbnltk.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3fhxjmrdw.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3mczepsed.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3tefhtvei.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3twpatyxr.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3nqpkmjcd.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3wpbisoyy.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3eaegjwym.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3zualixlw.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3ptojnhut.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3qccuhlfb.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3kexrvubq.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3rrknjthw.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3ywvwuvjl.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3rqpnwijv.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3goppzqsz.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3noxkitdf.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3ouzbsxip.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3kzvfufkc.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3vikgdmxw.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3zjhrcrqs.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3pxgkzxns.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3rddmjjgm.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3smpypgom.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3hnioqsxs.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3hoummkyj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3erxwmzvb.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3iutussrs.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3ootmsoik.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3unhfqsvd.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3kqfqxlnr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3umbsfezc.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qvmeisex.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3bjswqqjq.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hkdreczf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ofkpawhh.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3jwezfhka.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3ycdsqqsl.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3iwdbqhrf.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3xieoyszz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jerquwwq.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3mdbvywjk.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fdvcwdtv.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3feougsok.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3dadgvtjv.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3lmttlmrt.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3lugyqnhb.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3ihdvedvg.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3mqmmrjab.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3nodtnium.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3yuhlrzht.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3fqixzfwh.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3fhcoytdu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3msclsyxo.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3kdyrqlnb.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3hytebptn.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3suoguklx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3yuggikqb.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3frbgzmtc.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3uqibrejy.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3ddoqhhwr.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sriahguf.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3dvdvipvy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3lxutxvem.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3pymlhwwv.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3xseyltdc.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3sbfhcajt.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rdvoudrr.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3tivzlubq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ikiyjbxn.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3virqgaxw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3khgcmylu.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3otmyleik.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3gzfliiix.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3skrulsdn.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3gsqclwqw.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3yeijwzks.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qluyvsvg.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3cxhrlbby.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3jecaqsbw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3tltxakkn.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3jirmhupa.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3firobllg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qyukksrs.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3vrcrdwsi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3waaccgdm.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3wlbtjilt.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3tzvnpnwc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xyhdftzl.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3iwsvxkwr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3fqzszpsh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3mfrpyqwl.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3ghvfvggs.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3bydojeqm.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3fcbqkrvv.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3tbbdcxqc.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3qnkmndez.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vhdqzmdq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3jggssbhc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nyrlyqex.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vdvqhvip.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3yeqysdbi.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3inrlprtr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3eyofkxht.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3caafpzcr.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3tghyaibl.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3bupwpejz.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ausqvcum.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3advneuts.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3dtgqtvpv.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3edsplmbh.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3jqnajgzm.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3apizgwke.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3olthgzml.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3zupzhsys.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3ynfgulea.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3xbinlhtt.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3jcksmxvz.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3fneyevnr.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3glmdwjvw.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3tprkqbnp.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3bktpbylk.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3vdobmurj.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3njyxpgfr.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3rymmedns.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3yzcjnoft.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3mmghgele.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vmlmmwok.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3ckoynwfe.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3fwwshmwc.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xdtbqrww.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3eptcfdkk.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3ykdrbsva.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3fwykdlho.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3onwukirl.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3emithvyg.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3rmexmxrc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3ttiykpsl.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3gegjuxft.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3oykgjwoc.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3hxxqidmw.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3westnenf.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3tuimwsma.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ggkxrgrh.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lvhhldlg.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3dspxahsz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3zwdobybk.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3qvgbazzx.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3owdeefpt.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3toqmjwec.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3hxaawkqt.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3giopjkox.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3xbxxlped.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3yejfqyps.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3etrzlmpt.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3ochgrzjf.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3dqeivmoj.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3utylbvcm.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3hlvmkdoa.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3ckihveir.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3egvqguqu.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3vrxpnvoz.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3hxolykcj.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3kjiqulrs.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3wquzqsua.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3vdctfwba.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3bngevpni.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3kaimpzug.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3gssobkea.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3lampgzkv.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3moqyanza.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3bvbmlaww.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3pkejsuwe.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3udzvjcuv.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3tmdozheg.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3itokghwn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qjuqpszz.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3okxvjuik.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3puxwplei.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3idflhitt.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3lgsjscdx.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3uhxtghhu.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wspprbqp.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3dmvupouk.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3efdrysso.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3piyredaw.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3zrqmcobd.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3jrfnqqbf.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3ycppyith.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3atazeyxk.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3gtrvrrmr.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3ahjlgplm.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3uqzuliwv.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mnjwdmqw.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3vqjbljzs.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3ymyisiig.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3zrynssxi.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3bnhqmanw.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3bkqqmjhf.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3nnqaystk.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3mrquyxnq.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3sijkfbmw.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3mrezhstq.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3zarajyra.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3qvtrhsvp.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3aryalfkb.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3ydqrsxkp.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3zeafvcsw.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt3dhbflzkb.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3rylmujrf.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3fcfabllb.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3hswdhepm.html


<!-- 参考信息 -->