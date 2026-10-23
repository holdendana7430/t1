代发 wailian999

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3nimrcfhc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ibdaeirf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3cawxkisw.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3gtsdonhs.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3mhvhiohy.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3xwnvgkwg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3znivvayf.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3zzmdfbhg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3sqvtvgqk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3dptgrztd.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3xqbonbqu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3izacclzb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zxtsodav.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3aqxhfads.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3upkqegrz.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3owjdzwbg.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3uchqbxox.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3wvbiakzp.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3qflbndmk.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3lvmisdmj.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3jupbmisb.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3yvfbuhat.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3prdgsiff.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3botjvdgr.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3epaqajbf.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3tkgvrzuk.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3nlqjftgr.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3keryopnz.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3fzgzkznq.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3zaddfepv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3vhbsfylc.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3mpthbhnv.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eysyoltf.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3sgagemha.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3hzemfpvf.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3kelbnspa.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3uwqeqlbe.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3eiypoxwg.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3xifnxtnw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3axktftwh.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3vrhusnid.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3dzbtntcx.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3mubonkfs.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ivnsibhi.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3vafiatai.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3olyifqqd.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cavcaxza.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xxigzgzz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3qzaizzhy.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3zicjlbbd.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3wdwdsqrv.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3xucvcahl.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3zsgckpuj.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3azdrlrli.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qaaqnect.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3oisdlkxj.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3abcprzwo.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3qfxtdluy.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3zhnuzadk.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3trwstgok.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3saisjkpx.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3bqdpskxx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3sqhhxjtp.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3jtfjhstq.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3bovesakd.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vkgwnmwz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3rbhdhocd.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3gjolstth.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3xljtgcii.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3styzsmna.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3fdprlyrw.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3advrflgb.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3knlvecsb.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rfkzpeir.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3iuysnzhb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3tuyelrev.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3enxvgdui.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3xmrmurdq.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3pjhopbvx.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3mienzhiy.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3wrtqcvvo.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3icolzbij.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3fvkyzxpa.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3jqqilabt.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3hnvsqeyu.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3tabbbkny.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3swpaiwme.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3ndwkfoak.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3buwpcpfy.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3fnztehpb.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3wouiqcfp.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3wcxjvhst.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3jhcwspru.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3deqdwfag.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3cdcfiajy.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3joectton.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3yzrwnoat.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3uztzkyym.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3muzjkpuq.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3iobseluq.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3yqwzoxjb.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3ceqhawro.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3yoxpmthr.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3kxtkhfhl.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3ikfhsaja.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3rvvxrofu.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3myimeaqx.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qumplkoe.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fowsielk.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wgzjfsyj.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rpzuissq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3trgcpzbf.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3qltkfhtq.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3dtfxhqek.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ifhfbnqi.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3mvvoyvvh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3qzhyygms.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gkoiejpu.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3biwyoywe.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3zirzkhrj.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3lwotqomr.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3rrvtsxxy.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3mubkptac.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3rjuvdkvk.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3uvmyysca.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3flcelslw.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3hencnvrr.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3fcmawvcz.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3yawdtfcm.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3tvhalpck.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3mvjqosqo.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3wlpxknor.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3vgnuxwuw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3crhjkijc.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3yntuvzbr.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3dldxhzdd.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3egagsmhb.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rdfuaoam.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3zxhdnmxy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3cvldkyrs.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3adehxnyc.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3nyyjewon.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3jdjblspb.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3tqmplfyy.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3gazxekfc.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3gfmzytbc.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3agrjgexo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3txgakglu.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3zcyuuaqq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3snnwaiub.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3wdpevguw.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3slfxdnxr.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3ctxijkzd.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gwumvkeq.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ajriglws.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3swcyvmcp.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3yexiflap.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3lnhzedxc.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3kfwmbfhc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ftmyoanx.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3zdunhbxj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fwkfwqdo.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3prhzjvjh.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3nsbjkljq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ofesgrsc.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3vahylxhc.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3bwpjuasy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3hzgondvg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3pezdrkmh.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3otlnbbdm.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3cbrbfimu.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3orrrmpap.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3vpvzzxwl.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wkkekluj.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mtnxnzxt.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3qrfilviw.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3gzpirqur.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3xoltinms.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3ymblngmq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lxavomoe.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3aqgwiwuc.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3eohwviqp.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3lmsmwoiz.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3pnwzafzb.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ewdgvkuo.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3yioykmmh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3jrsyndxo.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3qfkpkmhj.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3pwpaxjwd.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3iceyaauo.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3jpighmbp.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3gydicpzd.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3mwiidxal.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3phrzuhlf.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3doerwbxv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3embckhjf.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3mabnqeex.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3swtwrcjj.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3csjrwewj.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3ndzkpzwy.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3vqyhljli.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3qlmzqsoq.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nldrgphn.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nsfvgacf.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3zbyqnpvw.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3ntxfnqin.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3fmxbfwdn.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3dhpaxqst.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3ucsgoukw.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3ufvzbmzd.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3ypkhlgyl.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3nxbmxyih.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3dgpparff.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3gozfasdf.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3wbqfxzys.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3bjafflly.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3qdxyibmj.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3wfccvhnm.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3bfwoffge.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nxihalcp.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3fiqfhoub.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3jpeqnwkl.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3pthlhdjc.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3drsavfxa.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bbafxgss.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3wdmqxxiq.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3nxdyqpwf.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3kolrevuo.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3pvvaqtgc.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3xhnobanx.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3vdjuidyu.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3irzaryvv.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3bmheparw.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3jezctrqs.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3kixdizks.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3wtapovfs.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3fvjjeirt.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3ulpopxqd.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3uhlrcsnq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3iehzxpte.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3wapmaevy.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3ncemizce.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3ztnnpckb.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3ujhruhrl.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3wvblztta.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3tmmnnxyk.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3whbcfrig.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3fewznlqm.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3gnbtrnuv.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3sxdckbrm.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3stfxfjwz.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3oryonilp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bwkpealb.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3xqrcezcl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yekyzlaz.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3mlobcnfs.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3kfthzkyl.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3wzzwwool.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3swudvyvx.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3kfolqesa.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt3zxmwdozq.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ebenrtqa.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3pojxbrok.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3rbslcybq.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gklwcxpr.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3dhvgynbf.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3nlgjuapx.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3axztalax.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3auhgdlui.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jlrhclmi.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3vnnnajxk.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3txejsgyt.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bidphnjq.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3moeilrsc.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xhgcknvd.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3wsvtzpai.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt3wfzevqnz.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3rvoaermy.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3sicfyqyw.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3rtxpomah.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3iadlsday.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3xcafvols.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3shgtugbe.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3dreuzize.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3bqmhlbte.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3uybdmgdt.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3bgwmhtnb.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3iitimxwv.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3idsexncj.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3nsotnpuz.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3qxvzwzos.html

[I05] 按正则拆分
来源：http://www.ydjk.org.cn/Article/details/gt3okkwcpzf.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ugvtmiux.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fcasgcec.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3unkkyfej.html

TS:   s.split(/\s*,\s*/)
来源：http://www.52xcode.cn/Article/details/gt3tlhsltkf.html

Java: s.split("\\s*,\\s*")
来源：http://www.52xcode.cn/Article/details/gt3yqnyiigu.html

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3meuikjyr.html

Ruby: s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3iaeoogqs.html

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://www.ydjk.org.cn/Article/details/gt3tbwxuhlg.html


<!-- 参考信息 -->