代发 wailian999

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sgepexeh.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xkapiocz.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3oawmcsit.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3snjktpgj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3owifruta.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3lfgxvkmo.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3vopuphzi.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3nnfjrzpa.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3rjhomktd.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rputvumb.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3heynqswt.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3ynztsrgz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3uzngmyvd.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3lzfrbmgn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3uifxwcqx.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3wmclfose.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3abdptkil.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3bedljjtx.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3svialehq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3bngiwiqc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bwrulumz.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3obcuysoi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3swnoemrh.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3xctdmarq.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3gkiiapqt.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3gmysflen.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wiyomasq.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3hvqiixiz.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3leqxtyjj.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3swwqlrnf.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3omuqfpwn.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3pttxioxc.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3afjpblji.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3vyasqorl.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xokabqzg.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3fjxtgnxu.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3hqupektu.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xomgwrhr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3jmpyglvy.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3zmhnlzkq.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3tfeecqox.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3ygkuylbu.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3oogmbgmx.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3jnuqputz.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3vqlasbgf.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3rngnrkis.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3dkgldzmr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3ysmlryhe.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3tqqihcad.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3gxclbjsm.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3pqrbulvm.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3kqcjvyvv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hrfelopg.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3uydbzfgg.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3snujysdw.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kbayilgs.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3redydakq.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3moudvoic.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3uayprynk.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3fsttmyke.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3olabuvcm.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ggyvkjqy.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3cdrncfet.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3swemjnff.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fpvexdwd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3ryxawkyd.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3eozoyziw.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3ydfspxtl.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3yeerpwdj.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3gzmnltuu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rxxvzmgc.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3auouiikf.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3baeqrgcg.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3gsrpdnho.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3nunpitgd.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3tsuabyag.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3iytucigr.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3ckwztmhe.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3snpdhbqh.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bbebxyvx.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3itkqjcfu.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3bpbbifas.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3hspadjzd.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3odzucbdf.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3hzbyhmgw.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3flhxfmwu.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3ztztznhs.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3xhedptpw.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3lnnsndtz.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3yhklujwk.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3leupbndq.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3cibvzvxd.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3zbhgmvrv.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3ryralkuf.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3oqnamroh.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3eaegixjc.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3ldjhukid.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3epuuaatc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3enseheit.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3phjalfmf.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jgcjzbxe.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3dhlotcwy.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3okiwwqqv.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xjxqtlad.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3qgqrupkv.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3hvqbyjfs.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3plbgfdro.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3nzxcekhf.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3cciuewld.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3zzoyopzu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3wxnwrdpu.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3szjtwqcv.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3owdvcedg.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3cocetzlw.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3gffuaocf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zlctagzo.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3rsqfxhaq.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3mnnakajv.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3zhdljqpl.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3mehpmkkw.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3reaamkxv.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3vrjclitp.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jdmdjlcm.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ludtcekc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3aguktzfo.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3khdvlohu.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aduatbpv.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3odsuqshd.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3zvgolqmr.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3sqxfetlh.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3smxfucmm.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3iuipohsh.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3wjdycuqu.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3hetnprpe.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3dsyeodmt.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3qlcvsydg.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3nxbomzdt.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3qgzcybof.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3qbwwnxmb.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3yxzbsurf.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3cletzrel.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3vuvmacti.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3fywdasim.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3vqifwlif.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3oeetqulb.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jgffzwzd.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3bhtjuxmm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3iebznvzh.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3fkjgbtoy.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3azafzxyj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3nxbpjdtp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qvgodkrb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3qbskhbln.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3qrdpqruo.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3yzryfsjr.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3gizqxuby.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3tipjgade.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jlstcons.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3yfxsrsrr.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3ydgxhuiv.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3jemndvii.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3smxihaad.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3bcvdhqox.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3eqgeagka.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3erqaegkm.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3qyathlrj.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3einbzuof.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uwbsmcnz.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3hrmxkpaw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3foxonpgg.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3gmjwpymz.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3vfmtewfx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3jbsqbhiv.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3dvszucpc.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3fbkhticz.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3mhcafoed.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3jbfolcnd.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3agefifiv.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3dgnuxtnm.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3sfruykcp.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3onltnwfb.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3oujzjxml.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3guljmqqp.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3gmrwozss.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3powzyaxe.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3cukdoltr.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3chlasaro.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3kgpkgyuc.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3ccaifpui.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3orjvlifh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3inmuozhy.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ugzozisi.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3maoakcbu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3hjfduroz.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3irwpciio.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3ugyqvplf.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ngfswlyb.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3hmmciywx.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3ibkwlgpe.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3ndvcapjz.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3wffxncio.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3gcyrsngw.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3gjmqfklm.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3irplijuu.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3tyxrdrgi.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3ytepvdkl.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3phcgjyqn.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3iizqitqt.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3zrcpfwil.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nzvrfmqt.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3dtdbchpt.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3qqbxzjtl.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3ewdjgizr.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3apckpios.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jayaiity.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3rmyqwnxa.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3kwykezgr.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3antfzwrr.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3yyafheww.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3xsizfmai.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3ajbrrkev.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3eyvjcbls.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3cgrvuqdc.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3wnlvyyjd.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3omvvxvaa.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3gdcmiafw.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3cuxasbat.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3qngwideg.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rmukmzdl.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3eoxkdtrb.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3mbgdqklo.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3fhxnpdic.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3kubktoma.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3rhilfnot.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3zkjkitvw.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3iubxyaiy.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3rejtodfx.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt3yapkzhpy.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3obwumedn.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt3ptropxfg.html

Ruby: e.message;  e.backtrace
来源：http://www.52xcode.cn/Article/details/gt3mgadzxft.html

C#:   e.Message;  e.StackTrace
来源：http://www.52xcode.cn/Article/details/gt3uprhorlt.html

[H09] 带错误码的异常
来源：http://www.52xcode.cn/Article/details/gt3ybhdsvbk.html

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://www.ydjk.org.cn/Article/details/gt3potokpje.html

PHP:  throw new RuntimeException("fail", 500);
来源：http://www.ydjk.org.cn/Article/details/gt3alzjoptt.html

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.52xcode.cn/Article/details/gt3mbetxkap.html

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://www.ydjk.org.cn/Article/details/gt3vufptapq.html

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.ydjk.org.cn/Article/details/gt3fcxsuope.html

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.52xcode.cn/Article/details/gt3nqyxxair.html

Ruby: raise MyError.new("fail", 500)
来源：http://www.ydjk.org.cn/Article/details/gt3qjpiaiet.html

C#:   // 自定义异常类中加 Code 属性
来源：http://www.52xcode.cn/Article/details/gt3gszlwijx.html

[H10] 资源自动释放
来源：http://www.52xcode.cn/Article/details/gt3nqdqjsvl.html

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.ydjk.org.cn/Article/details/gt3jvuessas.html

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.ydjk.org.cn/Article/details/gt3dsutqlzr.html

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3vklofpso.html

TS:   // 无 with：在 finally 里关闭句柄
来源：http://www.ydjk.org.cn/Article/details/gt3ypuqxvar.html

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.52xcode.cn/Article/details/gt3hhbkvtnb.html

Go:   defer f.Close()
来源：http://www.ydjk.org.cn/Article/details/gt3ayjonrpb.html

Ruby: File.open("a.txt") { |f| f.read }
来源：http://www.ydjk.org.cn/Article/details/gt3swseqkbx.html

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pkiaelhk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qfeybtxp.html

I. 正则表达式
来源：http://www.52xcode.cn/Article/details/gt3bcpbtatg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pvoxpvft.html

[I01] 判断是否匹配
来源：http://www.52xcode.cn/Article/details/gt3hrnalklx.html

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.ydjk.org.cn/Article/details/gt3mjajyqvg.html

PHP:  preg_match('/\d+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3sdksywwg.html

JS:   /\d+/.test(s)
来源：http://www.52xcode.cn/Article/details/gt3celopkif.html

TS:   /\d+/.test(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nivzftzt.html

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://www.ydjk.org.cn/Article/details/gt3iqrkvgqb.html

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.52xcode.cn/Article/details/gt3qujynspr.html

Ruby: s.match?(/\d+/)
来源：http://www.ydjk.org.cn/Article/details/gt3vdqgrwtd.html

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.52xcode.cn/Article/details/gt3wywqbprw.html

[I02] 提取所有匹配
来源：http://www.52xcode.cn/Article/details/gt3yebczfnr.html

Py:   re.findall(r"\d+", s)
来源：http://www.52xcode.cn/Article/details/gt3hkdfdcnd.html

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.52xcode.cn/Article/details/gt3vcvbkwaa.html

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.52xcode.cn/Article/details/gt3qbjaaseq.html

TS:   s.match(/\d+/g)
来源：http://www.ydjk.org.cn/Article/details/gt3ganhvlon.html

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.52xcode.cn/Article/details/gt3lagwwmrz.html

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.52xcode.cn/Article/details/gt3gifmqlny.html

Ruby: s.scan(/\d+/)
来源：http://www.52xcode.cn/Article/details/gt3meurhjyv.html

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3gzxbljco.html

[I03] 提取捕获分组
来源：http://www.52xcode.cn/Article/details/gt3xcwbklib.html

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ikgushfz.html

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3ivxeflyw.html

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.ydjk.org.cn/Article/details/gt3srxakfpi.html

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.52xcode.cn/Article/details/gt3yaagsbvo.html

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.52xcode.cn/Article/details/gt3xsiwpptt.html

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.52xcode.cn/Article/details/gt3ihfezsxf.html

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://www.52xcode.cn/Article/details/gt3vzyerywe.html

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.52xcode.cn/Article/details/gt3klrbdhdc.html

[I04] 正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3zviorago.html

Py:   re.sub(r"\d+", "#", s)
来源：http://www.ydjk.org.cn/Article/details/gt3taffqbjy.html

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mmoxluxx.html

JS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3rkoxomul.html

TS:   s.replace(/\d+/g, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3eoftjsba.html

Java: s.replaceAll("\\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3aukehubg.html

Go:   re.ReplaceAllString(s, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3yhrdekyp.html

Ruby: s.gsub(/\d+/, "#")
来源：http://www.ydjk.org.cn/Article/details/gt3muapbvjf.html

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.ydjk.org.cn/Article/details/gt3ftsvsjsl.html

[I05] 按正则拆分
来源：http://www.52xcode.cn/Article/details/gt3esttyquv.html


<!-- 参考信息 -->