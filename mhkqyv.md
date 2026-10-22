代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rihrjzpk.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pjsqjjsl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2mmjiizfx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yquhyqbu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ieyspbtw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dpxitszr.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2jjmzfvsa.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2sinxcyfc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2csjclwbd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ginbnwbn.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2usvvpsev.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2tjwjwqvw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2gnblvvml.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2rljrkyln.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2gfdcmlwa.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2xqstfzsm.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2kwgedyxl.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2qdqgrvze.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2cdwpuqds.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2ipzvzvyk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2lqqxqcox.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2sefojfca.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2vnkkepgw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2fhnpgvyy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sbixuzwm.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2acogdxiw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mtfqjkpt.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2ctfhpvfn.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2fincupxa.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2sgwzarxs.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pdbcirxs.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2oyzlyvnt.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2hninmzjo.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2bcpujdwr.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2znmrvnsx.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ovbhfvcv.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2zmwjwnnu.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2apfwzsxd.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2xrkhkbhd.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2jtwcwwlw.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aawlflko.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2npycgowo.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2mfrvggkd.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2ojjcaipu.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bfyevpaj.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2zbjtjytu.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2eqwlhykq.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2fytxqyzp.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2tdzcexhd.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2gdxmuwnb.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2zrbqwwhf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2gsurhcvd.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ncgixxhp.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2imxukcfq.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2xtogiorm.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2aoawvtne.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bhmjxfes.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2idthdixl.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tuohnhmd.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2hpsxunpq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2vycnmnnz.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2qrytdtvp.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2uaietiax.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2mewyfmob.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2larkljyg.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2xnfbquqh.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2zyvzdkmt.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2skptvxia.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qaleczgl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2idyytlww.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2aezbktte.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ousiqnjd.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2mhjxbdga.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2jvalerot.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rbtsgxfi.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2wyawhgkn.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2zocdupfx.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lsnqqznr.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2cykgueum.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2cuwqghwc.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2yvjlvcye.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2qpmoesfb.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2qtzqwgwx.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2ijnhtmbr.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2holdqhmu.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ktgpawtx.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ibgdnqks.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2nidwgjzz.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2amvlahef.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2naadinjv.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2sroqmjso.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2avwponnp.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2hytqgbtl.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2ragratvi.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2irwlnxfy.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hjzwcasa.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2vxrclmmk.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2okhjxaov.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2fhrdyjkk.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2jmxgqjto.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2ucnclgmg.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2jscucxwj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2dgsgbejx.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2umnhukud.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2hmkqecsw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2tcsglkbo.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2jyoauqbp.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2czexucqp.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2leugwhfh.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2kxhmvolg.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2gbylqrrk.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2rqzizcvc.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2opoqrzbo.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2tpjwenvz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2tvhokzmy.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2lxfzjkgv.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2hyqjhmby.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2ueyoizwj.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2xpomlpiy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2bcxhtjue.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hsngmdjr.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cioydkkb.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vxsmqyrf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2fmqzysam.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2dtjaizoe.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2bkiclhuf.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qfzxamnv.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2zxlkkpts.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tpoeaqyu.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qajmgljz.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2edxxvcsy.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2yohkjakq.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2tgxqiejk.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2mwkmgmmt.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2yokwjlda.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2dsmyzxwq.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2bujtlzsn.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2zaxcrmzk.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2qqdnvloc.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2mxhtpqry.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2mtofziot.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2kooxqgnk.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2fcagboob.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2hlggfkuh.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2zgvwvtjo.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2ubkhsnvo.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2mzefmpgt.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2wbghoyth.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2shvppkmw.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2zwroqsnz.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2tayuiyey.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2xsvhaajl.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2wslhukvm.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2jggisggz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2wqgigkkr.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2ezvmwzmq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2pqktatoa.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2irgviowd.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2xyswwjuo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2hhpsuhio.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2oddogoec.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2wecppuik.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2cgbozxgi.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2mnppyjst.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2xypnitxz.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2lnswudve.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cpazswdu.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2srlzbida.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2vkgonuwu.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2tjwgyhmn.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2kppmiozv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dyffzbik.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2ihyxjbmo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kwbshizb.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2ilutgpsk.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2cbtfoqqp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2cxngwush.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2lnxsofxm.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2fircpnmv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2zwyxrdzx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2gnbulbuf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2goboefhm.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2rsmupnpo.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2xfcgpqvz.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2sfksohcw.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2nltwfdyy.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2cggfzsri.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bhxwdcoz.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rkfxkwdr.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2nsadwsdb.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2ydqexqeg.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xvqtcedo.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2jkresphl.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2vagdytrc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2uimrtcfh.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2tncbxgsq.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2iriwuiat.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hbxkfdsh.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2huxtiscy.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2lngemqhz.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2znrrpbhu.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2sudlllcu.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2nrvkosec.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2zuhymypo.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2vlmcacnh.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2yhiaceuv.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2vbsbciir.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2lzxxrlbb.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2vygcgftw.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2crkgkpuz.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2evwwmkus.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2kkqszvei.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2mvoehxqy.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tcrsypee.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ejhizplg.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ijhdvxfy.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2ssbsozsy.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2pzbpkdgq.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mvuhphpw.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2eyvcnnhn.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2nqdqbpfh.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2hjcyeoup.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2xlgxhdqf.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ozbvixje.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2gollpdfc.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2omrwpvew.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2zwyaebqy.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2yxbksrie.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2sqjxcqck.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2waavfaps.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ijpikhhl.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2gjdyezdx.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2tdpjgiac.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2kpcddkdf.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt2hzcfnidf.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2upwspauw.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hqehowue.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2myurfnst.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt2zjdluyhl.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2iertwozq.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt2atxlbhwi.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2ybganpjc.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2bbgegmhp.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2fwaagdos.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt2qaxfwzor.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt2rwvxyqkn.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt2matebaux.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt2aqdtotzs.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt2dizndbli.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt2erjthcqm.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt2cxkwhkez.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt2espslqfk.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt2evggqbrc.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt2grfyefas.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt2vgfapgoq.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt2rojvcuul.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt2tnlctagy.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt2zesvltzt.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2tyrfuitv.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt2gpkbishg.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt2epaasinb.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt2gyzvpsev.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt2avyvtflo.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2oyccnjem.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dmfwamup.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt2shqrybzm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gvpevbii.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt2ardrclfy.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2oxrekovl.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2sczusjws.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt2czquphjl.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fpthvmsu.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.52xcode.cn/Article/details/gt2hktrxepa.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt2maezsoki.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt2joyxpmvt.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt2bbcgehip.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt2dzklxhab.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt2auvfrftw.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt2fktxxrac.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt2iwewvgtd.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt2qnpttjeb.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bvnbtohm.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt2dowtmopi.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt2hzvbvabi.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2rxybanpd.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt2nboufyql.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cemllofw.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt2ozpauizc.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.52xcode.cn/Article/details/gt2akhaotar.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt2pxclzloq.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt2efyepchi.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt2ybfxfsoj.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt2qazuvvkp.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt2qasucprk.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2hhjwontd.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt2dgnyysby.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2svrrvhdt.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt2hulitgeg.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt2qfycslvt.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt2gypikzgq.html


<!-- 参考信息 -->