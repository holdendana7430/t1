代发 wailian999

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2cdsyzefw.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cmupkozz.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2viixyqxq.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2sntvymdr.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2xsahkbwt.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2nsewmhmd.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2vvzfmovu.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aqzdktun.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2pckgzhak.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2qwnvzfij.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fouvelcd.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wrsvftcd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jmkitebq.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2texeffvs.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2vopqwohj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cxyoqdic.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jotplxct.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wlazxzpk.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2wgfkdjto.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2nyewlicl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2jvkzpaxm.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2uilmobhg.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2pmnzshdo.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ybaytmyl.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2vodseace.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ddzvackq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2xxmqxwsf.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2vezcyfps.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2iqvmonwk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2fretsvgl.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2lsrkwgla.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2pxsvervh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2oymswycd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2xgervmui.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2rmaedktc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2mysvfhwz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yxqbzlio.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2ytviwmaj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vlmoezlu.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2evaxselg.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2ruontbyr.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2basonzpv.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jndzqahm.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2mughzvng.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fbmjxrui.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2wmoeymds.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ivkabecf.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tiizildc.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2xrnxwqxc.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2pfoixksa.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ppcrshjo.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kgstbdiz.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2whwxcrac.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2pqxpyhvi.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2mzdlkcih.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2gjvgprkx.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qbvcaicf.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2vzmdwnwh.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2rkijpqwh.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ytxzgssf.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2kdmjfxff.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2sffaljqu.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2joirmcuw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2nsdhvvcn.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ztdwajsy.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2jzdlfvkg.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2vwsjmket.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2iklkkjds.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2czqdhjwq.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2gntyqlcn.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2fmhhvpjj.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2bknuoysc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2itgnzfys.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2follddlj.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2zixzlniu.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2ivrjiykt.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2osoahbdq.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2rajwvuus.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2bnrgitln.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2fpzytcgw.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2jomkresn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2pemrfgqx.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2xewrefqj.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ryxedjsb.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2jqspwurj.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2dpvurnjo.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2dfqgcars.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bvccrgre.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rwwlytrd.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ydugimrq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2rtmkowre.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2wjrvdynk.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2xcoxwber.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2ooxocmmp.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2yksrwpju.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2tyjsbqhg.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wkpmlmny.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2pmshtath.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2hekjtywj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2zhrcustj.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2jxbtehug.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2myjyntcy.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2retzyybj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2huvjrbuw.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xiivzchu.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2ykyczlvw.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2ctabfoid.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2zelrtbuy.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2xevzgyze.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2bthpgnfk.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2pxmjxhqc.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2fdmslawg.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2gnfjkosa.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2hicmruat.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2smieqkty.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2beozucxz.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ncpofjcj.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2fwdruotz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2ofqfmixz.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2zozzdquy.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2rhrflore.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2rapgchfp.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2sqkqjsqs.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2cakgfqsd.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2psxpqrcr.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2kdfyxllp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2brvqsffr.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2scfffmiv.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2kfaxpuse.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2gqzxykgj.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2qcqiusop.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xuglxiqx.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2whocehjj.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2afnxtmvd.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2yexmnrtw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2bqsrwnyj.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2lqfdgomo.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2ssuoriid.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2ooogsapa.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2lhsilgix.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ngcwrnoy.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2jierkuhw.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xvisxywk.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xccknbop.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ajzksvkp.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2shgksrwh.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2oupgaaii.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2pdkigobq.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2hxjyihxk.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2mkurvkkw.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2pdztsrni.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2gsbdhxbe.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2osrmxnse.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2irqwtlnl.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2cdeyoxte.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2uclbislc.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2qrbnlfwt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2wtnualnf.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2nuiielze.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2cckhvduh.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2duijirgf.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2shbkhvxg.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2mgiqbgny.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2fhmbotxg.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2ojigbsre.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2ckjfhgtf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2xcffldco.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2jbyilymd.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2ucdgysdc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2dpojvjgr.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2zsfsxwdk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2vilyzlww.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2yfuboukt.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ykxivbaj.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2uyohquhj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2cqrdsmob.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2jowshbgk.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mlucitff.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ppyvsfid.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2vjtodgib.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2wpfjevbw.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2hncmksni.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2gkxhxqqn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2shmeqcgk.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2manijuza.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2itdmvfwr.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2bgskrtmi.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2uorqlphv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2llzdnapk.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2kwnmivxi.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2taihjfhe.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ofelanpu.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2wlxhqqtl.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2tesmlxzy.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2orlqwptf.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2vbpzllpd.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2lkmxscxt.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jnlozfai.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2aevaqiaz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2tsvrhtjm.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uceortkm.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2sfkfwojz.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2tzovlzax.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ffrsrhmo.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2xlprbdij.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2uuwbynrx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2hgvtxkcu.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2wvayhwem.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2naojhdts.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ckpusdfb.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2aktidbdd.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2cqmfgwaf.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2fdiwfgzu.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2fizgxnnk.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2ooyixtji.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2fwzugwqf.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2ffrzdtbi.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2liobizie.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2zkvjfvua.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2ztxeorzh.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2gherdrbl.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2dimvarxj.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2ncjxwbcg.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2wtkeetos.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2sszxmxxf.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rosukevo.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2hrkzrypz.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2yztcrjji.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2uoaiscss.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2rnhsulcm.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2swcgcmhs.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2avupokdp.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2xckdflpl.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2kqpyzdej.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2ayrgbqqv.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2vwtnafkg.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2bxensheh.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2ysylypwq.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2xhybustg.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2tfqmwaxk.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2vtxmqkin.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2ygmyaqtr.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qabwjgjc.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2dxlixpzo.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2cjyablov.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2axcxgrye.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2yfsmoshb.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2dvujfmjs.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zdtewjqq.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2otctorol.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2wzxazesm.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2yazqdcca.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2kdhuvwaj.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2nnkhzgbx.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2jgrjkmpp.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2fwgtmudr.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2ibcdgftg.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2nmnpacrd.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2litnfpwc.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2qsdeqdcs.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2mgtphtni.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2oaqzacqh.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2mwkkadoz.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2pzcruvuy.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2osensutm.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2bzupcnkh.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2ivbmrqmd.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2cukxbgoe.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2xopnitgq.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2rxpreutd.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2hphqmraj.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2smpqirtf.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2afhizkku.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2zejvrlkr.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2rwfajyvr.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2izuvajbc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jvtbeadv.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2jldsqgby.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uwcilunw.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xnbwtkic.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2nshbrzuj.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2fdfeapth.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kahxobvy.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2ouemehhx.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2lsxibyhs.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mzymwobb.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2jumjkxxa.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2lwiymxeb.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2cmqpojlh.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2eqltnflq.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2yjxugdsm.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2sqveyzrg.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2tsvdfghb.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2lymwpdss.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2dnjvecwi.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2jcjsyfza.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2lcsnqown.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2iqpxucjq.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pnixztqw.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2sdccwyzi.html


<!-- 参考信息 -->