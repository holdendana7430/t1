代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3wtwsoyve.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3mqpliqzc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nyfxkvbp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pvmnqdtg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jpizfkza.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kbdczyhd.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3adfunhvp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nljzjuqs.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gphmxlhe.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qzrhfbrl.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3bxpnjxnk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3kyditwsv.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3decpuogv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3kbwybyyf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3bszwjgmc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3vlmavifj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3iwzconqo.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3epwtdecn.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3ppvllgle.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3gonohsuy.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3yxugjjmc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3ceevafvk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3mqzbxakr.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3yuhxbqzn.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3jbjwcprm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3dxclkxyf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3voanyucc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3uglheowh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qewqeusc.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3pzwbdwki.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uppkjlnq.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3hhkfvecr.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3txemozez.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3ewrmbdix.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3pgemjcju.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3iowcfxwv.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3sljzyvkq.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3xjzxqfye.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ybmqemsa.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kpblqbkm.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3zapjibpz.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3htsssqkf.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3vvliwyqg.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mlgnlcyi.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3faakjkdp.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aqwgblro.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3khfqxaqb.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3ruyuivky.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pjmhvdvw.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3cgmluoic.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3jrpdiaka.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3njitclpp.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3vkzubdyj.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3nftqnvzd.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3rzmneiox.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3vqponosl.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3imiekrma.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3swqzkkxa.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3znbqsllm.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ihhwuppm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3lzrtmrye.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3mhewgpba.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3akrpumui.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3lvgsxdhc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3yqpkqhyz.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3fgejirdt.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3jefaxyet.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3jrdddoxw.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3afsggoci.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qzcvzucz.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cppgddyd.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ilezhkes.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3wgfweuph.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3olfbfpyq.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3xiszkzdd.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rornecfa.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3jkqzbtyo.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3bxsxsytn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ywhazrna.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qjovjlyq.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vqkzqklq.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kclhghgj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3ufqkxgoq.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3pqhubmnl.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3crncvoaz.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3npnsegjy.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3gagooxyk.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ahcwqfca.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ylhiruwj.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3iquwlsed.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rekcjjew.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3famsmcey.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3hunkpaak.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3gjmcgntx.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3vhumodsx.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3uiwsszov.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3fgpzzbja.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3wqbcdbhn.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3plqpllfv.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3zgtpagvk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3hxvxxkjb.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3vlwqcrou.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3hgvsqaob.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3hvcqwvmn.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3ndhkokdx.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3blzekiwn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3uqhvyozb.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3mgpwwjuq.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ifldibwh.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3ntxwblwb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3rdhbains.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vehxvqtx.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3wovwcngs.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3ynghexow.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3vzyknnuu.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3noauvhss.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3hphxdwlb.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3wcjrhkoq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3dlxtdwbg.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3bubbjvua.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3bimbtjic.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3aivkrtgt.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3feylzjxx.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3wzonrsho.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nzhjxkio.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kymynzob.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rkqipcpn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3bsrosjgy.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3qqomrkvu.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3ruuurjvs.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3urgwrhrt.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3zwucxrgx.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vrurujsq.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qchkbhvm.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3zmxrtrmr.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xkpzulkv.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3uyxyxjsx.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3tlxofdlb.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ppuncmbe.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3upvzvsqh.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3eqaaxinm.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ibwpcydx.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3dyhiymhm.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3wjmvjpcs.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3oshyqgzo.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3mtjaieib.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3rlyuloyp.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3hedwdqzh.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3jrusvrub.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3nhqcceec.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3mcjnleko.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3mnteskex.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3etsahkhh.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ksunwqwj.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3hwhbbpxu.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3kspcuxzm.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3zbuglefw.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3wtdyksem.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3ghatlkoh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3ghmlluaw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3vooirgru.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hsvsgrxb.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3xihiujpd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3xaziepem.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3hbqvjefo.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ojdoxari.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3tcmfalfn.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3peetgtqe.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3odfxpkbc.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xidpxcgf.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nlwyllsw.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3enuacrcd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3enwlustr.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3ksjtdnds.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3imfosypw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3skgnmidq.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3gxceakmh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zvrjbhlk.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3ygclhksd.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3djrsaclq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3ietnvrgt.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3vqgchtre.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3icbcuzxs.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3hvagzmgs.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3txbcafgf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3lspfyzog.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3fqgthdou.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3rlironho.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3dxubhyvq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3tdtlvtfr.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3oarvspcz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3rqrxzazf.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gqmonjnx.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3csyzqzil.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3mvjazjao.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ubdjbsxv.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3sslraubv.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3mvmitmpn.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3xmbhshcn.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3lhjliduw.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3lkchhwax.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3qbczcppe.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3ubgfxozn.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3cciemquw.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3frewdqrz.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3zokmszhd.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3xyzrzthu.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3wdcxqbyf.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3xdkwbsai.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3vabkxlel.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3otlachps.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3glidehzm.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3pppgkckr.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3tmzimmig.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3djjdgzou.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3vegcllrx.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3slvpkcmx.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3cbtduqju.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3vrlrmxzl.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3acbpsxku.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3vsxeauvu.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3wluwhbfy.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3hgzvoejc.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3ffuxqvvm.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3usuqtwja.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3xoutispv.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3pmaglbrw.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3wodxpfad.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3gsqqesml.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3wpjrtojp.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3eyxblutn.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3nymahrda.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3gipoqwtf.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3vvonxsyo.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jdgunpto.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3wcdiatvo.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bccmknoj.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3lskygcjc.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3imzfanwi.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3cdkydupl.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lnbaxial.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3fbziyjqi.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3hhxwnabj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3rugsthzc.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3jsrvsbwj.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3bpkmwksn.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3hdbqetup.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3hjvudvnt.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3bjfmnuuc.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3jvfiwzhz.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3mtvgvudq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3pkrxjfvc.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3bddqpole.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3zwqxsinp.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3xsofsvqr.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3ightfuep.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3bgwepqmy.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3kilwzwrt.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3glzgqgbk.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3anrsyumh.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3sglyzvat.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3cecdnuxh.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3arhluqek.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3tsjzmxxj.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3busdzpjc.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3taqupbhh.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3auqvixpo.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qrqvjvrl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lvsnkxvb.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ntexissm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lszstggj.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3oejmiplf.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3hnllsdny.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3uomjdctc.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3jdcbwydd.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jxzajmhs.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3ufzprtya.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lfstmthu.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3rrvmajpr.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3whihpefn.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3gbnyibyh.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3eehcyvav.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3lpujlxqx.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3bmeneapr.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3ledouzit.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dvxhpnbt.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3bkspcutm.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3jwuqihob.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3rhynmrtt.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3jpcymmaq.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3jrjmldyb.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3hjxdyxfj.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3ccqmcgec.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3liscwcbj.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3aeznjyln.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3phdunzci.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3ltfwaxmc.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3rvlyvtal.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3ubblkkpa.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3qwqdfqra.html


<!-- 参考信息 -->