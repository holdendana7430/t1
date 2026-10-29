代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.zdbjq.cn/Article/details/gvczvqpxb.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gcejezlip.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gptztledy.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.fehbvm.com/Article/details/gempzcxim.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.zdbjq.cn/Article/details/gtqdfxmud.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gcmjxltpw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.fehbvm.com/Article/details/grlnrokbe.sHtML

[F12] CSV 读写
来源：http://baike.zdbjq.cn/Article/details/gqcdxxrau.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fehbvm.com/Article/details/gwyvggpvi.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.zdbjq.cn/Article/details/gotcivlet.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.hesvh.cn/Article/details/gdhufatwb.sHtML

TS:   // 同上
来源：http://read.share.fehbvm.com/Article/details/gliceghcc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.fehbvm.com/Article/details/gibdsfxqt.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.fehbvm.com/Article/details/ggamvixcr.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.hesvh.cn/Article/details/gumgcmcpu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.zdbjq.cn/Article/details/gkxoznxqo.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gvvnhtsxd.sHtML

G. 面向对象
来源：http://mobile.hesvh.cn/Article/details/gqncsjkjs.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gaxvafduv.sHtML

[G01] 定义类
来源：http://www.m.share.hesvh.cn/Article/details/gvsjwwkop.sHtML

Py:   class User: pass
来源：http://3g.fehbvm.com/Article/details/gdhpxayyg.sHtML

PHP:  class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gftapmhpq.sHtML

JS:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gifufesww.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.zdbjq.cn/Article/details/gthnwoavi.sHtML

Java: class User {}
来源：http://wap.hesvh.cn/Article/details/gxcftuwak.sHtML

Go:   type User struct { Name string }
来源：http://www.share.hesvh.cn/Article/details/gbcjcqscy.sHtML

Ruby: class User; end
来源：http://wap.zdbjq.cn/Article/details/gxwyxvujk.sHtML

C#:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gnsgythfg.sHtML

[G02] 构造函数
来源：http://blog.zdbjq.cn/Article/details/gwhqbywqf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.hesvh.cn/Article/details/gnmvidgsv.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fehbvm.com/Article/details/guasxefaj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gadqzvmrl.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fehbvm.com/Article/details/gklelecra.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/ggxktnpst.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.hesvh.cn/Article/details/ghbatbufr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.fehbvm.com/Article/details/gvmdhymjx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.hesvh.cn/Article/details/gkjjlirsl.sHtML

[G03] 实例属性
来源：http://baike.fehbvm.com/Article/details/gvchkrlhq.sHtML

Py:   self.name = "x"
来源：http://www.share.fehbvm.com/Article/details/guxbtkaxe.sHtML

PHP:  public string $name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gbujfnews.sHtML

JS:   this.name = "x";
来源：http://read.share.fehbvm.com/Article/details/gppqzttzl.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/gvwfkuyvf.sHtML

Java: private String name;
来源：http://blog.hesvh.cn/Article/details/grjxxspcw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fehbvm.com/Article/details/gzgrbdgvk.sHtML

Ruby: @name = "x"
来源：http://wap.zdbjq.cn/Article/details/gjydocnkb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.fehbvm.com/Article/details/gkyqezaby.sHtML

[G04] 定义方法
来源：http://www.blog.hesvh.cn/Article/details/gmhkwhokv.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/guhqeotrs.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gxceaardl.sHtML

JS:   greet() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/giqbdfiji.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gjunalrfl.sHtML

Java: String greet() { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gydfjaqfj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gxkadbojt.sHtML

Ruby: def greet; @name; end
来源：http://wap.zdbjq.cn/Article/details/gzegmivvt.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.hesvh.cn/Article/details/gmhrlzbip.sHtML

[G05] 继承
来源：http://read.share.fehbvm.com/Article/details/gdizroqcw.sHtML

Py:   class Admin(User): pass
来源：http://wap.fehbvm.com/Article/details/gsuwmiunc.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gdozsejhr.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gxwzfpikr.sHtML

TS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gquupondp.sHtML

Java: class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gkqkxuqsl.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.hesvh.cn/Article/details/gvjgyvsqu.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fehbvm.com/Article/details/gxnrjrodh.sHtML

C#:   class Admin : User {}
来源：http://m.share.hesvh.cn/Article/details/gdtryxztp.sHtML

[G06] 重写方法
来源：http://m.share.zdbjq.cn/Article/details/gqwsqlswx.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.zdbjq.cn/Article/details/gelusjldc.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gyurechoh.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gqxkzsmfu.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/ghznueozs.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gcwqjgnri.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.zdbjq.cn/Article/details/gtkycmzsi.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.zdbjq.cn/Article/details/grfunptec.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fehbvm.com/Article/details/ggwpsoipq.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/gpoxjappa.sHtML

Py:   super().greet()
来源：http://m.share.fehbvm.com/Article/details/gvlhdignz.sHtML

PHP:  parent::greet();
来源：http://wap.zdbjq.cn/Article/details/goajotdxm.sHtML

JS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gzptdlfhm.sHtML

TS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gvdpivpog.sHtML

Java: super.greet();
来源：http://read.share.hesvh.cn/Article/details/glkwmrvxi.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.hesvh.cn/Article/details/gbrsltozu.sHtML

Ruby: super
来源：http://read.share.fehbvm.com/Article/details/gcfhgwkja.sHtML

C#:   base.Greet();
来源：http://mobile.hesvh.cn/Article/details/glwlqgozf.sHtML

[G08] 静态方法与属性
来源：http://read.share.zdbjq.cn/Article/details/gakfjpyje.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.zdbjq.cn/Article/details/gljueffvj.sHtML

PHP:  public static function f() {}
来源：http://3g.fehbvm.com/Article/details/geddxhkgj.sHtML

JS:   static f() {}
来源：http://3g.fehbvm.com/Article/details/gyaaopjor.sHtML

TS:   static f(): void {}
来源：http://read.share.zdbjq.cn/Article/details/gggtaatdf.sHtML

Java: static void f() {}
来源：http://www.blog.fehbvm.com/Article/details/gcoizohbc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.zdbjq.cn/Article/details/griscpukt.sHtML

Ruby: def self.f; end
来源：http://wap.fehbvm.com/Article/details/gzpysxcge.sHtML

C#:   public static void F() {}
来源：http://www.share.fehbvm.com/Article/details/ghqyrdrny.sHtML

[G09] 接口 / 抽象类
来源：http://baike.zdbjq.cn/Article/details/gitewiham.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.zdbjq.cn/Article/details/gidyubgyy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.fehbvm.com/Article/details/gvkyxgnrh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.fehbvm.com/Article/details/gfbjwdqrk.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.hesvh.cn/Article/details/gyziinhgj.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fehbvm.com/Article/details/gajvtsoob.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.zdbjq.cn/Article/details/gwpurnxgy.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.fehbvm.com/Article/details/geuzzfpwk.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.hesvh.cn/Article/details/gvwzhebwe.sHtML

[G10] 访问控制
来源：http://3g.zdbjq.cn/Article/details/gpzkrgyza.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.hesvh.cn/Article/details/galtlxkbf.sHtML

PHP:  public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/ggkadvvwa.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.hesvh.cn/Article/details/gfbapvwda.sHtML

TS:   public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gymlhbmwh.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.zdbjq.cn/Article/details/ghlmmbvkw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.hesvh.cn/Article/details/gultfasbv.sHtML

Ruby: public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gkrcklbtq.sHtML

C#:   public / protected / private / internal
来源：http://mobile.hesvh.cn/Article/details/gyynrghqb.sHtML

[G11] getter / setter
来源：http://baike.fehbvm.com/Article/details/gtkllunip.sHtML

Py:   @property 与 @x.setter
来源：http://baike.hesvh.cn/Article/details/gfiwyshla.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/ggnipsksg.sHtML

JS:   get name() { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gtnjlchbm.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/gfucgxzgx.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gddirfswq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gauvpdoig.sHtML

Ruby: attr_accessor :name
来源：http://3g.zdbjq.cn/Article/details/gqtiaumnk.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.hesvh.cn/Article/details/gqvdkbbun.sHtML

[G12] 对象转字符串
来源：http://baike.fehbvm.com/Article/details/gvmhtvyya.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gcgmiysil.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gsroyfhtl.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gkpynlsgs.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkxmfmfpw.sHtML

Java: @Override public String toString() { return name; }
来源：http://blog.hesvh.cn/Article/details/gucjjtrni.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gijdcanto.sHtML

Ruby: def to_s; @name; end
来源：http://wap.hesvh.cn/Article/details/gvxbrnfte.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.fehbvm.com/Article/details/giewenmdm.sHtML

[G13] 判断对象类型
来源：http://wap.hesvh.cn/Article/details/gcoytciyr.sHtML

Py:   isinstance(u, User)
来源：http://baike.hesvh.cn/Article/details/gkiebizpy.sHtML

PHP:  $u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gzlqahwht.sHtML

JS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gqorustjk.sHtML

TS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gvymmfkmx.sHtML

Java: u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gqfdnizex.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.fehbvm.com/Article/details/gncjbagxu.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.zdbjq.cn/Article/details/gycswcbqr.sHtML

C#:   u is User
来源：http://3g.fehbvm.com/Article/details/gezmekjva.sHtML

[G14] 数据类 / record
来源：http://www.blog.zdbjq.cn/Article/details/gqryiuhkc.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.hesvh.cn/Article/details/gjvnbzxou.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.fehbvm.com/Article/details/gsfgzauci.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.hesvh.cn/Article/details/gvadgvpyo.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.fehbvm.com/Article/details/gkxmbivmp.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gclyobhlh.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.zdbjq.cn/Article/details/ghoiklvli.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.hesvh.cn/Article/details/gijyhieim.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.hesvh.cn/Article/details/gujqpfhmn.sHtML

[G15] 枚举
来源：http://read.share.fehbvm.com/Article/details/gkaqrumkn.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.hesvh.cn/Article/details/gpwdvinfm.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.fehbvm.com/Article/details/gtcwwvtzm.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.fehbvm.com/Article/details/gzusaoupj.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.zdbjq.cn/Article/details/gxexiqhqm.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.fehbvm.com/Article/details/gpwuoldrl.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.zdbjq.cn/Article/details/gguwbkiik.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.zdbjq.cn/Article/details/gotkborww.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/gkfpyplsd.sHtML

[G16] 对象转数组 / 字典
来源：http://baike.zdbjq.cn/Article/details/gfmxzjwhz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.hesvh.cn/Article/details/gwydnpzlm.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.fehbvm.com/Article/details/ghuiveraz.sHtML

JS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gisztxngf.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gpnbcznkm.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.zdbjq.cn/Article/details/gjhxtsury.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.hesvh.cn/Article/details/gvrfymunf.sHtML

Ruby: obj.instance_variables
来源：http://blog.fehbvm.com/Article/details/gzxtsijau.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.zdbjq.cn/Article/details/gewhumezn.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gltwspttq.sHtML

H. 异常与错误处理
来源：http://baike.fehbvm.com/Article/details/gkteslhwo.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/geljtsamr.sHtML

[H01] try / catch 基础
来源：http://www.share.hesvh.cn/Article/details/gdavxacja.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.fehbvm.com/Article/details/ggayhxvoh.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.fehbvm.com/Article/details/grvahoeoo.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gygkghsxr.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gxqtzbkup.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.zdbjq.cn/Article/details/gvnifivfp.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.fehbvm.com/Article/details/gjsraolmp.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.blog.zdbjq.cn/Article/details/gbyaekpmm.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.fehbvm.com/Article/details/gzhfgrulz.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.fehbvm.com/Article/details/gqxvkhntx.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.zdbjq.cn/Article/details/guvjklzcw.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gmwfzvwlh.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gdvjxjlep.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gyumxulxq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gytrnkdxp.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.fehbvm.com/Article/details/giqhgkgfw.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.hesvh.cn/Article/details/gdixsawsk.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gvoyhybox.sHtML

[H03] 主动抛出异常
来源：http://mobile.hesvh.cn/Article/details/grzsmtykq.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.zdbjq.cn/Article/details/ggwhfwckq.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gjjufjbyh.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/gbfwidrem.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/ggawnlxql.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gckpknrtq.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.zdbjq.cn/Article/details/gaaivhalh.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.hesvh.cn/Article/details/gicfijoen.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/ghmooppbt.sHtML

[H04] 自定义异常类型
来源：http://m.share.zdbjq.cn/Article/details/gijtkxqlv.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.hesvh.cn/Article/details/gajbdffph.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/gkbxnygta.sHtML

JS:   class MyError extends Error {}
来源：http://wap.hesvh.cn/Article/details/gcqidiofb.sHtML

TS:   class MyError extends Error {}
来源：http://blog.zdbjq.cn/Article/details/glgnyaolt.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/gsoborefe.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.fehbvm.com/Article/details/gnkprdwpj.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.hesvh.cn/Article/details/gkohszvpx.sHtML

C#:   class MyException : Exception {}
来源：http://blog.fehbvm.com/Article/details/gitkkizvx.sHtML

[H05] 捕获特定类型
来源：http://blog.hesvh.cn/Article/details/ghasszemt.sHtML

Py:   except ValueError as e:
来源：http://baike.zdbjq.cn/Article/details/grhqmcitz.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.hesvh.cn/Article/details/gdlmzkhsa.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/gpzbiifnu.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/gbpcyycrr.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.hesvh.cn/Article/details/geypemzen.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.hesvh.cn/Article/details/giqxsrfeb.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.fehbvm.com/Article/details/gvnphsfcq.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.hesvh.cn/Article/details/gbmfdieiz.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.hesvh.cn/Article/details/grynwiqws.sHtML

Py:   value = d.get("k") or default
来源：http://baike.zdbjq.cn/Article/details/gvdlmepis.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.hesvh.cn/Article/details/glkcomwxn.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.fehbvm.com/Article/details/ggrhmoirt.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.fehbvm.com/Article/details/gvyrfwcsz.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.zdbjq.cn/Article/details/glcoezecq.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://baike.zdbjq.cn/Article/details/gijoaojge.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.zdbjq.cn/Article/details/givwvkdwx.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.zdbjq.cn/Article/details/gfjbwketo.sHtML

[H07] 断言
来源：http://blog.fehbvm.com/Article/details/gwkskvcgu.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.hesvh.cn/Article/details/ghwabjvfm.sHtML

PHP:  assert($x > 0);
来源：http://read.share.fehbvm.com/Article/details/gubozcxnr.sHtML

JS:   console.assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gaxuvycfn.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gfvzsyxzu.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.zdbjq.cn/Article/details/glhirtenx.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.hesvh.cn/Article/details/gvfgajeby.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.zdbjq.cn/Article/details/gazsbclgt.sHtML

C#:   Debug.Assert(x > 0);
来源：http://mobile.hesvh.cn/Article/details/gqqolxxxo.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.m.share.zdbjq.cn/Article/details/gfsxnpvmi.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.fehbvm.com/Article/details/glayuhyxo.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.fehbvm.com/Article/details/gtrtzxhry.sHtML

JS:   e.message;  e.stack
来源：http://www.share.zdbjq.cn/Article/details/gbjandvcp.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.fehbvm.com/Article/details/gsqfezffo.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.hesvh.cn/Article/details/grdxgxooj.sHtML

Go:   err.Error()
来源：http://www.m.share.fehbvm.com/Article/details/gothixmbo.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.hesvh.cn/Article/details/grldhknwd.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.hesvh.cn/Article/details/glyeyjzlp.sHtML

[H09] 带错误码的异常
来源：http://read.share.zdbjq.cn/Article/details/ggerhkbzs.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.hesvh.cn/Article/details/gubrjpxas.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.fehbvm.com/Article/details/gcjfyhfkr.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://baike.hesvh.cn/Article/details/gkiqbdewt.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.hesvh.cn/Article/details/grbxjlpia.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.share.hesvh.cn/Article/details/gllwogvmu.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.blog.fehbvm.com/Article/details/gfocsgzcr.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://read.share.zdbjq.cn/Article/details/gyiowsnnw.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.blog.hesvh.cn/Article/details/gbwgmqakt.sHtML

[H10] 资源自动释放
来源：http://baike.zdbjq.cn/Article/details/gfdpihbze.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://read.share.fehbvm.com/Article/details/glkleirjx.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://m.share.fehbvm.com/Article/details/gygixnuyj.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://read.share.fehbvm.com/Article/details/grqymgoky.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.fehbvm.com/Article/details/gukzlshny.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://mobile.fehbvm.com/Article/details/givxhgepu.sHtML

Go:   defer f.Close()
来源：http://m.share.fehbvm.com/Article/details/geciemnug.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.zdbjq.cn/Article/details/gvxjrvjbl.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://3g.zdbjq.cn/Article/details/glemuujiq.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gbvjrnzjc.sHtML

I. 正则表达式
来源：http://mobile.zdbjq.cn/Article/details/glfusxrsi.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gqeqnirwg.sHtML

[I01] 判断是否匹配
来源：http://wap.hesvh.cn/Article/details/gacycarfc.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gnyyjietn.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://wap.hesvh.cn/Article/details/gmkqaeqdm.sHtML

JS:   /\d+/.test(s)
来源：http://www.share.zdbjq.cn/Article/details/giszrnjde.sHtML

TS:   /\d+/.test(s)
来源：http://www.share.fehbvm.com/Article/details/gmgpzlmxe.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.fehbvm.com/Article/details/gijlqdhsk.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://mobile.fehbvm.com/Article/details/gftbqutla.sHtML

Ruby: s.match?(/\d+/)
来源：http://www.m.share.fehbvm.com/Article/details/grfmollww.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.blog.zdbjq.cn/Article/details/geopwyalc.sHtML

[I02] 提取所有匹配
来源：http://mobile.zdbjq.cn/Article/details/grtvxyqwb.sHtML

Py:   re.findall(r"\d+", s)
来源：http://m.share.hesvh.cn/Article/details/gaszwiigf.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.share.hesvh.cn/Article/details/gapdjwxoz.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.fehbvm.com/Article/details/gtxlkjbfa.sHtML

TS:   s.match(/\d+/g)
来源：http://baike.zdbjq.cn/Article/details/graikcczj.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://www.blog.zdbjq.cn/Article/details/ghyevfxah.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.m.share.fehbvm.com/Article/details/gfqklocuu.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.fehbvm.com/Article/details/gkzkietrn.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/geqrlnfij.sHtML

[I03] 提取捕获分组
来源：http://www.blog.fehbvm.com/Article/details/gwrlcgaoe.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.m.share.fehbvm.com/Article/details/gzoowenjw.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://mobile.zdbjq.cn/Article/details/gwohxedsg.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://m.share.zdbjq.cn/Article/details/gjqpyorey.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.zdbjq.cn/Article/details/gmwlesbea.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.share.hesvh.cn/Article/details/geteidohd.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://mobile.fehbvm.com/Article/details/gvvsoyfop.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://read.share.fehbvm.com/Article/details/gmvsxsygx.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://blog.fehbvm.com/Article/details/goesvxymo.sHtML

[I04] 正则替换
来源：http://wap.zdbjq.cn/Article/details/gzlxpeccf.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://3g.zdbjq.cn/Article/details/gbuspdhxx.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://mobile.hesvh.cn/Article/details/gxtputbxz.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.hesvh.cn/Article/details/gpuzraadt.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.hesvh.cn/Article/details/glwjbmhri.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.blog.fehbvm.com/Article/details/gssymtscx.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.fehbvm.com/Article/details/gtegymmrt.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://blog.fehbvm.com/Article/details/gnyoxrbjv.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://baike.fehbvm.com/Article/details/gczxizrty.sHtML

[I05] 按正则拆分
来源：http://m.share.hesvh.cn/Article/details/gwrvdrtkn.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://wap.hesvh.cn/Article/details/gcdtntnkj.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gxdogcpqy.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://m.share.hesvh.cn/Article/details/ghorfyifp.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://m.share.hesvh.cn/Article/details/gmucelfhk.sHtML


<!-- 参考信息 -->