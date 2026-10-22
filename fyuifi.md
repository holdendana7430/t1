代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ydyyhqok.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sisyhpnz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2mqoruvfb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rtrrkvud.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pzvihulo.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vynhzpgc.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2oxknqwfm.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2wpxpwqou.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mmryytzc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2czmmplyv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2rfwckpxm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2chgdsyhy.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2hcczqcoa.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ygfhcqhi.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2zjonwabm.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2xotmtdpq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2mdvrrbnh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2iqspqlnu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2euhklbxc.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2vnuufrnh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2uwjywhkr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2sdlfueyo.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2dbfxgbxm.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2uzbgdknl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sznjznpy.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2dsuexrli.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sldgxxyc.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2msvykgsi.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2gllcxtun.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2crpzxrop.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nneyxihp.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2xpdnpbso.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2mmtxjele.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2xvnokyha.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2wxgwixfy.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ivuxemna.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2zzvhxiuk.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2tnevvhyq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vibzanbq.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jyrcmypg.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fffpqfux.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2nobianmk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2kjjxybyl.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2ltszlufs.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ftkplacs.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2zprdmmfx.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2nksqxqfw.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2vkpdqjkn.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2sqqldjsx.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qojxckjv.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2rhflerlq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2gyfezxwi.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2xfdwggjd.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ovmpdcix.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2skyulkyb.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2uhklznhm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pfinivwk.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xbhbxggb.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ncmpnsfm.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2csvyshsc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2dbydlgoz.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2osxohruh.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2mkgmoomd.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2xlszomky.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2andmwtun.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2wttylsrv.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2holovooj.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2tdoeblan.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vmpymdvr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2eoplhhbh.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2vdxktgff.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2omruqlih.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2qkqqoque.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2xmqjoecm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nxmiosjj.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qnuibrac.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yyoxeqkk.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2tvcodghi.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2mgguyjgx.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2vwjvnmmo.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2qfgjrhan.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2ooxdsuiw.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2fsnlcafa.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gmmddmst.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2dhhjppzz.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2phdgusmm.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2podjviso.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2jeceslvs.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2qhvwakoy.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2tafyxxdh.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2ewahpnrs.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2jrdqwojv.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2sjygrpkv.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2rsqhecdu.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2smxiluvm.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2gkxstnca.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2mmbklhpi.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2zksslpgu.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2lclliqmn.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2nuokfvdc.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2uzpdahme.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2bumfoqyo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2zvgmgivr.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2bwadmdfw.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zlqedpzw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2vdsfvdiz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2uzavkesu.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2bynyerzu.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2jcrvsryw.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2dfkakxak.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2eoakgclq.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2megwqwek.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2uhewpqka.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2kpzsolqi.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2kgbpafbx.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2exwqeptj.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2qnrhmctb.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2unvyhugc.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2pughwlan.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vytozdgf.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2zqobhimc.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fajtmanf.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2occlqyce.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2mdflbjfu.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2agkvslhk.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2ydvrknyw.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kfzoiysv.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2zaortvom.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zoazshff.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sjiejfer.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2etifdajs.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2trcpuvoe.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ydchvoxo.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2mafbnutt.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2mfivnrnh.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2akyferik.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2ovugslna.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2wkjirpmq.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2wgolkrne.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2bqvxmdsk.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2zfbiiiem.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2iojxjxzt.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2ybhtztoi.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2ocioygjm.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2tlzgrtbr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2qitifjhi.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2pxqtehqj.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2kstovycn.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2spuniyrt.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xbrngupp.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2xgkfreyr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2ttfbgifd.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2xnvgcfpa.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2esgxvkly.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2ieagsiiw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2qgdjmdnp.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2udrpncti.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2zpbonceo.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2tpbpdbfv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2arjzojrj.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2yvxxvcfb.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2gaagdjmw.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2cmlqaijh.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2bzbirfdj.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2kutfudfw.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xhtzkspc.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2zkevmsdy.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2tmaveaqw.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2uqnomoep.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2svimywjg.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2ejzalruy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2muwkapal.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2vsrwrwyf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mfwkdzyb.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2skyqwnqf.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2yhdbigfl.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qxxtjuux.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2gudhshlz.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2oafchqec.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2clwevljd.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2wijkjnfz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2tmmkxbww.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2xeojljbu.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2ykdszost.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2avfykeaq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2clviahro.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zsvmqoxg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bkewrpht.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2tfbhirnc.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2xczfsnmj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2osxbbjkr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2zofbngjr.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2ihasvtjx.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2ympapbds.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2chjaymlv.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2gpdsioor.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2wanynbci.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2edxvxzrk.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2vkavuvhg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2wdrqpxdh.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2btikvmmu.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2ckivfdms.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2rblbcywu.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2kolhoqas.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2xkmhaamz.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2yvsvtrtx.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2hcumrshz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2warkionf.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2osjzmkld.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2beppmzhs.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2fflfydis.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2kdefpfsy.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2obyohkvb.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2xwmwifdc.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pmvbhpmc.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2kqtvimta.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2dbsqkddb.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2oeufknit.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2fycujmxx.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2xruzmohn.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2ncmwqnjc.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2bnzoiyjf.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2xbobislq.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2yfekuaxw.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2kejpfbdf.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2pmxjkioc.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2hjzqntke.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2mpkxgqmf.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2banikrlr.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2dfveewzd.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2rkugmcht.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2yovtzhpa.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2bjizinfe.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2xbdqitvt.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2hekchjsh.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2lecbarbq.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2gaadnknu.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2riauptfe.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2fljcnyni.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2ayvyhien.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2qkaqceba.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2obumxtry.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2tcecldbl.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2kilqaxqa.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2lvwyjmye.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2fenmryyn.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2atqsmhjz.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2ufwdehjb.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2ikhovfpn.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2lkilacdh.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2imxejsmx.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2lpfrbicn.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2zyljdzzi.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2pdbsciok.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2igawimdq.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2bcwvrsma.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2zrwqztxl.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2hsqpbrqk.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2igxnaupc.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2vavldehb.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2rkdysmcm.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2aahpditl.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2vmmuewxp.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tuphzekb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2frqhkkgp.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2plsdhplv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nqlpsaxm.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2wucphxsb.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2dgxzcsfq.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2vuvoeabv.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2wvesdort.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qbmtijxk.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2ceomxijq.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kdozzpyh.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2izgrnqfb.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2fefzajjd.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kjliqibu.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2uqddgtpr.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2peshndsw.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2kuehxsay.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2obiujntn.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2ihxlofpk.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2erlemvpz.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2mueipddk.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2hxvxmpsz.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2sijwhmmu.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2djebwwhn.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2dsoquxvu.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2lywyqsua.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2vjmotuvw.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2yxgorwgj.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2opvphvke.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2mpbijkoj.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt2vjzlejsn.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2cscfwjrl.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2qpoamlxy.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rlbopnbg.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2qyspqpak.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2ewvcywvg.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2cqbttibt.html


<!-- 参考信息 -->