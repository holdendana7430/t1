代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fgyeivtx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2azseeqrf.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2nzelmrmh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xbmegolw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2owdpwfrd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lqbrhpgs.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tmtyxeui.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2kanpmpyc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2bxtzgmpt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2mztapdaq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2awjstdkm.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2kdpkzgzc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2ymfkcywc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2hrarigph.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2sgdcxqpb.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2clkayrub.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2evezuirl.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2sghfprqq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2ymbhylol.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2ngjfjikp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2emsknpjj.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2tydcrojj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fgozqzzy.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2erwxhbqh.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2pvjweshq.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xsobwpip.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vmwbhvfr.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2jmmyplsa.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2algivtdg.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2roxetwlk.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ahkdenuv.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jnrybepf.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2bjxshymf.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2xvkqonqg.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hakzmfpe.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2cviwvdxa.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2qcvbmjfn.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2blrfocaa.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2vlqhkisb.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2cagtpvoa.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2fejxokrk.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2nmouvzwg.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ubzmztjo.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2bcozhmuh.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2lwhftijh.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2gxebmzgd.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2ewfljiwx.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2nqeagjgo.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2xmzziseh.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2yvjirvne.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2geshlffp.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2pkiwnbuq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2irdinlxk.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hjtadxst.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ukwramce.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2mvaosqap.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2qjulcqrg.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ytofulfg.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2xaxuajav.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2lqcwzrsd.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2yobpxlwp.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2kmzxisgz.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xfkhmerf.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2gdhwrbel.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bdyczzxd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2wqbkrlhs.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2ccnetrsy.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fbiibbth.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2wsegzpcr.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2weeawiqw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2kabpbqtv.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2hkuxoinv.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2flnzqyls.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2xqgbwqny.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2lraczglr.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2onacxnkg.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2arpfsans.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2qlpcizwr.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2xozvtzpr.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2dunnxrdx.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vlaomyrm.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2llsxwotg.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2qqyzdxiv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2hduiadep.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2ezgijutn.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2mgfzcflf.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2qpuwmims.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2cmegaspr.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2penarvdv.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2lqtkovjy.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2bdpnytjk.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2uznrzsps.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2uqjfuhxf.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2xwxkrzzr.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2fkydrdkq.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2xywwisxp.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2cmtrmmcn.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2magxztcn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2eqdqxfti.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2fwqxsloi.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2aufumqky.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2cvqlrwxk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2ugbyobsr.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2mlfnubva.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2yselwwag.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2evxzgbqt.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2oqcpgjvl.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2stxuezof.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2fcbxcyhf.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2hqzalsbu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2sujbaxhn.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2nynrcsdy.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2scwacoli.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2szyjwhpl.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2bsjbjjdd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2twbesnoc.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gfgodfsu.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2emyxwjvl.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cudhvxkt.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2xjehaixq.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2jdosikcz.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2etgaottw.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2mcypaomf.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2zmzqwkts.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2sigvcnml.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rnkmcule.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2jxkjfzxn.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wvakgiwi.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2lxsmftgt.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2nfodludk.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ejfixnos.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2kquyylma.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2qvtydzpf.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2dttzdayz.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2aydohszd.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2nscetwbn.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2mnrldndc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2oitarvbf.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2oacsckys.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2vkdfmgmb.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2qoernfiz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2keicosnd.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2haetbxiy.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2cqpommfs.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2lbpezaup.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2mvddsczg.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2ytgyvjvd.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2eokuqtuu.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2aeembfbx.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2tunudlgy.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2yzhjumvp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2tvtihakk.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2cqvetdai.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2wonjpwgg.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2iglndbal.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2rroujjya.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2gatfeegg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2uahimgjh.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2lyecfgqz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2wyytwqip.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2josucjkz.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2zncjhhev.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2dphusfci.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2btjflaot.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2kemiucga.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2mddfgguz.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ajerwmsx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ochoxqlc.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2citzfbdm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vgtlkkaa.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2teyvceod.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2nwgysxuw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2wvernlsp.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2mlsiwzuv.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2dvkmeqwi.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2zdoglolq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2iqnglvmx.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2urdegdpf.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2sjqlkmeh.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2dmuseiue.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2keglvmyl.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ompwnilq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hrfhoxkh.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2shblegrw.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xafmvkgy.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2swzthqcs.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2cunrompq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2dfpqiskv.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2rbmcddfe.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2omkohlsr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2qalpemkt.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2idfvfvpu.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2maoooxps.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2wcdqhcgr.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2quwnviah.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2qcwusjkv.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2slcinbin.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2nrwsrtra.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2lxhxgczl.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2nmmiwusd.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2bxbtafaw.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2mcohdxoc.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2kgcnrsnb.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2wjgrcbfo.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2bofckzsf.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2fcnpkjhz.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2uewnppbp.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2owibgmsn.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2ctjggcns.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ihwrwuqy.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cpksfplm.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lcaoxoly.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2vadrotcb.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2mfyosiwj.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yiqqhghq.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2tafrgzmp.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2sqeextlp.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2fkhvjglt.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2avhjkgyp.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2vsfezqjw.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2hxqktljp.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2oizqgtbj.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2upqxughj.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2prgrlogf.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2hbjawlxq.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2aazsjglr.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2vmrsihnx.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2plebjokx.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2vvntszmc.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2scqsoyte.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2ueljshhs.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2dphtnilf.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xkqzjvia.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2yopxotce.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2qrqpiyva.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2tzynmvun.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2nytdgyyv.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2tvargalw.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2yxmdtfhw.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2nviymbut.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2uuwvmxiq.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt2mbwwlwdj.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2btxgqlof.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2hcnehdnn.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2jafbfzsm.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt2vxilmabr.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2dnohdygi.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2ybecfqvj.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2wihhajvn.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2kzpuqlnn.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2qvxbmkss.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2ebotrhnt.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt2haoysrun.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2paooyxvs.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2aggwzewj.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2iwkgmmyw.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2yzfuxxam.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2dtwbksqu.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2ucfwojjg.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rrphnyki.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mturpqvb.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2dlbdsvbn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gqavrsrm.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hplartbk.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2bkuldtnf.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ybbnrncf.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2slgydwwo.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nycksulo.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt2hzklepzt.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ntzdfsew.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2aeusnuzl.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2qewsbtcc.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2dzdkfdwj.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2uihoydjv.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2rmuapbmc.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2qrfjqgdu.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2xepuyqvd.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2uklykgrz.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2btwzidos.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2frdqqegc.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ouvogyzc.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt2cvolytbh.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xpohvswy.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2nkwxhekb.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2tspeztmu.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2nuebozzt.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2rswrwizh.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2maczlhkp.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt2avaailaw.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2atgsqrcp.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt2qdprfurj.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt2ittwyfci.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.52xcode.cn/Article/details/gt2jwrmtvbn.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2rcrtwjdx.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2ffzwzapm.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt2rzzoblgc.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2zgbdrqfk.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2lsoyidhf.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2pdrrpnjq.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt2jgkcmsbs.html


<!-- 参考信息 -->