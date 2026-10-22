代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2dewghtoa.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2brhwpama.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2fzkrkkuo.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pohtxhym.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2givqolva.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2gbsesdun.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mfzrjbij.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qtjtypse.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ekkcbeja.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2apxrdqyk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2odyfjmfb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qoqsashy.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oenkivyp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2icxxotjt.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2ehcofmiw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bhzmxojd.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2zytuztdg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2oaaxzeao.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yrmxiigx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2jhrhdxms.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2mpvlgiit.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hbcxuhil.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2mjrnsuot.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2fpwcadvw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2otlqqema.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2mjlrmcea.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2nxyywiet.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2twahpghh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2neqjrewa.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2jydkccgx.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2rfhvyetr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2rslwzibo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ofivjwrn.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2kigqvzgy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2noqwbzjf.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2fpovtvjx.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2mseamvew.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wjgxgjki.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ffakbdfk.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2khmztvgy.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2bryabkap.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2pwnrqjez.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2ogokijil.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ukipkuxy.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2xfjoshgl.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2wledsmxi.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2xlnxpxeo.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2witlvkvs.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2rzpnmuhs.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2zqzapfia.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2mqrxvrgf.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2kptqukbx.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2hxfltout.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2ksrunvzz.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2pjqhnsts.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2pdomiiqp.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qsgyagqg.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2flkqtnfs.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2sgdloxae.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2tesmfbla.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2gkqssisz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2applzyxn.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2woiffsdx.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2cdreqecm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2jyxnfhsh.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2gvetdpfo.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2jncppxvk.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2hpkavyvb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2vwvxsybq.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2jfvggyhv.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2zzyzlpwv.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2svvidhbq.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2epahovmr.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zezbhluo.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2fdonedpn.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2wxdbakny.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2anjwwlhr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2lwrnsltf.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2cdpyhmvm.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jrsmsoxj.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2xabfapls.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2tmbnamwk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uuelxvym.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2eyyuypuo.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2reitgjxm.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2lmpywjqy.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2bqsqmhci.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2qymxdgvv.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2bseizboo.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2yuomvvfp.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2cixpefby.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2jenagbzm.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2fsjosdsc.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2xomjugmk.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ypcmqhfp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2jqabyfin.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2oeqapryk.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2jtuhpvaa.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2qtdivlje.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2eaosrraz.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2aifnrtqb.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2oqysxbnn.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2gqbziixj.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2qycwnsqc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2lbilvavh.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2gjcfhmzn.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2ekvyffam.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2miuxpqoy.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2mnwjwwwn.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2lialorhc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2vnqglqru.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2qxyfxbmr.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2wyevgfrs.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2uuenqyeq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2hexlpunz.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2fngglrkt.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2tkjxnbwk.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2mntmezlw.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2xkekcchl.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2nbprzgnl.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2valtmjul.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2swarlbjx.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2qgtimvmk.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2cavkokvp.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2skeugwkj.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2qawutbws.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2eyhwekxz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cxnfcsws.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fsaoxubb.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pqxexozv.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2womfxywj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2jliuoosu.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2bjnstbgl.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2stmchytd.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wekyihno.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ueyilsgv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2edrexzym.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2idawhwuh.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqjetzrn.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2gjmuyvgc.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2tufcmjll.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2cwfooqey.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2rndebchb.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2moqeewxv.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2rawwahxz.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2hbiytnpn.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2bhsjlnxl.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ogetrald.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2pbugwbsy.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2gtjqakub.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2zunmtski.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2aicrpnmh.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2rvgulyle.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2yvfvxpos.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2xqrjtqfo.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2cdyyfino.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2pfmzscsi.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bmiazvwi.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2mfpfqawf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2mklxicqq.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2zpifwgtg.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2mhzotzbg.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2xzosjvax.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2ulinyxtg.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2tzdpmvhv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2oxxabwrw.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2lajfldbu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2oycmthvj.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2xemwpqmi.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2cfssehpi.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2bfnxtoxk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2fexktwqj.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2mzvfeymp.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xufibtyv.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ganvefkq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2gmxqbpju.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2rrnqomza.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2rcjssenh.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2sqijhhkb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nhtlgjlm.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2mzajvunp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2puqpmzgl.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2wzajdcim.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2plxnonrl.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2gtimrkue.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2zohrazem.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2xbuzmlxs.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2syluqeul.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2kjacxgie.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2bdmrglcv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2wqyubvnu.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2ztugsmsc.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2gtdhalbg.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2rnsscqhh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jecldemn.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xecgeppu.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bcglvuoq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2ucgmzoix.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2iygaqbef.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2alsfzywn.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2uynjcmww.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2wlewvdxi.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2hnyyuixc.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2gvstjrxm.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ogdhlylg.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2evdvyier.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2uugrmtsq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2nnvacgqb.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ffklhoka.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2wstciedc.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2guqkkezx.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2ecvzrkan.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2kwbgmuth.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ggbmnsxu.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2oaxhegxn.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2njiicgmb.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2vtujqeax.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2ivquwrlt.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2pthnelor.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2lruhadme.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2smtmetcz.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ejrfzucb.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xufcbkke.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2djgrkykk.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2gujdpjmt.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2mxmbmtek.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2sdssgxje.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2zuxbohpt.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2hfeagrnt.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2gnjxoncv.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2wvozdvnm.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ldonozfw.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2pflzphdc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2hmdqnxvk.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2nhfpnifp.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2klbehpji.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2beptlsfd.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2qdnuejyz.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jzllrbnq.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2iknpcldd.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ovehdpqk.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2fpknuivj.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2whkmtfqt.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2vvzqhhvz.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2jhepenoc.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2qonmuywl.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2bilvfmns.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2oztkkqwi.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2sxqmspuf.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2omjaqawl.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2xmzjcmtl.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2ivuxbewj.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2ibwvepti.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2mvxolwxc.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2dxlivnja.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2wvwfxbes.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2trdrmovs.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2rzbscrqg.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2egflxjkv.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2kxiusrbw.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2mknlagil.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2fkvtmwbe.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2gklngpax.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2owrrfkvd.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2nlkubwtc.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2pahubnjp.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2gltipivk.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2lloqlsbl.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2krpkcwaa.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2ohnbdipe.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2lodkbehl.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ioucjagz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aoehmisi.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2hwkywvqn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gptdvfdz.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2pictbftw.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2yylxgsoi.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2jgmncpba.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2emmqfzla.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2tfrvledz.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2hvszstml.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fsdiobnl.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2lixwbaqy.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2qrxpdwcb.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2dkmolyoi.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2psjvnkfr.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2aiuneaop.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2xktfrioa.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2epcipobb.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gnsrdokb.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2uosdvhje.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2gyzyjkax.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2flvoliby.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2jkbdzzxz.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2asebwqvq.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2ibnpsiye.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2mcxawgih.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2kpdnibzu.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2ijmxddma.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2aqvdigdy.html


<!-- 参考信息 -->