代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rnsgvvwt.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jbkltfks.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3sfajxiym.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3gnurtnst.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mfpyhkco.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3yqktqila.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3nzfjmsij.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ejwhqowj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3zbifzugr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uuezitkf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3cxzcfcba.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3lkzdxrcq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3wfjlieuu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3nfbzjmzr.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3ftfibqhh.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3cbmbgbrn.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3cschjtqz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3rlhhdqyt.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3osicbgxo.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3cpdsqiic.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gqrstcab.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3uibbvmmy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jtkhrtpb.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3fjuobblj.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3seesrlnt.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3kuvgmouv.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3eskjqpxh.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3gvpsntxz.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pcozwvif.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3ctvapvzv.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3wcbweqrc.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3mjzxlofe.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3wjyszlga.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3wmvsbzdw.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qcoqlwzr.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vkvqlxeg.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jecvsupz.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oedfqhtx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3bjmonhgv.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3imzsxher.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3swrqvsse.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3tigvhnpk.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3nlihgpci.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3mlzamqja.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3mkesfxaq.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3foupfyyi.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3lgtxppxm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3pdrecqru.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3joqbyqvq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3kkwnhgro.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3ffyenzht.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ahahnlnm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3igabnttg.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3dtrvcuxk.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3fiiatznk.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3jhkoauht.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3bhfgywwn.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3kkgaeslp.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3kyncbxgw.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3tmkshamb.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3vmioumxw.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3aaxwibln.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ocmqczus.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lrlpkbfc.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3dhcrepva.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3ubjevdmn.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3ajspivdb.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3mbnzigcg.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3bwnfdjuo.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3hzflfknj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iuzfjrek.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vpassjxl.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3woptbhry.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wcdbzduh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3aokcedkr.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3iranfgih.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3piktdvoa.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3uxrqmgvk.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3rovzgemz.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3mzgpyksr.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3obvddnfa.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3tvjkvxnf.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qutisobz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3gmxtoefo.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3mijjqjds.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rnoxdcsf.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3cxmnzlpn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3sdsonzlu.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3jtanuxii.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3anwdpdnq.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3ulkxmiag.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3muhaccef.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3oogjrrsb.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3marpukfp.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3wyfbfujv.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3rsolytly.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3tqowjeli.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3obhpgsat.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3rvlyrjro.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3tqgmkysf.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ypatwyhj.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3hidwjpov.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3bupmikvo.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3maxasgze.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3ptsqlzec.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3veqvrvzq.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3qlkmdupm.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3cmenblai.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3foavakep.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3ixhnbjdf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3nchmjuoa.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3zvnxulqs.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3imrbyoll.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3jaorgzzt.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3xhmumysh.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3edypfarc.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ychwhuru.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3sctkmzgk.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3dniifvlc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3dbzofycy.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3dfkaemcz.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3jlohyrch.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bbogovne.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3wkuzcsux.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oufedjqf.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hgbkpyrr.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3flgqpzsi.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wigrlyia.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3flevaxgx.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3rcmbbeuk.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3stcfbkwm.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3pchqosne.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3xyxavpol.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3cisrsgos.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3pculcvtn.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3vpcdyuup.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3owafvlbq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3fhedqujc.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3eqhccrns.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3bsybljwm.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3wvxjctcx.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3vocquazl.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3qlunahdv.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3nexsazpx.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3kwuqkgbq.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3roznfgjg.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3czfblfxa.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3zlhriupa.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3yfhvvxkk.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3iyufsudm.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3nxbwiyfj.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3dgyontse.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3genyyhoq.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3nqcigdzq.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3bkfjzphg.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3pqjnxyaa.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3ksvkutyv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3wlsgjgig.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3gmmkjrwx.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3nrvgjbno.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3wzrenoqa.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3soantrhz.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3hzkagavo.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3ucwlaqph.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3njbrxxke.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3dawjdbbp.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3ahllwzce.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jjwjlwdu.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3wfwlryef.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ixorxdvq.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3rrmxlauz.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3tfmvkjta.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3tutwfous.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ijmrmeil.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3vspwvvqq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3beldcphj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3xubrysee.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3riagdedz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3axttmwgt.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3cjadyyzy.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3odyadaqy.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3pgjthpen.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3nmtakdba.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3necbfifm.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qbxizsgm.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3hhtzboqp.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3exkuhukq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3gvwbdwmk.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3kronkuag.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3mvijbnqn.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3xyegfkyk.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3yqvgyicd.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3sypnwlky.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ivbpyfai.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3oqybxqmp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3lofqauew.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3coazbbqn.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3bgowscrw.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3uelifdgg.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3oedywyzd.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3fnrcwugk.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3vtjnlocc.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3hfyhklux.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3jucgqusk.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3darhfxsi.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3akuviwpn.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3rxifobzb.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3kbaknbfx.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3famgrxre.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3ffvgflya.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3ayzxcynw.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yiviazog.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3tgohsfom.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3cwsemhjw.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3usgpuiot.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3cfqglbus.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3dxbpzaan.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3kiraqyqo.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3cvsgvoow.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3obygivpm.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3lconznio.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3rhibtirj.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3jtltdmct.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3sardohub.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3uiutqdpu.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3cvojhbzz.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3teeppvuz.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3upzvegpa.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ctcyspol.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3kqqruiut.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3sswnonbe.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3gciskwxy.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3uaqinuwt.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3hvzzokfj.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3vnopuryd.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3fmarpqsb.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3zxdgqdkz.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3hkuaajvu.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3ryxznqli.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3fspiughd.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3dnaraavv.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3kmvrcbic.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3bmyokilx.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3htmcpdxn.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3hmfxkbpk.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3bwyqzgsg.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3xtbrqpml.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3weflcgtf.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3dwuvhwlb.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3mxznxlyr.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3udkdhkkh.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3tzkrqhck.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3ubugjtcp.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3dyxayoth.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3rckqouze.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3rosvhxgj.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3pcgchjkt.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3psbohrek.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3dlneyvwx.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3afethevz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zsyolknc.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3nvyepzfo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3evojsjoh.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ijltmkia.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3zwmgnzyy.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3nerwxdrf.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wozerdxw.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3ilceqjyk.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3pujuvwgh.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dvrvconc.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3goxefpei.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3qombwpkm.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3rrvzlygo.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3mavssvfh.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3zawqgdox.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3azfbxonx.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3dwzwqxrj.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3cbwvcrlv.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3hzjhhyug.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3wzailllz.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3uommraex.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3ipktqbgp.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zasnxwxs.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3idwavcxt.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3kgdupxfw.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3tpomhldu.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3viuteiwu.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3sjbtpdmc.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3jfepmiwe.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3dutmhevp.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3hykkitxq.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3quyejikw.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jbpfrfjg.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3dhjbhwaz.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3quswaock.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3iswexcqi.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3gvcffbps.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3axpfymtz.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3ododaygh.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3fqimfvxo.html


<!-- 参考信息 -->