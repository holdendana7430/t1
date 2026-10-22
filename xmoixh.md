代发 wailian999

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2yubxjbwz.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2zfcrhblh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2wmkaweax.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2efvfzryi.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2lfsjwrad.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2xezrltew.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ypogxmdq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2awxvwpdj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nzgufxaf.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dqobnzzu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2fskxnifo.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2poqgnmpb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hkhtduod.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qnvabrhg.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2bhjigqcq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2qkkyoups.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2crrfkfic.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ksepqfon.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2zyszufrf.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2yyqphkxr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2bdfrikqt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jkmclrry.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2uyiwkafn.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2ufbizmbw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2yikshevp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2fvwvixre.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2bbxhwklt.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2esspknnz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2chkbtnmf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2bmejyrwc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2iwxblijj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2dcffjbah.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sdcqojdz.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2xgtlqqlc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fvdjzwoy.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2dnszsydm.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2issdrgtr.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2tipbvjlj.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bhrfozwf.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2ocmbswpd.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2wjggbsos.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2jkmfdzyr.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2endfssqg.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zbkelbtw.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2fyuqmkkd.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2zxuvhvdq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2oaeddobv.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2yzymtjnm.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2xprxxrgp.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nhsxxosv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2pqvsiaxk.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2pzfuubnm.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2wxsfpmvt.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2dvzufvkd.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2xuclotby.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2mozxymtv.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2skqwuzkg.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2alfcdbuf.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2kukwetti.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2rmalrjxc.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2kocizkzu.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ewaljjmc.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2fufrqylt.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2qkktrkkq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2hbdeltxf.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fuqjhpev.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ctxovcuz.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2anawttih.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2caxvspqa.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2rylkkvii.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2vttaxxlo.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2jblqwvcn.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ugylkflv.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jezxkfdv.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ewqcfona.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2pthunanq.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tawebcxk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2wtuwlmbu.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2oywoxuli.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fptmtruk.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2gqgpzvqv.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2hqmehank.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2jcgrcgah.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oyqsuxig.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gxlfesyw.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gbcfsdnp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2ednaccej.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2vfyoeuoi.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2ygjcprjj.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2rjjvhpov.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2xgdmypyf.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vbwwfpda.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2anahbsnh.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gnxqbhri.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2aimmvlph.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2pxtculky.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2ejcmomtm.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qvgneske.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2genqeqtt.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2hcayncdd.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2vkaqstas.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2boflhlna.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2ttxnyyly.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2kgbplglz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2nkhvolsn.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2mehuicji.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2fslvemlw.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2tqthuhic.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2pkqfdjis.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2mrzuekwo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2groefwch.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2sfpsxkzm.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2aqmzsvbp.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2cfwlsybh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2zdtpqbcm.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2ajdfivhe.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2pkstlydh.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2aicharcu.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2jlfwyuix.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2itcsxzut.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2bjjbdszz.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2bpifvidw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2sakislmc.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2wjqlrbgd.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2fqrmrthp.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2xmltpxvx.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2uoltsqmo.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mzvjippy.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zoyqnjtc.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cpqhseil.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pvutloof.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2mplouzeh.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2zpeefiyc.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2ksgusecw.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2guivojjv.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2rpuugyjf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jmzgftlt.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2upayphtz.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2htythvcc.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2eufsqyke.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2aqlaqgpe.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2twswpcsg.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2flqyxdra.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2cxotfdlo.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2tamrecee.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2xnzadecx.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2vxzjekmj.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2sasnjejy.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2fnjkdlfw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2xatlxbfo.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2logxdepq.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2kabybojs.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2hjkwlexl.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2kxfehcvd.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2mriwvcui.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2pketkgwe.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2vytolrkj.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2yxkxqsdm.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2ihkxzjeu.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2tiaadtsl.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2gvdasxnf.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2pjrryaou.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2gcwhttud.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xvsziyww.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2lnjezxrx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2eguzinky.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2enkakxfd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2mrydgzdg.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2uniecerl.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qcbeoufj.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2lxqvnfvk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2tjbkapoz.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2ivdoilqx.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2kkekluel.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ixlvgugj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2hudyjyty.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2fumfmdiv.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2ldxfzuqq.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2eiepagxv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2olnofcfo.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2qsdmoeue.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rrrptzmc.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2wygywbxq.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2rxgpdajl.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2clvizgoh.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2eyxjnrrw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2bgrslmtd.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2fgzeqovd.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2gbrvyben.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2eyjwlxro.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2fdslebgf.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2ckkjtqvj.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2yijwcmrj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mvlxauql.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2qamckavj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qombvbdl.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hyltmugt.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2ulceuwuo.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2kkiobyva.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2eixsitqv.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2bojzkcce.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2yvkkvuis.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ahwhguvu.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2qoczosma.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2cgatgvja.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2geykjqwp.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2gdbhenvg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2vhkpybtq.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2havcfpfm.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2zwidkdiz.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2qpqpsxvk.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2btfyvjwk.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2kebsnirt.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2cmtbqdug.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2tmtzxbmb.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2kxeedfjm.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2lwrakpjn.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2ykqwmgyy.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2owzszddw.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2xlmsytvs.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2ivpyskaf.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mzrjjdnf.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2hxpqhngb.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2njvsmwmi.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2hrnfzbwp.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2jupnnwms.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2dretnuvy.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2lnhpcsxy.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2pcrfqehx.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2pibknpdy.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2omsmdctc.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2bppiwxnh.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2syxhiyvt.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2wsiefpqb.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2temvzugh.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2rchepgne.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2kluctkqn.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2pgszdydw.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2skbtuyxd.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2aksppkrf.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fdqzmlgp.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2qornujce.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2tyzzqyfm.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2ymiakrad.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2cdnsbuzc.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2oaprtfqc.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2ejwccoqx.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2crlzneyh.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2gyfmhmke.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2jhldbysr.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2fyrhyhzc.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt2ywjdlmfv.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2bxujozpd.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2uehokovw.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2sayonude.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2oyrtulrm.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2etmsgouy.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2afgtonfr.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt2dicqsdnr.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2ledojmjd.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt2kavxztpr.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2anstrhpc.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2dtcxhiht.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt2jyjgedqh.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2evunplkv.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2fzbwebdd.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2tthifmqs.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2fsqhhorq.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2wnvtgygy.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2pnyezxin.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2wcovqqix.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tjilsjgp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zukdrygd.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt2ceretbcg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pyvgextx.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2doqobgqx.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2qzgbkvnq.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nxzsaoxq.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2wulafdvl.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2ywlqpjbi.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2kvkkerxy.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hbuciggx.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2klcfmasu.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2lwrfebet.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2obpbkpul.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2poioifyq.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2fbfqnxgh.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt2rjkcierg.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt2ejcushkg.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt2lkcgcddz.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2ymbpkbtu.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2akqibgwj.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wxvvfixi.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2yywkhred.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pwoyvysq.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ccqpqpkk.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2qbglywxu.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2hggbwuwp.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2wvrprglc.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2xpqubjms.html


<!-- 参考信息 -->