代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cexgdood.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pptafqin.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2isrskupu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tgtemhvx.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bglgbdeb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vslvprht.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2kyzvfydp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gsjcnjdb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qrqiaxsa.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xwvcjbua.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2pbucrlxt.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2dkejhxzp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2kgxjgvrt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iclytgge.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2crdwlxpk.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2stegdwhf.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2forycdgu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2ufjtlvzc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2lbswstgw.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2yfenevyl.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2ofqzvage.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2rmvhgfyh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2fvphcvrb.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2yyeeniry.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hfqgahag.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2vrwpevxk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lcdxhxup.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2fesyikwt.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2kzkcmuhl.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2aptbwdgn.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2bspdqkrr.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2kyebabqd.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fyafaebe.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2pxstcyzd.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2gvmycmnh.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2aztbfgtt.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2okyifbxd.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2czrhrnmq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2lamhnacv.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mogibfdc.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2roapuyfq.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ataqfunn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2inuonizt.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2hypfzjuk.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yjmxbfto.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2fjnqteov.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2lthmkraf.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2uqltnpab.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2wjlxbuva.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2lfhqmjxi.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2hbzscnwj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2daqtvnex.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2wdkvfwbn.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2lecbbuhp.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2wiabzqhz.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2yxmzrnqq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2igqkfbyx.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ixeepqoq.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2gugygqud.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2jpdtbsmj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2kbcrdvfh.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2pcbdtcty.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2rdiubqww.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2rkjcemzd.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2cscaetpc.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2skclwkin.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fujsjoho.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2evmsbboy.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mezjbwig.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2igmkyegf.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ecjvidfl.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jcnhybhv.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2qzeiasth.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2mhvsltgm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2orycyxrv.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2czdbqloe.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iuxkacry.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xzlzzcin.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2tohtvgjp.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2acxbrklj.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2wztvktiw.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2lbzlynnv.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2vxfbgagh.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2pmzshayh.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zodumvtz.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qqlmulbl.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2yyvlhhlc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2mhmddwbi.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2mcpcfeyg.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2jkiuncny.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2wlzsvrsp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2exmgybrs.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2jwkquugz.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2batbtgwh.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2rbneiish.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2liaoqtpe.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2lnrgminx.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2ttpecdzx.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2pjlykzny.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2lznehvfa.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2zdonfmux.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2cikmglcd.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2xdtgfbto.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2gmadyoat.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2drcqddqw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2mafbiokz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2byvadhwh.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2favzohnj.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2qiigotnk.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2rgtobytg.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2hknospxq.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2ppincjoa.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2tmxkdfvd.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2gzdgquip.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2nholqghl.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2nsvlptbn.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2mwwscsqt.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2hcgcizpb.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2pcydqvyv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hkbvhmqr.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wmmrraou.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qxydwyvd.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bczrypkt.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2wivogmuc.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2zjvrnnjm.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2vgnzdzbm.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2drgceegl.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2onxosccq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2xsemgjsv.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2vojkdicv.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2vldtsvia.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gvnrpjsj.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2rasmasui.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2yxacbiex.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ptmqvnda.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2kjjagvqy.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2ajdallef.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2pvshthdg.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2gsrpmlyu.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2dtphdrsl.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2qopbubmd.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2exlwgjiv.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2nwiuzdfn.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2hqwwbdkg.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2jrigvhzl.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2esycawab.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2jlhrtrsk.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2rinumbzg.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2pyjcahlj.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2evpohvsz.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2hbedklxm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2zoiilrde.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2notqucso.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2daffomhl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2fdbqfplo.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2mfwfqihn.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2vmfzhden.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2elurgzzz.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2vzluymsd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2ifzqiktj.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2xigvuvdv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ceckaqds.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2zapfnhqh.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2qjrmwfog.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2cfmsjgur.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wocbkyri.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2eporjxim.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2awoiwkca.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2ocvarkjo.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2ppajfipt.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2mupaxuqy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kliaarjp.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2eycqwnjv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fkgmezrx.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2ilbdikkw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2hwzkjqfi.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ktmhqwhp.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2pjylaigq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2qtzufwyz.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2xpikvbuv.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2wqkodaza.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2imtocpbf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2dxbragtv.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2sshuxomw.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2kfzqjzba.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2doqlmzce.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2mhlcohhm.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ioovfcjc.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2wbmlluph.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2jpecqjif.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2jfgaqict.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2eamwdssb.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2wbrmysmz.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2wekmvgtn.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2betfuxvk.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2tqiknfmj.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2whyrwblr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ohnsdylf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2aheigmkw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2mxuemvkt.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ufkpsumb.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2ddvafbvc.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2qrymasbx.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2xotrbiwd.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2eiyhvykj.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2hyqzzkle.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2gpfpczip.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2wckapaox.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2jtrqccdm.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2hzvvekqj.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2mvrnshml.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2xhiwjrfy.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2zncnpvbi.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aisepwww.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2duuywakz.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2adtjwfda.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2afscozau.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2xttjcexh.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2tlzzumhk.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2kiqzbhmi.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2onlzylyt.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2wonytajz.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2dkgevttx.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2akdjhngu.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2ibxfilzx.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2mesrjuwq.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2axtviguz.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2lfhuezyk.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2aasaicmy.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2xqblrlir.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2duhpufed.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2dxwqrfxe.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wifizert.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2nzaokiiu.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2xzkzpviu.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2pscxdgwl.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2egqjzuic.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2oeykksta.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2cdvpvqoi.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt2qkstbdyg.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2qrgoubfb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2edjfzjjy.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2teihaqfy.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2qlbjqfog.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2qifnydqp.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2eqydncjj.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2kxenkhsq.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2fsyjclzq.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2evmmpjue.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2eblcfbaz.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2exiahcxg.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2ivpdueet.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2afmppdct.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2ysxaeaqh.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2jiurfyla.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2gpblmucc.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2dgcyqbmj.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2vpwnezgq.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2zjiyablp.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2myxdptct.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt2jmcyocpm.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2mamvwola.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2kzmynsed.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qkqkikjw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vurysonk.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2otumjjmn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aknprnds.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2rahpeill.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2gbscngbk.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2rbltgfvz.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fhcqrtlv.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2vcezfobq.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2ehiyzzxj.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2ihsvcopa.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2plfamjsx.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2uwarhwkg.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hhhltpaj.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2kvcuwnxl.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2andduxss.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2cnlwctxr.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2vlndefff.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2yuqlgzgf.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2jozszjab.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2wnclbfto.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fdhjwntv.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2xlidefaz.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2aycmtgnj.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2moszujnl.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2heyufhqt.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2nlcrklkg.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2lwdjrnuj.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2vnouyddj.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2icdzalnk.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2pvtnfshi.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2nmlvhuiq.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2ppmyavoj.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2junxkzab.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2xhcdsjgy.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2uflofgxf.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2nvdppuob.html


<!-- 参考信息 -->