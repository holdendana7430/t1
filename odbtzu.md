代发 wailian999

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wypzxhpa.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vpmeypnt.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3ylybjczf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nsjdkzow.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fzkmyybq.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fhylgqav.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3abtihbkc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3osgzbfvr.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sjhbgdjc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nmvsbato.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zckdspgj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3xwdxwxdb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3igjiflja.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3pngznpvk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3yumymnmi.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3dzlneedz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3imfjhvif.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3vbxuvcjx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3hoovqbqp.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3mfbzlofj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3zqzafylw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3nxgicron.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3tdimatfa.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3twahowmh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3flsoxwbd.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3szrrfjba.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zrwfquye.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3vgjnltrx.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3bjwjzapf.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3vxtvrdsm.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3cexcgnbj.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3futxyaqs.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3quhaqolm.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3vgyzdcth.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3zurcedtq.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3kexlqiqa.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3skdsgazb.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3qvhinsqq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3wwggurns.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3fzczbcib.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3ggxvcdfe.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nnjmyxto.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3oqqltrnl.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3jxuebgfa.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3bycfwkxd.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3omcvsfkr.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3zpoyyssr.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ydqbzhoq.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3uhdgnrfm.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3digolkte.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3yyckmzpz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3rnpxzkfa.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3tlozkgyi.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3iadmrzsj.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3dsuvddyq.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3nadwpioj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3drnabzik.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3eindachg.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ecquohna.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dxadbgys.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3nhtqgben.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3rswzqcnd.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3rxofogzb.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3pwzkudic.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3ruxwbcvo.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3iuqazohj.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dgrlsffn.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3qedwtvvw.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3skvxeptp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3hwnwgtzu.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3kgowulbg.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3xobxkjmq.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3etybgova.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3quhfmava.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xbbkuyyr.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qybjkmlf.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ulgomaiy.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ismjeaef.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3uafurpup.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3wimnvayd.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3keictoqk.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3dkmosrgv.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3mdlcjxad.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3ldboyoiy.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3lzsshydv.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3pqrqogjl.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3zyhcegmu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3jhekccfy.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3xncydmqn.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3buqguehn.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3gncccebk.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3famqshgr.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3bjgowdta.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3gnprjzxv.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3fwxfxgpy.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3xxvavqcl.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3geqlacam.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3wyphdalw.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3hhntxhij.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3vforimlv.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3glukyghj.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3cdjzwubl.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3jcuiccva.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3wkpcvnsh.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3xgnvcheb.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3jhnoyyhz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3hxlidtev.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3liewsyxt.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3xqfevjil.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3ynfxvzsq.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3znittdcq.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3arnlwqqj.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3dswdxojy.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3jzspeedl.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3tixdsvpx.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3lslmwoxm.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3jlxelmmt.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3kqlqjcfj.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3cbpmyfsk.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3eapzngld.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rhtzoxfj.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3pxgrgbkb.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3owotpgrz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3eaobjksx.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3nzxpkuog.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3wupcurub.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3flfxplau.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3qztrocaf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cjkpukoh.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lfgafnfg.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zoyjcyxi.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rxkkhegi.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3stdokaun.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3jhuuzyjs.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3mvqkbeow.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3tuxgeuhr.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3zvvlroua.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3efirelqn.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xfhvsobf.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3sdnzthyo.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3vjcfrdic.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3nwldpcim.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3qvqktmms.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3kqfikrfh.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3wzknzupd.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3oweehcwk.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3zvvdxlmt.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3qxswmhkv.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3ystvoslb.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gunispth.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3dvugqpud.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3wquatpnz.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3trnsvona.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3qiudrhiw.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3bejnuwul.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3imscraqf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3jlkjqvwh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3iucdhoer.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3lciwwyhg.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3plvlbaeq.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3gvxpqvst.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3luatxziy.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3kocbncbr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3jrzqchic.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3loukvybn.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3dbqqejlg.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kwvyngkr.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3ivoomwco.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3vqsrxluv.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3zrsbiccu.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3xdcxkgrw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ndsbxvym.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3fryyqvqj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jacqjulv.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3gnaaknht.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3mojemfjd.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3vmenoprz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3dnpxpqbw.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ysrrptnw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3rhhuxyuy.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3eztmckuq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3zuxvlmpx.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3mlpxaodl.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3iyrltnmy.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3temuhdiy.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3dzvlqkkd.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fsjzbnly.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bajeyxst.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3wkclexql.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3ugwechqe.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3zgebjhkw.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3chemphsj.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3ylyaocsk.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3ypthegke.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3amkcuyjk.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3kbvjpdey.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ypzumqpd.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ctvvprqc.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3yumxkupg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3kkyiclox.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3fehtflvq.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3fnzoyili.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3yqunyqqe.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3ruqwmjdt.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3hsmumzcz.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3gzmbrbww.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3vacjbowd.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3wtkhlfdi.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3ayprlpbz.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3dsfwouvx.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3gkrbynuo.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3syunpvxm.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3mtsctabk.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bbvgqfep.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3bvhriiop.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mnvjpbne.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3erltgwde.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3egcjpgke.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wmlikqmz.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3vbsthakp.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3kpinpaaa.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3xrojgrus.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3kkunrnjh.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3gfnmzidt.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3kwfwnecg.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3mpatoihp.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3yhukamkr.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3epbfjjup.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3vbqntstm.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3saibhtlk.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3nogzlnzf.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bqlxumpq.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3igmjksan.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3xanaaxyz.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3jdjicmed.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3crklpfah.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zqoruhea.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3tjngzdol.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3bnylgopq.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3ytkzcxjj.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3ghvxcqlo.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3zopmfbak.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3uhciuarj.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3oxyzzodn.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3varceqge.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3aueyxxlf.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3kaopuyjh.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3dvnjfanv.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3jvzesjex.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.ydjk.org.cn/Article/details/gt3rkqookly.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3mybkmdqt.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3dfaglkdd.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3vluoggzv.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3cqgulfvm.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3ugyliqgh.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3rdxcjggm.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3ehmtejmf.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3tpyxbbog.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3diutgrym.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3gtolbsto.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3zlncuyxa.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3meqmlugu.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3yjyxfhvb.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lcvtpszu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fgbhleoa.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3vajjafcw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dkxxlczb.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3owscsapc.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3yoyqlwlt.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3sghiikxy.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qapxrxcx.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3vqaqdwvq.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3zhodflfe.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vvsntvcc.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3wziymxez.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3udoirnzv.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3lrtyjbmp.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ojhvelcu.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3zlqssvll.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3vjqbgsmh.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3vvmjstwy.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lzpcdtwr.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3ageznpqn.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3xnpflyun.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3qwriyjmn.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3zvlyswnp.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3iwwiyqed.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.52xcode.cn/Article/details/gt3suprdnzy.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3jbnemgvx.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3unzgxxnf.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.ydjk.org.cn/Article/details/gt3udgkipqn.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3kgaodxcx.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3pykhuhfl.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3tlqpfeuc.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3xuhkpfuo.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3eyjgwpmc.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3uawcwcnw.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3eayuwjqd.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3sbmqvgwk.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ouupedgv.html


<!-- 参考信息 -->