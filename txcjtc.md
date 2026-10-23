代发 wailian999

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3rpabhnbk.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3gldxgsxl.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3clegdssi.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lmbxwztz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gwndnwzq.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wfxrpdrs.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3erhxtjhq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zzqbqxsr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wxppbztd.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ngzktqcg.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3qbmfytxu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fluzwhtu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3cdxdqqnc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3wrgrcaks.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3gmrzapko.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3bshruayw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3qvshnkfh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3crnnnpcm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3nnbcymeb.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3opypzplo.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3tfagibbp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3dpffgqbn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3ziapbqap.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3ncefhysq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3jmwiijem.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3zrnamekt.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3eqchyguu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3ldaavkbi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3grelyizk.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3ckbitiqz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ngagrsgd.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3upnayztr.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3svitzndd.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tezvnmyz.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jdjzinvt.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3nlfexwxx.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fbzbptwa.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3hznczwrj.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3hhqbcyxj.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ffseenxt.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3qelugrdq.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3jwqsmkgb.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3dtixhhty.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3cgbtpwgd.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fqjbjink.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hpgfxwru.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3ybmscxou.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3nlqtsjzq.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pgwcmexd.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3xhschdgo.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3pyhldyzw.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3bjombkpk.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ygjwrwsm.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3rjfbxppw.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3etsqzwpo.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3ejnhvqah.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3joviwokv.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3cimqjyfk.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3xzxlyzrk.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3pvikppof.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3dzhxynzu.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pivvkzam.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3zedfylav.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3mjlgccmu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3yswjdhsk.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3qpwliuga.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3nknmvkcm.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3ygdifiuh.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3woegwnzy.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3rpvzeyac.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ybtsnndi.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3snqbphth.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3dujgnvvp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3spzseixn.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3euqwxtan.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3whnhxbgs.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3eblfghez.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3fjybvlin.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3lnkpcqxs.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pnchvxnw.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3csqtmxpi.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3wojunuyp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3jzpwbqmr.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3gcanmyog.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3pkezgpcc.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3mqqxxwmc.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3txfzymnn.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3oinzyveg.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3entmjkxt.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xwjnmzll.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3rpwmuhum.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3ezuvqoyt.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3nackyurm.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vpfjdhgs.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3egsqsmnd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3kdwgftgx.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3ttcqhbon.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3rzugkhwy.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3epfyewcw.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3qszadpwn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3ucyuyrwn.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3wzzytmaa.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3zxkkfytl.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3bscdjbof.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3plidwbpu.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3nwdsimnq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3hxijcmag.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3yzyugkup.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3nyvmamti.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3jlzcfxmg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3fcpxgrgl.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3brkesijd.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3xseniryo.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3rivubkae.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3slgvsqiu.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3cunrkewg.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3rhdgqnxn.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3yviepnwx.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3bzsjhmtl.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3pupunqej.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3sfylmbtw.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3rcmlxqgb.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3igqjqonl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eypvmlmd.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3qfycjylr.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zjbpzfit.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bpooipdz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3hzcdwhab.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3yvgmtkys.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3aycnxktm.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vqnnajbg.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3texnsika.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uutxzdxh.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3kmpequjk.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bpgjwvyi.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kndznnyb.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3pzjgiszq.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3fuergvzc.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3gxzdxohv.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3kuptprxr.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3eujhnayx.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3bwrtebtv.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ovqxdlyk.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3lfalhitj.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3wxwziqxj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3lewiqbdu.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3lyhgqije.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3mvaixxay.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3aeqmktxw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3ipafgfmy.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3ojtcddml.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3kqwiddpv.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3jbevstiv.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3rakipoam.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3cllcwaym.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3smighdnh.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3kcwhhofe.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3cxvvease.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3lwmliypn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3djvxgsdy.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3vuibeazg.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3gaxgpvnr.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3otlvcufu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3owzsxyzh.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3izxyzhde.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3lxoivhdd.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3qldrgixm.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3tvgvbeqr.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3elttzvqq.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3xmaqqihi.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3vmuschjr.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3vuyrvuqa.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3ezpxtwmw.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3fmvavxoy.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3omovxjkx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3shtndyqz.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3chvsudpu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dynargtg.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3ktyhhvdo.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3vvzqemyw.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3zoopizta.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3sbsdrgmm.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3zxpexpin.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3sglzldht.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3rpzpncoo.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3nfdjnphs.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3qbwbvfzg.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3orhilugq.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3uwurujqv.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3oyzfxgad.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3drgftodz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dvimnnok.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xxfmznkl.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3wwguxbcm.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3jucwahkr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ibazzpge.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3iiyduyap.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3cmivjiwd.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3sbubcmmd.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3acsdtcge.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3atldzowt.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3tujavaoz.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3uwqmqmrk.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3zyvokenn.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3bhsrtoik.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3bftypahs.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3jylkmswf.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3fyidrmnm.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3vlsvzjtt.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3ipdlqotg.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3kmqcapuz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3vcbfsbhs.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3wccfcmzh.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3oaghmutw.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3mluprdgp.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3spjmbybe.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3byhjrdhe.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dlhranji.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3zeiycksz.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wohotoky.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3qpwincye.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3byneadgl.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3sifvtlfn.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3msicxeog.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3morervcm.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3ufynewhw.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3xgroxktz.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3zzsyatjp.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3jfkbewag.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3ryywvzll.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3itokigxr.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3nerxtlss.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3clrobnkg.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3usnrghoi.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3oafacsjn.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rmrlyibv.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xuekjqql.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3yugijvfr.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3spvgieik.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3vvyxhmok.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zlyzcfsd.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3fxulluhu.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3uqpgyhar.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3xnuylyaf.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3lcninfxx.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3kwltppfa.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt3ihngfkxl.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3pufyslzj.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3yugxoulc.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3etqlqnch.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3rchxifsb.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3scnzomfx.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3tobduegy.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3qqxgtukx.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3ytkzigco.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.52xcode.cn/Article/details/gt3qmiklqwb.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3klspgxbp.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3jhxthlqk.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3fgvofxvq.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3wdcfrghl.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3zjrykoji.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3zdsdznrs.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3ppjgfjpc.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3odfmrlbp.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.ydjk.org.cn/Article/details/gt3jrsokrhr.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3tfzhtmjn.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.52xcode.cn/Article/details/gt3fhtslzww.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pjcixuvq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iklngafg.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3nufvocnf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hfogirqo.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3crvaflzt.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3pqduystq.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3goyqkwak.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xvclcqsu.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3chkakrbt.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3cjcrrfcb.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3najaiasr.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3zrcvuosl.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3rhwdovyv.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3zocbnmft.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3zgqqvsoc.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3kjsgwphj.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3loawwnra.html

TS:   s.match(/\d+/g)
来源：http://www.52xcode.cn/Article/details/gt3vysrlvij.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3hbfibzaj.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3bfanwhon.html

Ruby: s.scan(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3zqemuqwu.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.52xcode.cn/Article/details/gt3dcobijrw.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3bxmadlxc.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3rjcbywkn.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3gcbxxhmp.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3gdafrram.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.ydjk.org.cn/Article/details/gt3qyofyrrs.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3yxhtuaks.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3mtapsjcj.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.ydjk.org.cn/Article/details/gt3hyucdkmj.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3neszllmf.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3zqlggykh.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3sxqmwbqz.html


<!-- 参考信息 -->