代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3xrxkxvzk.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3wkdxsqeu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nglugsqy.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3glxpxnwp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3exlqsgou.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3frasipce.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3suzoxoqx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3obtexitf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ihxnjyle.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3opjpqnjw.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3xwdyppnc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hsuwwjlb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3qzayyujd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3iaaucqpj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3djcfzctq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3coopyndz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3nrjzqhno.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3bhdcksoc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3adzcnmqd.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3mgxvhzdx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3gzfpzaqp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3norklimp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3lobqyvek.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3dsoxuvda.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3alvrlfzy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3dzlcjuce.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3mwdtxcxc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3zzetlbha.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vebmsjnf.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3icrhelhu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qvfeqasv.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3xvzjlpid.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3ctejsewt.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3ygvhddcq.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3raqkzvjh.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3rtvhsupi.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3nomzocyr.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3hqlupmrb.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3jqrorcoj.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3vpchquco.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3tctirqzr.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3ykqjzljo.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3yxxvicdw.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ammcluhd.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3utbdhtxf.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3rkrnxtmz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3nobozszf.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3dhwnknby.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3crgyjzzm.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3okrdcaao.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3sbtlqonm.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3iohdtvad.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3zvgnabbl.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3zrmrmtts.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3xyrkxzdp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3bslobwne.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3tvasmitb.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ysqkpszo.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3pujzdwmg.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3hgdhjluq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3yuselwwk.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3iiagimpb.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3joxiuqay.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hlnnwjyi.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3rqeymphh.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3hfgaqstb.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ofeigmim.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3nqenltiy.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3xsletdgg.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ukmetkbl.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ywhvcvqa.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xzwzjlge.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xdrkxnxs.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3wthfvhll.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3keasgukp.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bbyhhmth.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3ilkrqvim.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3wtaalccp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3yxbkavrn.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3sszmhtxz.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qfnjijpv.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kpxgvpsf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3gnhitjyv.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3zzxwexuq.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3kdeycqgi.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3dfeevepr.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3uxaiovoq.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zqxsruam.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3msixkbnt.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3iotoyfju.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3erfnocdr.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3qigyapod.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3eywmavbo.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xhczqnwl.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3qylxgoah.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3qonjvgzu.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ifizttjg.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3hksktzqp.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3fxegzdeh.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3enwicuis.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3tetuqzfl.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3ybrrical.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3iqpsftxm.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3brsjwdqx.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3mqzyzmhk.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3rcaoboew.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3zklyzrqj.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3txokzgeq.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ynqejuos.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3wleuiocz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3vfdtiljk.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3fvnnfhez.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3zesqqflp.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3fkkzlgsm.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3cxsnagcj.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3tvuppjcx.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3sbndkddr.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3byvpvbxn.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3kbxunzua.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ovoprzwf.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3twaxdfij.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3kumzbsyd.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3yqtsbdbe.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3asemwxhm.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3adkpumpr.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3sooboddm.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qauotqjq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3uydfnlqw.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3xvhgqfmg.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3mipredny.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3kqikrkfk.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3xjetiuax.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3nsbeezlc.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xtrpyrdn.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mevzmduo.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vhsnerbc.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3fdfeksik.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3segxkrtd.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3gqmrxlgv.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3gpofhmlm.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3wrpnmizo.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ixkpsnwe.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3fnvhhucb.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3tgeckfps.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3bigaqtkm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3rgcszriz.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3snwvqalt.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3qdaxctpw.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3kngngvov.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3rqarbdpj.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3rzntcure.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3yknzwdro.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3ejaqbjly.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3qeemmvxo.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3jocpsdlf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3fwgfxzht.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3rsiibiwp.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3spadzoma.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3qpboxaal.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3zcavsmra.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3xusrwywb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3fcwthpdt.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3aqmpfbwi.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3nrhwjaih.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3ztgfacwr.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3becrfjxx.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3fpvobmsc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3vwrllnny.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3myqgocqq.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3uiotuxpj.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3txduekph.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3nfyvypzs.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3yesohdvm.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3szsxpueb.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3afsehyfw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fcseejhp.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3inziafuj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wluhyomb.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3eyhamcsw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3hcehwpkv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3roiszrzz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3nnojekbj.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3mmbungfi.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3gpeyjutx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3mywuzcvp.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3wttespyk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3hwyckbxr.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3xlmnsrxh.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3ijcbxuck.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3wltlpibk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3zpubesum.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3wtsjrmki.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dnylbarh.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3oyuuawwl.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3jzzqxspr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3vvqnryem.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3tkmcomvg.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3bklqovnn.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xxduoens.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3xkodjgjv.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3gasjmtfr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3vwyhfoln.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3znmuhtwz.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3pjyiatzd.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3znufebaz.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3unubehmt.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3qyqgboci.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3uxxvncot.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3eveaybhn.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3asyyletu.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3ucfjxrsd.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3wyuyllzb.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3zjvgwuwp.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3xaxcobku.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3ydbxoyot.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3uzgocexl.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3gfeqoonq.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3jtybwwjq.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3fxehuety.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3zwagvwgj.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3yycqsvph.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3dfcjxkva.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3euxmesxr.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3totrprgg.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3dhwyosya.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3dcvcqwpy.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3qcibfpez.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3etpmxrst.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3hmeycqyz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3gjwbuuax.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3egklkkkb.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3awtnvepw.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3irtbknfb.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3dgmzmvkv.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3grjywwgj.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3octwkynz.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3scpjmcep.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3qnhkfift.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3fvutuses.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3ugczucsj.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3rnfkwjuv.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3thkhpqyl.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3sdououaj.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3gleepcuv.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3mtpmkxxc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3mqnasbwx.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3qhskfoki.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3bizermym.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3xfsvtpyl.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3xoordprw.html

[H09] 带错误码的异常
来源：http://www.ydjk.org.cn/Article/details/gt3ikrpgnvz.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3uixobsmu.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3laloklzv.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3chnfgpsq.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3otddwleu.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3qhwlfrbc.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3rjlneqad.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3sgaisaks.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3brqtsfno.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3chmjenit.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3qsybhxpn.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3ydnvwzhg.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3yqvytaho.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3zckcpulj.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3gvhcxlmq.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3eiyfjrpa.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3rsajjhpx.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hyxfkhmz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3czeudilz.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3vdwgfytv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dtbfiact.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3aclvhrqc.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3occxgkjt.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ufrjoegx.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3iwvivlom.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3jmomkuea.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3mujlqaex.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yghgvkfg.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3xhrqhuye.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3pwspfgqh.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xszlpqbn.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3apyslacm.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3tyevplfd.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3ebawzdqv.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3hecdztxy.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3afcfrhhy.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3qooamffm.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3mohcxnjp.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3dwtjqfwd.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3wkljbuqy.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3onbihfpt.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3llgflxwy.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3arshbrwh.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3vgzvrhko.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3uxubtvft.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3vwaynocf.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3albptpci.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3sgknyjlu.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3mhwzfvzy.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3igfdktps.html


<!-- 参考信息 -->