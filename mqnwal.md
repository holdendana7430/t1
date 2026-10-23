代发 wailian999

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3mtawgaxc.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cjkzmlpe.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dofagvcf.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3bnzgupko.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3kqapwrcr.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ggecxxjj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3jprptrqe.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qbnxngvz.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3aoebqwef.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3zhrlvpyl.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iqvhmpud.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rzfwejzy.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3diuhwiai.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rhqjrvpu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3cscbwmvy.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ilybmvzq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tfikcwkq.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3awxsgbun.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3nnfewvrt.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rmvwuyht.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3mnxbyblh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bglhzwiy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ruyzczly.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3vcbztyns.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3gllaeolr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3oxwpbqme.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3zbmxiwqr.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3azkgrims.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3urxoeboe.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3ybmigvkj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3uazxztdx.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3zwberxcf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3chupwexv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3vynsyttr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3vtalxrsq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3haepwotc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jpjxhoku.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3jkcfzlqq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3upsqkcfe.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3nanoimmp.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3rwqzfuyp.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nuukojlb.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3bgtepdrq.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3zakybtte.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3niniflgj.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3drvmzjqr.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3ieejrozx.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3okavcvlf.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ueezopqi.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3vamineoz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uvklxqhv.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tpyyfowo.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3puzmzntq.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xdufcuep.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3hlgyaqwb.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3izjtvhhb.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ardukhqe.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3qvbxjpne.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3etcyszgn.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3cxkxtmsa.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3mgovhngm.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3eimmpitw.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3fuvufkxz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3hlthobsh.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3daozdfiq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3fttxfrpa.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3dgprwses.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3qbthuxqu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ystrffbn.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vzcwxjyc.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ypskdxzn.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zgczlhkz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3nmjghuyy.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3cslajlui.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3bmjgmten.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3gevhfbwu.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3rqessgqp.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lfguvwiy.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3kfsaswyc.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3aleiejhc.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3wrcspsny.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3cyulwwev.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3texbeqpv.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3qkujsczk.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3quvlgcsx.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3rpyngqbz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ebhftamp.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3alliueqd.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rovuvrpy.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3khrjuisg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3uvldzgqu.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3ayouobdn.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3nkzftlki.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3gmjuafjx.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3wnytchby.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3hvrxvglt.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3polpliky.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3gxkydhdr.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3spmvaitl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3bqihuzcz.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3eobyztlo.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3morgszdd.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3nrkcutfu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3sxwuioyk.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3gjakftny.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3wguuybbe.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3lwzvpjwo.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3iikzmxwo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3ggidlejh.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3dnebiynk.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3wvdnmmvf.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3jolwjykx.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3zfqayext.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3vdelunkw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3vfjjujyh.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3vxthtdie.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3hcjzbvre.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3kleckuse.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3phrlxpbk.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wktbafhe.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3dbhooqwj.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3xtzfziqv.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3jhkcojqe.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3osaelhbk.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3htjhqfaz.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3cteocgta.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3lqsesway.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3husdioiv.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3ctdvucro.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3teexvnqm.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3gtrboxrg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3xjyiqkjx.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3zbgpsaiy.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yjjqqcvq.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oxfpewtw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3fldphcii.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3dghxddpw.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3xawperpx.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3gdcrwvap.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3mtjnklnc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3downjyxj.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ddmsrmuu.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3gzvnwvva.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gsolstod.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ixdkaujg.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3tctmrtzs.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3liaobzen.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3gbxwitkd.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3lncitgwa.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ygkgncdk.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3plrssjvw.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3tbavkfhc.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3byncnfik.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3rrrdsjca.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3ltdphxfm.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3vqekxjum.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3wqeqnyiu.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3juvrrssu.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3wodxcfyq.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3viqsrcdl.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3zheekejn.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3leoljjoq.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3pqadrypg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3csexatai.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3aabnrseg.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3svpsrpzz.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3cmbbwixn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bqjerazn.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3xnyvvhxx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3bnwukymd.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3sunqzgmb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3rbaogmiy.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3ghxcazte.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3pjgqxish.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3oeineeqn.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3zknweifz.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3zwkjubtw.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3wrppprci.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3whukiudp.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3wfcpdnph.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3viuttncg.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3wfyooxkt.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3ttmbymwv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hbxygreg.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3wmhfcpqy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jpmislrb.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3ditrhthi.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3eyhlttwl.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3kioqmmvn.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3qtnvwxtu.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3ssgohjru.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3etfvskhe.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3wkvacvzf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3rvlengmz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3saojmqtz.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3tsupcpns.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3iafhgijc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ccdhzijb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3mkgsrtck.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3qafivgcv.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tssejnqw.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3vgrcrjac.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3gowrcljt.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cimiyoqy.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3jwwvtbar.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3otbfuzeg.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3mihtzxwn.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3pzatvlqi.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3paceviau.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xqalwvlk.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3bizqsmtf.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3fwklyagx.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3xtqszboz.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3mbecxumg.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3wcpkwgrl.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3txfuduri.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3wbuzujpi.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3ldihyqge.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3ncnfylbu.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3annktyei.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3thhvbalr.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3ekihzolr.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3cjpkyzkb.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3qnwkwoll.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3dfhkntkx.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3rldiomit.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fouztubr.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lwrmxowu.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3pcaandah.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3xduijqbp.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3hjbxjnze.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3ggyikqxd.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3lwlkexck.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3qrjwvlzd.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3wugzjtfa.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3womibhno.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3vzyadljb.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3jdgddqov.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3bmozqwiz.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3rkjxhprv.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3uonyhfae.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3nzvlcntt.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mmjtvngm.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3xqemxtpo.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lfivsooe.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3kmtegqlb.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3hhupmoam.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3ehbsahiq.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3drsqlaek.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3giafjyur.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3bvrkuozr.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3nueyqmnn.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3rthnjiqs.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3xcknfcpo.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3nqihjylv.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3dlfdiotk.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3potxzgjb.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3bgroszto.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3fsvszafp.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3udktgtpy.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3stcusvyk.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3sjhxtvja.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3coxbzzal.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3etpezfbb.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3pkbvccfc.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.52xcode.cn/Article/details/gt3qventklw.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3yrywnuqd.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3odpzcfjg.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3mhpeaduj.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3vmoztgpz.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3rhohvkms.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3vgmhgatv.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3bhoyfraj.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3zaggfgkl.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3iqxwnbwv.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qrbhqled.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cmupbecu.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3nzodmfsy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ewakwjwe.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3diioofbu.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3irujlkxr.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wcdwwtaf.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wqgekvqt.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3gmojnpgn.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3ambcxquz.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fgcvvixz.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3sypmonms.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ybfdlzuz.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ogllmpng.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3hcobqlfq.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.ydjk.org.cn/Article/details/gt3grkutkci.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3chnwvqju.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3ooohumyk.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3toowjahq.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3xlfhzbeo.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3evphvrqd.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ohmwpftu.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3okhmgoqw.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3tpbauewb.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3qjntgutw.html


<!-- 参考信息 -->