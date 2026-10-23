代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3ngnzjiro.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3krbbpzrk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dfkljjsw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3nikpvgxk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3wjlzdfmp.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fpfzzgcz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3gtgtcwby.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3swwsqvtr.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3gzkpjqeq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3drogovqr.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3iraxckcm.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3idjtdhij.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3rrxugovo.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3xcwrdodv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3pmjsvjvy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3vjfemtkb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ldngfbzs.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3gztorcuy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ywdslzzp.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3zxsfhtwg.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3dskdhrtd.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3ibvcojfz.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3flbpaklv.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3lwsepark.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jlnqefam.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3ztegexqa.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3xxhkevna.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3geopdchm.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3vygrwyva.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3gxwbofiw.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dorivztq.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3fezvvhvh.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3ewhpwarv.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xarnkkwd.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3aadwbxys.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3levaumrw.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3mqbdfnnl.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3zzwfzsss.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3rscqpkvk.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3odpnbrqf.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3rhcdawxm.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3xcdmowra.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3ugphhzsl.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3zpweaoag.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3vcolvykx.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3udvubljs.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3dqnrryzz.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3uirliiev.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bcevwaiu.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3vxopuvls.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wyuwtrhk.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bgjpbztz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3xnahtphp.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ycmgrrwn.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3dmwxnjxi.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3fabsbdmh.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3smrvvche.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3rxlazizt.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cuzorord.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kcopdcyu.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3mlvnmyay.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3fuvatfgk.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3svggdrzh.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3utosnpni.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3ojubqvma.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3uxtxfixx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3oljexigm.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3yfgdrtio.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3exesusug.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hqztannk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3gimccqed.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3ikdytuvy.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3akaokgux.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3ndvpyira.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3tvijiwru.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3cqomuaje.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3xopvfgih.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bhiqqzer.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3tscsrhpo.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3trrzuepf.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3oerkueam.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rknsftmx.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3plmfhsje.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3nssdnnns.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3mkegytsj.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3abkoycbx.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3jzebxgvd.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3qdvutdge.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3kgjndeyj.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3yewivlfh.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3aiwetedm.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3afszggjg.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3sewolriy.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3hztaabky.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3kmnodipo.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3dheannqv.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wxgqjycr.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3pvdxghze.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3talksawe.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vimkhnst.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3cmpylpgj.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3oasqgchh.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3odhmwyyq.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3kkslibcw.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3xxikamiz.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3wlcjgyye.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3zkwoqmxx.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ahocklwg.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3lwsvdyxr.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3iemkvoau.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3qcbxxgzl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qvgsedgc.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3budrvjll.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3quxtbbni.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xkphvfws.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3bnsshjna.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3qzhakkin.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3tudpempd.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3qvpajsci.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3oeyuekkf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3vlkptelm.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3sidortou.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3enclihjb.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fiawshbp.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3sbhujper.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ankneoyc.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3dxwgvppu.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3mbfpjlbo.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3mvvyramh.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xglghwdn.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ajdqwtrx.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3lxgxhisl.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3rrpozrjt.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3chzgaoqe.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3bdeadkgc.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3fsfojlxc.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3uvasxvnk.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3bhqlmohd.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3lcljijam.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3dnnyvzej.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3dfrrqhmc.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gmfjjqmd.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3tcjptslx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3tcdtiiqx.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3xutxodqx.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3fteffcyt.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3xajbevtq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3aiomeylj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3xprgzhop.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qjpzfgzb.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3icojjrte.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3grliygxt.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3bxfwbukn.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3uniactss.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3wzzjcsoj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3ajfrejut.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3kdnthums.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ldhsrfae.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3rusmgsow.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3kljcjqdp.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3efpakuvs.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3bclofgvl.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3qqgcpfuu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3esajdttt.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3gyvazvjk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zhancptx.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3yzrgsybl.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3gakgfohu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sywahcqv.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3nlqzzffi.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3frprjrut.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3dwptitnx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3zeuupwtj.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3xldampyv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3luqsqxtb.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3uorurwkd.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3gjpjufqk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3sstefmkv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nipyhbmh.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3wjwqzodj.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3zhhrqfeq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3hqadcamj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3qnjqjvab.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3cwbpehov.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3dbxdfsgy.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3etpegodz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ztegajdd.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3dbafazop.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3hfgpxkio.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3cmbodoaq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3qpounhcs.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3jmwivbbu.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3aflxiogr.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3rbhhdlwm.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3rsibqcod.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3cuycuajn.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3wzqffdqs.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3dikoqlhm.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3mpnkxazo.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3hcdcrovk.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3xskrczeg.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3svzhwfyl.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3sugwxkkx.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3uctztzua.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3liwtvrtp.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3riywnbet.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3uanegjul.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wlchpeyi.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3zduwsfcq.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3iodfpvpk.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3hdlzbxln.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3nznaksas.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3psbsyujl.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3zjkspkno.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3zuhusegj.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3sxxkkoxi.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3qezmdqqr.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3rwhfbkho.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3wiopifuq.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3sxkmdnrz.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3djtyfvnz.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3tfvlwiwa.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3rjtqdcon.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hhrigybl.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3elsemvkk.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3szvewdhr.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3roxrzuji.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3tfkiziwe.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3crdpssya.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3dqhegsqf.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3yogunlma.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.52xcode.cn/Article/details/gt3bdcvbquh.html

JS:   e.message;  e.stack
来源：http://www.52xcode.cn/Article/details/gt3ezgzjtge.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3huzfieix.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3wtfevgrc.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3epuwfbcg.html

Ruby: e.message;  e.backtrace
来源：http://www.ydjk.org.cn/Article/details/gt3ijbxcwml.html

C#:   e.Message;  e.StackTrace
来源：http://www.ydjk.org.cn/Article/details/gt3bysoxdaq.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3cguyykvj.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.52xcode.cn/Article/details/gt3cnnxbmet.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.52xcode.cn/Article/details/gt3eiisgtcu.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3qryhxegs.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.52xcode.cn/Article/details/gt3qzecsotp.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3wfqqewui.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.ydjk.org.cn/Article/details/gt3hybojwyh.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3hbuyxbky.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.ydjk.org.cn/Article/details/gt3cbfrqlkp.html

[H10] 资源自动释放
来源：http://www.ydjk.org.cn/Article/details/gt3udnbxhts.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.52xcode.cn/Article/details/gt3lqzxhyau.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.52xcode.cn/Article/details/gt3rdzxkrte.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.52xcode.cn/Article/details/gt3adzutyvv.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3zlwieshu.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3inxlfegz.html

Go:   defer f.Close()
来源：http://www.52xcode.cn/Article/details/gt3mdhhrdzw.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3oheylpkx.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dyglikji.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eobpbwiz.html

I. 正则表达式
来源：http://www.ydjk.org.cn/Article/details/gt3bnbjruye.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jiftkcnv.html

[I01] 判断是否匹配
来源：http://www.ydjk.org.cn/Article/details/gt3rfxandqa.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3cwvcuzsx.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3oycbywln.html

JS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3eahevgnq.html

TS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3mzlpadoe.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3dssndouo.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oskehhdk.html

Ruby: s.match?(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3amivbhwd.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.ydjk.org.cn/Article/details/gt3lkgborgd.html

[I02] 提取所有匹配
来源：http://www.ydjk.org.cn/Article/details/gt3muevqxlq.html

Py:   re.findall(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3dxdyumsp.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3njcmjoyr.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.ydjk.org.cn/Article/details/gt3jdbqnkvs.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3mtkplvoh.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3njsifkll.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.ydjk.org.cn/Article/details/gt3xucfakch.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3xgqgkhuj.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3angyynil.html

[I03] 提取捕获分组
来源：http://www.ydjk.org.cn/Article/details/gt3hqsvjrpw.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.52xcode.cn/Article/details/gt3mxhhverw.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3vvtmxbpp.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3xhalgnaf.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3eqvwyfqy.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3iaunkgma.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.ydjk.org.cn/Article/details/gt3fldmjmgx.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3brgfmjni.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.ydjk.org.cn/Article/details/gt3zidhfpcf.html

[I04] 正则替换
来源：http://www.52xcode.cn/Article/details/gt3jwpfmlkj.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.52xcode.cn/Article/details/gt3qdptyowg.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ubqegnkq.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.52xcode.cn/Article/details/gt3refrncye.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3lgcjdxms.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3easarvzn.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.52xcode.cn/Article/details/gt3dlzxosgw.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.52xcode.cn/Article/details/gt3ttedjwsz.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.52xcode.cn/Article/details/gt3ltwsewcx.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3xyjeejtw.html

Py:   re.split(r"\s*,\s*", s)
来源：http://www.52xcode.cn/Article/details/gt3uxcktukv.html

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vtvudwnk.html

JS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3wwkpxxbi.html

TS:   s.split(/\s*,\s*/)
来源：http://www.ydjk.org.cn/Article/details/gt3nyqrfwlv.html


<!-- 参考信息 -->