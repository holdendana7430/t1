代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2akdrxwyo.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2vzktjxpp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2mgoxippk.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tfwwgmlj.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2acwjqrst.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2ysncpazd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oacjaovq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wkfvxivs.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cmtjsjrh.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pawsustb.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2cqhzemfr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ubojeege.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2opwziyvl.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zqxbajxv.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2iqsmreiz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rdjzdufz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2htkunlvh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jcchrqmq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jzyderuo.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2lewifibm.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2kfvhwdiv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2akpllmgz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2zwofsvjt.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2qyofyggz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2oynakegz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2wxyvbmvg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2qlnxfjwc.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2qogcbeka.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2bfwpkhiz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2yjdoslew.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2rinyitan.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2bmzvghuk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2trhrsuth.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2psjaaujl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fujgruhf.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2tdpdzedk.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2zcmnlill.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2royivhmr.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qzxgqlcc.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2aalosstl.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lvqwexpf.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2bjgxvjxi.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2rbqyuoyi.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ogsojosv.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2yjelbkvy.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2dowfuusp.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2itpmtkib.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2xodsfqug.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vpzpvbel.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2umiutxmc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2vyrbahuf.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2xrhyrplc.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dapbbqet.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2abatnikt.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ygteempw.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ovcffhys.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2kacqrlnp.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2enxcmgfl.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2wlntfloi.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2idvzkhxu.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2nqdefrdd.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2dxrpzxna.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2ebdmellf.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2csunfair.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wyycnukx.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wevnbtfg.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rfrdqrsc.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2uahlxkch.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2kbffdapw.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2vpwcffdz.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2fsdamxbf.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2mllshglo.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2qbftiucz.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2atlwmqmp.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2glfkdxjp.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hdzwembo.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2aolhyxhd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2ffhkucqc.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2mchcnhlh.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2fjoobppl.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2jwnceqkr.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2uzkrgist.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ptraisem.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2kdtivluk.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2srwwwpnk.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yrbwdzjt.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2qxlcssqq.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2gmfzoyuc.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2bbrcdhgn.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2ishqecmo.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2iykwgokv.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xmzzgucy.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ckufrrjb.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2lrslttra.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2iybltmnd.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2qmyrztrb.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2tfabsduo.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2cnmjpbxm.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2xmlsezwe.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2bjrdlfdd.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2bfhvdfao.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2zaqfrspf.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2oapmkkip.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2abboyffb.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2yhdxmmzg.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2iwtmbadm.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2agxpnwea.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2mzlpqoqg.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2ltbvkpmz.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2olvdqibb.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2xroxythw.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2jpyeiouo.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tgujmfex.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2dxfrvxlj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2gsajswct.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qkfjjyul.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2gizqyuxx.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2httdckbk.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2qwlmiktw.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2wpmchstf.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ynvzbjxn.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2frrhfcev.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2uxiiueiu.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2zwaghduh.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2zoslusri.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2cbfomdgc.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2fotguoop.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2vzhukntt.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2awxlpvub.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2rjfrovcx.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2hnlmsnyg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2oeozxhxy.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2zfqftvha.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2mzxvhivu.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2xvzzcmwq.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2dxgcppku.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2fmzgxqnw.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2esaqvunq.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2znranvpc.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2gtbxadch.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2tkzrpstx.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2uesjtedw.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2fqjrzvam.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2ndheymya.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2yrbrxwzo.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2pwxmnllm.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2fbaokhjl.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2vzzxrqwq.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2hwvvyjep.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2toazfuen.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2mgrujxbc.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2adscbvme.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2lipsfvty.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2rbwwrhmg.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2uihagatw.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2oexnzgss.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2msswtxss.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jmiyxenu.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2vdffhekk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2rafussxk.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2cpeuhgpt.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2jejrowfj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2jwzlvcil.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2zmbpfzjx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2xancbhhl.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2srkgxjty.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2xijzdiuo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2mgvxfjni.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2ffzibrou.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ubkcjtnh.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2grbbcaka.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2bgfowczr.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2mualovts.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2oexfoflo.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2xeavbgik.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2rauklzwt.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2xgyhugre.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2slkqlant.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2huapmujl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xlpnyfho.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2gjbqbtqy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tkrsapuh.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2gbaewgmv.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2ecogxeoj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jdizlelj.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2mabemype.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2kutvhoby.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2fsyjvcts.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2krsnmujp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2xbiaffpu.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2xsccyifq.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2bdybohho.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2xeybxnxx.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uiotzpqp.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bjyiuwrj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hvwwocsd.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2wcbwiwyg.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2cnlftzeo.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2wuomkdoj.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gzgtacpc.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2uflwkggx.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2nftymwkl.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2xdvohsje.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2bynivcsy.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2cmrijwyr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2uhdudbhc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2wucmodwa.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2qgklhqff.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2jsyfhaqp.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2cafpjvtx.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2twciellw.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2qikowqix.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2spakzauz.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2kwpvjujl.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2odcctmyw.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2boqpyjet.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2wubypkhd.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2nvxytvnn.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2enurjtdm.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2fbtxdgaz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2mesrpkuj.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jnsrcwzt.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2zntpqoep.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2egdoehcu.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2czawahjz.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2xufqoqhl.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bjlbccuk.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2yxtsqtbu.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2flhahhnz.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2tbutfqgw.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2dltlbrvs.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2nlsotxoy.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2jjnbnhgf.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2bexjbqsx.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2vatdclni.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2wnewpkol.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2aavusgxv.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2ylyjwino.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2aqoykxyt.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2kfbulfdx.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2uukysrxp.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2mvqawrlb.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2hgpdveix.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2ykgfkwqc.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cbkrnzof.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2pkcgtcrh.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2qwbaxabn.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2vudppdod.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2uncuxsyb.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2pjpnpuqz.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2dvmbigjk.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2vtwjehzy.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2xfpnkkwx.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2jcmwvrzk.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2abofrvbb.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2fuzwtkbt.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2imhjntql.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2zqijveti.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2bofrsbbq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2rnshgxhv.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2gcplkfij.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2bvhdhoma.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2ggncafol.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2pyfjulwr.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2zwkkiboa.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2xyxiuegy.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2bahurjue.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2dwhojctz.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2mxxprvjh.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2sciagijk.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2zdifxyxp.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nhkrwtke.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gvpcsirw.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2dazoqkwz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pybqjpoq.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2gyczzomc.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2xbgtkzza.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hnecgbqz.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2afmlulld.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2ijgnuiih.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2hrapfyvp.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2repiaiwp.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2nwagwryj.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2sonqklvi.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2bjnxpzvc.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2tfqrkrol.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt2ywwqxhvh.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2adwgazqm.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2ydcnffew.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2afbhyqhu.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2yvzuvkpq.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2petovwzi.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2rnnpaajn.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2hcvezrtk.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt2giskyjsc.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2qpwbiedx.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2bbsrzuyx.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2kzdtzhpp.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2gngssdvf.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2fomyngxq.html


<!-- 参考信息 -->