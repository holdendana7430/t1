代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ewhaxqch.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vtzdgnns.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2ejxcjdok.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vrevoney.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bwxjwnzj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ghueuigc.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2qtaqpfpg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fwlznlbj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2hhkkbqby.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tqsznwzk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kcphmrru.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2mdjgfxha.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2jddwilmg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sayhkzmd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2wipuqhhs.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2rjziwejz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2sualrcwj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2byfqnbep.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2wfvgrtqf.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2rieyxfpf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2tepxwzni.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2nyllvcvz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2gcbnbnbl.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2pwcokzaw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pddttsbb.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2dqqdamls.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fddyfsqd.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2rhsihuey.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2dupfkgbw.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2rfjsgtmr.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2veglsiml.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2yognbngh.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qucfsoto.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2xclkxifx.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2yhaxyyfi.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2oetiaawf.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2apwgoifu.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2nlqflbei.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2owsikkat.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pbhksews.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2hbebvbqx.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tujlqrlp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2qfkjdemi.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2ezemiytk.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yrbqridc.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2moamrdfa.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2nggfskne.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2reqbwbid.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2stpxmdyp.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2wvplbrss.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2qtogvapl.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2skwvrwxo.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2xclmlflc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2vsbujfwr.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2umjpgwcp.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2wunmflvd.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2rikpjoci.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qxiuyiqx.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2glqgpwhr.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jfpywdyw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2gnspoxew.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2tqetgcjw.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2egipvtif.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2hyzypxis.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2inakzvxh.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zuglxljx.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qoavgrgj.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2payjglvq.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yzbiaedx.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2uvxummye.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ixypljum.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2cwxznnyc.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2rtaioupz.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2ugphekgh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2lsicawnl.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2swhxwyqk.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zynrydha.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pyhkcpdp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2krezhqce.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2rxnxcbyf.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2eyukjups.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2nzlqtqda.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2wvsdrnaa.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2sywmtzvw.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2zlfxzyuw.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ndprjlqf.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2vpbxgann.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2lmfamtdb.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2pbvgcgxi.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2mmutrzwy.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2vznyyape.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2fzlznzbd.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2zspyitlu.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2yjdirvnn.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2kpzalbpm.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2aoumgjlu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2ydxyqwlm.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2rgortjah.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2lhohgloh.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2ytodkubx.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2czftnofu.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2qtsiwrce.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2qdkkhbbp.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2fcnfcxbh.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2tdavzrga.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2yqnuhjwx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2mxwiewxy.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ehkkyqsd.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2ksabocyq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2odmbzfrv.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2oabexeqr.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2flhavjmf.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2fyzxhnsy.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2qsruxmat.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2ohpvzmiy.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2afyiqhhe.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2ewcantlc.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2ofltqyjn.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2tsxrditx.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2opoxbaji.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yoeakmfn.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tjqizsjg.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2cgyqzcuc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2niszvgzo.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2zheiisrp.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2ilgrvnwz.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dtwonahh.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2brxmceif.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ynvgpcwq.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qdqzpqes.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2eeifjred.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2uvvrgzds.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2jkxbhivz.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2nlvqzvmg.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2iwnkgzbj.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2aghayohx.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2rbliulhm.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2jaytbhah.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2dptpfdna.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2dkmkiaid.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ahqmquxj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2dfblkcbt.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2fsjsngbw.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2qkzljvjw.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2oixxticq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2zkpzaosx.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2zejfjpmt.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2nwepvahr.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2yimsupfy.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2olnfuovv.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2oidtztwu.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2xmftwmum.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2jbvwxtff.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2indqixuf.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2gtbioaks.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2pgdgminc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2mqukjyhb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ijrwdxra.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2zefgoabo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2usybcklk.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2wiplonah.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2rakkvtvg.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2dbhecblv.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2bmnpxppk.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2ccqfnaex.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2yifovujt.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2whgvhwjo.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2hyrbeode.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2kqdlyxsl.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2okgowzmb.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2szickdwd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zqoypmle.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2ecvrmwtr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wbpbtpmo.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2ywetmwai.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2qynwbzgs.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2ubjjlljl.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2dxqhqrdi.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2koiyntjb.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2lrkhrtma.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2hnfrdsnv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2kqbtvsjt.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2peukwbpf.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2cestppwe.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2jtflxlpf.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2pvfzqqmc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xzrurkls.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2fpijmmbp.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2eyqlxdxt.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2ergydtjm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2oyrwtsbg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jqlrsdty.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2fgffwpyp.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2elgymlkr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2vtnpcarl.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2wjwuyjqm.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2sjcukbks.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ohezgkvt.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2bxxsvpmy.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2bfkoahei.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2klwyhwuy.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2btbeagzo.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2udgksgyi.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2wgpnnojq.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2qoweqzuu.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2ceicomfh.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2ocdftofh.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2zjvksjnt.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2fhspbnjt.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2gnhhxdln.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2tqrmqswt.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2aoxsutzb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2upomhmcq.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2jfxtuzeq.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ugqgcuty.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hsssvbtk.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2izoespgs.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2lcqwwlvu.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2orzttyob.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2nwruiibz.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2fijyjigc.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2cbrjuimp.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2cysdinbb.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2qpwgghoe.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2pyuimasc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2viiwjorq.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2rqmdpuga.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2lxuzduog.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2xxbjopnf.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2ndmfajgh.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2vivzckws.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xbhcazhz.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rilflphi.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt2exccqvjh.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2xnfgfknz.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2aqumgefw.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2chcldjtk.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2lccsozsl.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2vdepjklj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2wblpadgo.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2ddbcmbrr.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2otuoywwa.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2jwhjiylw.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2omvpwkqr.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt2drpckapt.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2ibhmcsnj.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt2gbnvgywu.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt2jclvnkzl.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt2ipsszwzn.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2prpvhwsh.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2bcxqrdjy.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt2ulbyvlhx.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2bmrumofh.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt2zyevorxx.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt2ylgqcerz.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2ijukseeh.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2cbnekmyp.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt2btliugxu.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt2rnpeozoi.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2qdnnayva.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2eavxsvgu.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt2ckvnmcwx.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt2uivsrdlr.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mrijutpr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2awrawhsw.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2hcyvfkdp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wsmgiicr.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt2tjofpbem.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2wyuqzyno.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pwnkdbsj.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yaqxwnvm.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tjgrhkrx.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2vhxbawqu.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oqslaamn.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2yikegoqv.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt2iyjuvmor.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mgaprgjf.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt2mvhpjpbw.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2trubozbk.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2hfomrtnv.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2kkonmxim.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xplsdxyz.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt2jlsmhzci.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2bkjwtycn.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt2bpnpwqkf.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2bzsoykud.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zqbiibbv.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt2ntwrpjrv.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2mvbofofg.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2riycgrhf.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2cxljjpfk.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt2ycacbipn.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2lhumpaye.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2nssbhppu.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2oadkhefm.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2pdzqoten.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cpgmpguv.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2qxjbjaxk.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2wrunfjlz.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2dnlanwcw.html


<!-- 参考信息 -->