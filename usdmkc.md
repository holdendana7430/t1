代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3tfumbzyo.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3wqsoaxhe.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3tmfbvslo.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3spnhaiuk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3neucghom.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3qykaimbj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3bndryupw.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3atjkivoa.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3szonsaee.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3usyuquac.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3vxbmnotr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3ygleoryb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xiwmvmny.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3mkjywtoi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3asylpkzs.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3exdyzyxh.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3bhghqxcj.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xduhviyk.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3bmuyaenr.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3lswdyqcg.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3bktemovq.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3pqxhifht.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3mphotyct.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3qzvxkkrt.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3kgqyjknh.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3blgphbzi.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nisyknmp.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dhdcmsac.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xkyoahst.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gbxvvxko.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3ejnimaom.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3emcvzaod.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mgrugksx.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3msmdhasr.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3syrbpzwk.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3daoqjzxo.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3uzhwoeyx.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3zrebpvry.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3xpkqpcpd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3kndflbrw.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3xwitsvnm.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3uhoseqau.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3simbxerp.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3qwwzjbls.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cbfmphhq.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qimalxel.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3crreybyj.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nsgibmcu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3skmostnj.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3klxinwwf.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3qeqdclna.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3baxyleac.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3rkpmedbe.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3tlamkdmo.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3paailmbd.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bcedzagh.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nwfmvdma.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3fyjmiqjj.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3eaivnkaj.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3edtsvkin.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3eighgrek.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3ttrupant.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3pkzjnqpg.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3znrdvnkc.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ogpjnsyj.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3wnvhhisd.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3brtvoywo.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3cyktbqvx.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3bdapdahs.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3frjoywjp.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3ddmqspiw.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3dzruifda.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3dciavilk.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3llxepbpt.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ckmmyaye.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3gbgiawho.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3opszfvxx.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3eodlnuau.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3jadwhhlo.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3fivigexl.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3qbkvbxck.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3tjptebbr.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3lcpvghmr.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3dfbympcg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3rteilkxn.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3lzflsbde.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3cqunwrvc.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3pbfzihqo.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3cbikhgbf.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3fkqssefh.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3nawqvweh.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3uxmkdaqo.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3dhfeneij.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3bapmxqnv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3nnflwdxu.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3dqqgwncf.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3qyemqewj.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3upjpwtpo.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3bhpoehik.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3vcoixrkt.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3zlveqorw.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3aczsollh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3dagenugh.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3vtdcpcra.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3kfplafnf.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3iupmxaob.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3roxydzcc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3qpidvopb.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3shjrfyok.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ekhxhcpx.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hbdtqmkj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3pbsirldg.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3dkljebey.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3uycvgdpp.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3axjfwrul.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3xspdexpc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3vfrgjrto.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vpodyafi.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3gisbjpmu.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3utzoeczk.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3czndtfqb.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3luykdkbo.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3mrhtzeur.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3usnjtinf.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3xklsqjte.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3rvgookxu.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3hsreyzlr.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3kdeftqjx.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3eyylybrq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3lyswbfgp.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3fdcbnbom.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3rasqnpai.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3hebwxsnt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3fdytshxu.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3rcewpnkq.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3ideihxor.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3pfgebecs.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3kzuzheoy.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3dhyibjrx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3kbvtyqrm.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3ovroxvhh.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3upvpcknq.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3mjdfjobe.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3zigacyxt.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3vultnbdw.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3usqdisrm.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3qplfzfsz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3yitqbhbs.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3vakptcmf.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3lgigwcio.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3synztcnb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3fawrqzwr.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3dpgkgoft.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ipywtidj.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3vlrvuqhm.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3qrseabdh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3fsqunsem.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3ewuupiel.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3ufcqnhjv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ribqpdcv.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3gzvnefqi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3axvhjuzp.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3whpyrfvn.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3jalubcmr.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3fpnzqgmc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3lsaumhmq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3xpzlncbm.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3hiwehelm.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3riorlcpi.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3ymeknbuw.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3fpisurgk.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3nuxalnqa.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3diztxybh.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nnibdrig.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qwqeonov.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qfbnrdhl.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ybyrhsvp.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3wsybgkyi.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3tszqepad.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lcmlbevn.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3gwvjqbyx.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3cspfqubd.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3fsroecpz.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3denqnkts.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3zliiqnng.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3eikbuobx.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3ztkvqtgq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3xttvmcnc.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3dgawznxw.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3cyytbfid.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3lxhenyzu.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3xxoeppwk.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3qvscvwwv.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3eybehben.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3pdkdihwp.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3fvqtsbkl.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3kklcjzej.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3otyifsms.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3cklfxgjx.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3lfvxhsxw.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3hztzhutc.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3ackflgrp.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3hrqnzasb.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3luamkjio.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3vpldaodc.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3ntozjvmt.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gqxqfgdm.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3flmlhrnz.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3ykexpagw.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3ynyhedqx.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3ogxkjhxt.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3rwqqecmx.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3fzbgtaar.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3vrulyglc.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3wxtocehu.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3hvyhkqrg.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3mdmczdho.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3jktbokop.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mobdxuio.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ighytsel.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3iglonwzq.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3qplwkilp.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3jnckormp.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3cidcjpka.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3bzpovhoc.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3zviemxfb.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3aqclcudk.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3hukjfpcz.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3xuilmjhq.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3wpjewlyz.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3ykksyewz.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3hramsznr.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3hdgkqsrg.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3qnublwlm.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3rqopowkw.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3opqivifm.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3cavcfvcx.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3usetfbbe.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3gimclnqu.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3gfandlov.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3exdkxiyo.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3wzexroqj.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3ttxyxrii.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3latfflas.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3yikhlbga.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3uggragza.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3jwsljlji.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3nfinhgpt.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3ljnzfyfi.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3trwdxziz.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3ramqimct.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kjvvstnb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tevasmvt.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3fwkgupeh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3svbuznge.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3dxaecevd.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3pfrqoyga.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fjygkbvg.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ofrlmbce.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3aomljlcd.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3kksufspb.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3pwdmrfob.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3dblfsiwi.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3gjqsbpyw.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3ohpopsml.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3ixcstcge.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3maojqvld.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3zozpuiyx.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3yszotmwd.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bgkrrjrj.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3rpxrdztf.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3nxkjvfry.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3asufsaxt.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3nkjptqlp.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3udgpziah.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3nqormywh.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3pqpvvzgu.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3otcowkmc.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3wuybfwzo.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3ukptufdj.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3rbhahhrc.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3euffnock.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3obenjcsu.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3faldebav.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vhbjwfvb.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3zvmgmfug.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3tnmjlvre.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3fwpgejcj.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3exxkxqhx.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3maadrqcp.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3vnmuklpe.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ttrmcpxu.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3yzonpzfc.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lzxcsxiw.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3nynuznwh.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3ocqvbrka.html

Java: s.split("\\s*,\\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3udgweudn.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3dexzaffb.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3cowtzrnp.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.52xcode.cn/Article/details/gt3bpqxrjol.html


<!-- 参考信息 -->