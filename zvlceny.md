代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.fehbvm.com/Article/details/grzhroxac.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gyeachbqs.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gobngeety.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fehbvm.com/Article/details/gwjlvjldl.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.hesvh.cn/Article/details/gkyhiqnfi.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ggwpwdmel.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.zdbjq.cn/Article/details/guhsrcqfz.sHtML

[F12] CSV 读写
来源：http://mobile.zdbjq.cn/Article/details/gwtkrzjyx.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fehbvm.com/Article/details/grvxzumyk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.hesvh.cn/Article/details/gtiisdcrj.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.zdbjq.cn/Article/details/gswscpjkk.sHtML

TS:   // 同上
来源：http://wap.fehbvm.com/Article/details/gpmlsmdgv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.fehbvm.com/Article/details/giyqiqxck.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.hesvh.cn/Article/details/gunjmkauw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.hesvh.cn/Article/details/geuccmvlh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fehbvm.com/Article/details/gckeabqkb.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gdawpbsqi.sHtML

G. 面向对象
来源：http://m.share.hesvh.cn/Article/details/goczyeado.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjjhtlbso.sHtML

[G01] 定义类
来源：http://www.blog.zdbjq.cn/Article/details/gllrrkpsm.sHtML

Py:   class User: pass
来源：http://blog.hesvh.cn/Article/details/gjrpigudm.sHtML

PHP:  class User {}
来源：http://read.share.zdbjq.cn/Article/details/gqxptyaik.sHtML

JS:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gqcnujanj.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.fehbvm.com/Article/details/ghhhxjenx.sHtML

Java: class User {}
来源：http://www.m.share.fehbvm.com/Article/details/glulxtvkh.sHtML

Go:   type User struct { Name string }
来源：http://read.share.zdbjq.cn/Article/details/glegaioct.sHtML

Ruby: class User; end
来源：http://baike.fehbvm.com/Article/details/gzstzygtq.sHtML

C#:   class User {}
来源：http://blog.fehbvm.com/Article/details/glohcvram.sHtML

[G02] 构造函数
来源：http://3g.zdbjq.cn/Article/details/gufgnhnew.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fehbvm.com/Article/details/gwiduylsk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.fehbvm.com/Article/details/gdrgxqvsy.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gpwxvgyvt.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fehbvm.com/Article/details/gmdmllrqn.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gcuuhifsa.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.hesvh.cn/Article/details/gqhbumvle.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.zdbjq.cn/Article/details/gjizdyfvx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gkvoyyany.sHtML

[G03] 实例属性
来源：http://3g.zdbjq.cn/Article/details/gtyjnzjhn.sHtML

Py:   self.name = "x"
来源：http://m.share.hesvh.cn/Article/details/guhbggndw.sHtML

PHP:  public string $name = "x";
来源：http://m.share.fehbvm.com/Article/details/gegthpmde.sHtML

JS:   this.name = "x";
来源：http://baike.fehbvm.com/Article/details/gyqqddmff.sHtML

TS:   name: string = "x";
来源：http://www.share.hesvh.cn/Article/details/gzyvxaboh.sHtML

Java: private String name;
来源：http://www.blog.zdbjq.cn/Article/details/gdcwokzkp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fehbvm.com/Article/details/gnwtxtrrk.sHtML

Ruby: @name = "x"
来源：http://3g.zdbjq.cn/Article/details/gfmlemdgf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.fehbvm.com/Article/details/gkbvyxnuy.sHtML

[G04] 定义方法
来源：http://m.share.hesvh.cn/Article/details/gucxyyhgi.sHtML

Py:   def greet(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gkfhpgckl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gngifftmx.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gzumakjec.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gdwpvfpmi.sHtML

Java: String greet() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gnhiziktt.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gncpuljhx.sHtML

Ruby: def greet; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gsrxvmnma.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/gkpbuqazx.sHtML

[G05] 继承
来源：http://3g.zdbjq.cn/Article/details/gmlvdctfh.sHtML

Py:   class Admin(User): pass
来源：http://blog.fehbvm.com/Article/details/gyampjapp.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/ggflszqxd.sHtML

JS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gmqtmuhzn.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gggkbvclz.sHtML

Java: class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gxdedeton.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.zdbjq.cn/Article/details/gsbbasijg.sHtML

Ruby: class Admin < User; end
来源：http://mobile.hesvh.cn/Article/details/gtdpiveqv.sHtML

C#:   class Admin : User {}
来源：http://baike.fehbvm.com/Article/details/gclmhzuzq.sHtML

[G06] 重写方法
来源：http://blog.zdbjq.cn/Article/details/ggqaqibhx.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fehbvm.com/Article/details/gouowlvki.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gipqkdacf.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gqsxwtaae.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gtddsjoxw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gjeybeigm.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fehbvm.com/Article/details/gbtwoubjd.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.hesvh.cn/Article/details/goyqpvgpp.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fehbvm.com/Article/details/gsbecizgn.sHtML

[G07] 调用父类方法
来源：http://wap.fehbvm.com/Article/details/gwhvlxcma.sHtML

Py:   super().greet()
来源：http://wap.fehbvm.com/Article/details/gfhbvozpy.sHtML

PHP:  parent::greet();
来源：http://www.blog.fehbvm.com/Article/details/gzvomuqik.sHtML

JS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gkhbjcmid.sHtML

TS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/gilkucotf.sHtML

Java: super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gfiicnybo.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.hesvh.cn/Article/details/gcqkrfvjq.sHtML

Ruby: super
来源：http://www.blog.fehbvm.com/Article/details/gaarzewtf.sHtML

C#:   base.Greet();
来源：http://3g.hesvh.cn/Article/details/glaopgoed.sHtML

[G08] 静态方法与属性
来源：http://wap.zdbjq.cn/Article/details/gdqfxiqqe.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.fehbvm.com/Article/details/gddzobxzc.sHtML

PHP:  public static function f() {}
来源：http://m.share.hesvh.cn/Article/details/gbudltiem.sHtML

JS:   static f() {}
来源：http://baike.fehbvm.com/Article/details/gscwnnzfk.sHtML

TS:   static f(): void {}
来源：http://3g.fehbvm.com/Article/details/gpiavoqfq.sHtML

Java: static void f() {}
来源：http://mobile.zdbjq.cn/Article/details/glydzspfq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.zdbjq.cn/Article/details/gaxmqebnn.sHtML

Ruby: def self.f; end
来源：http://blog.fehbvm.com/Article/details/gukuvifui.sHtML

C#:   public static void F() {}
来源：http://www.share.fehbvm.com/Article/details/ginkkaxua.sHtML

[G09] 接口 / 抽象类
来源：http://3g.hesvh.cn/Article/details/gmqykfzwn.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.zdbjq.cn/Article/details/gnefebvoy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.hesvh.cn/Article/details/guufzkrkr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.zdbjq.cn/Article/details/gnldixgxc.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.zdbjq.cn/Article/details/garsjhqjx.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.zdbjq.cn/Article/details/ghcxajqzf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fehbvm.com/Article/details/guarbzoth.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.zdbjq.cn/Article/details/gvmhrntda.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gpqwhvcfx.sHtML

[G10] 访问控制
来源：http://www.share.zdbjq.cn/Article/details/gufepjshq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.hesvh.cn/Article/details/gzmjtgwav.sHtML

PHP:  public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/ggdfefqpg.sHtML

JS:   #private 字段；其余公开
来源：http://blog.zdbjq.cn/Article/details/gtqmnoydx.sHtML

TS:   public / protected / private
来源：http://wap.hesvh.cn/Article/details/glzrogepc.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.hesvh.cn/Article/details/gregwbfib.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.hesvh.cn/Article/details/gpjdsfdtq.sHtML

Ruby: public / protected / private
来源：http://wap.fehbvm.com/Article/details/gxinkeqkh.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.hesvh.cn/Article/details/gejpbckie.sHtML

[G11] getter / setter
来源：http://wap.zdbjq.cn/Article/details/gvlcldjxc.sHtML

Py:   @property 与 @x.setter
来源：http://3g.fehbvm.com/Article/details/gprkjlvhy.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gpxmsnyao.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gudpqqktj.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gapsuplou.sHtML

Java: public String getName() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gqqjhkfun.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gglujtlgn.sHtML

Ruby: attr_accessor :name
来源：http://baike.fehbvm.com/Article/details/ghgllvqfd.sHtML

C#:   public string Name { get; set; }
来源：http://blog.zdbjq.cn/Article/details/ghvbmesuh.sHtML

[G12] 对象转字符串
来源：http://blog.fehbvm.com/Article/details/gcnezhzxf.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gogrlzlfj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gswsykoeq.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gmjdliksh.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gftjbnqhq.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gxnjxuhvm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gqndpryuf.sHtML

Ruby: def to_s; @name; end
来源：http://blog.zdbjq.cn/Article/details/gzcriffds.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gvngznmeq.sHtML

[G13] 判断对象类型
来源：http://www.m.share.zdbjq.cn/Article/details/guvdkmeeo.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.hesvh.cn/Article/details/gxxbbxsut.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gzsodnhvy.sHtML

JS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/gqjrfpkrk.sHtML

TS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gdfdmrbdd.sHtML

Java: u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/ghgukypsv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.hesvh.cn/Article/details/guqdeouum.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.hesvh.cn/Article/details/gcbzxnwwk.sHtML

C#:   u is User
来源：http://blog.zdbjq.cn/Article/details/gsgnrnzwo.sHtML

[G14] 数据类 / record
来源：http://www.share.hesvh.cn/Article/details/ghxintsne.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.zdbjq.cn/Article/details/giznpclbm.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.zdbjq.cn/Article/details/gfbrxojgg.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.zdbjq.cn/Article/details/gbqhngisc.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.fehbvm.com/Article/details/gedecddna.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.hesvh.cn/Article/details/gqclmuohn.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.fehbvm.com/Article/details/gqzaeqeaj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.zdbjq.cn/Article/details/ghipyqsjd.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.hesvh.cn/Article/details/gpamccyyb.sHtML

[G15] 枚举
来源：http://m.share.fehbvm.com/Article/details/gcixzcwnc.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.fehbvm.com/Article/details/gpganoobv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.hesvh.cn/Article/details/gdvmokxre.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fehbvm.com/Article/details/gkxfvrckb.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gmqkxjkyo.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.hesvh.cn/Article/details/gfgdvwaui.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.fehbvm.com/Article/details/gfvnhhkez.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fehbvm.com/Article/details/gimbebkpn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/gtsrnhmos.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.hesvh.cn/Article/details/gbcvzzfwi.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.zdbjq.cn/Article/details/ghuprprze.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.fehbvm.com/Article/details/gwvlmiuat.sHtML

JS:   Object.entries(obj)
来源：http://baike.hesvh.cn/Article/details/gveskmfzj.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.hesvh.cn/Article/details/gjrgktkrm.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.fehbvm.com/Article/details/gahfysxol.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.zdbjq.cn/Article/details/gcqdeumsz.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.zdbjq.cn/Article/details/gbncnyicj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.zdbjq.cn/Article/details/gxgsegshx.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gautxqwri.sHtML

H. 异常与错误处理
来源：http://wap.zdbjq.cn/Article/details/gthocmgic.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gsitqvweq.sHtML

[H01] try / catch 基础
来源：http://m.share.zdbjq.cn/Article/details/gyznumzgc.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.zdbjq.cn/Article/details/gewgvgztb.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.zdbjq.cn/Article/details/gwmtuxely.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gfvlpwkod.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/gevuqjuob.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.hesvh.cn/Article/details/gbzhpuian.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.fehbvm.com/Article/details/gdtxftnxd.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.zdbjq.cn/Article/details/gpnwkyiux.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.hesvh.cn/Article/details/gxdvhzeol.sHtML

[H02] finally / ensure 收尾
来源：http://baike.fehbvm.com/Article/details/gkooohjwm.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.zdbjq.cn/Article/details/gwjdsjblw.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gxbiplhsf.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gibsqitjv.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gkwlbvpug.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gmbhyklyx.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fehbvm.com/Article/details/gdfjctfiw.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.hesvh.cn/Article/details/gruofofte.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gddelsuhh.sHtML

[H03] 主动抛出异常
来源：http://blog.fehbvm.com/Article/details/guuizvjnh.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.zdbjq.cn/Article/details/gtzuexgqx.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gimnybvth.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gvycoqolt.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gizgnjesh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gtvzjvrqg.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.hesvh.cn/Article/details/gvavvwyrb.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.zdbjq.cn/Article/details/guprabgcc.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/ggpcwxajh.sHtML

[H04] 自定义异常类型
来源：http://baike.zdbjq.cn/Article/details/gzofbwhkn.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.zdbjq.cn/Article/details/gqpfcndip.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/gdewzbczq.sHtML

JS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/gxomcuopg.sHtML

TS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/gsdbegiuy.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.hesvh.cn/Article/details/gakdjdizq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fehbvm.com/Article/details/gwgpuqwme.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.hesvh.cn/Article/details/gjuwwthue.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.fehbvm.com/Article/details/gwwnquzep.sHtML

[H05] 捕获特定类型
来源：http://3g.fehbvm.com/Article/details/geslanczn.sHtML

Py:   except ValueError as e:
来源：http://www.m.share.hesvh.cn/Article/details/gmujmdgpz.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.zdbjq.cn/Article/details/gufschzhm.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.hesvh.cn/Article/details/gnuilskpx.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/gddtpniia.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.fehbvm.com/Article/details/gvzrewvfn.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.fehbvm.com/Article/details/gydlnxhsj.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.fehbvm.com/Article/details/gexlrdyvh.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.zdbjq.cn/Article/details/ghvpghkbg.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.zdbjq.cn/Article/details/gnqaakbog.sHtML

Py:   value = d.get("k") or default
来源：http://wap.zdbjq.cn/Article/details/gophukxok.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/gfalzyyho.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.fehbvm.com/Article/details/gomiohcxx.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.zdbjq.cn/Article/details/gwytulsua.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://3g.zdbjq.cn/Article/details/gznpmgdss.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.hesvh.cn/Article/details/ghorlkdtq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.zdbjq.cn/Article/details/gjrtxfmtz.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.hesvh.cn/Article/details/gndabogdn.sHtML

[H07] 断言
来源：http://www.blog.zdbjq.cn/Article/details/gfovwqcmf.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.zdbjq.cn/Article/details/gpjkgopki.sHtML

PHP:  assert($x > 0);
来源：http://read.share.fehbvm.com/Article/details/glqgrkxqs.sHtML

JS:   console.assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gvkpknhlj.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gamiqkzhv.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.zdbjq.cn/Article/details/gueurpanc.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.fehbvm.com/Article/details/geuhwtogq.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.zdbjq.cn/Article/details/gqcrnisoh.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gwcfxkiqp.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.fehbvm.com/Article/details/gvrffjduw.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.fehbvm.com/Article/details/gzcnaqfxe.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.zdbjq.cn/Article/details/gscmgwrop.sHtML

JS:   e.message;  e.stack
来源：http://baike.fehbvm.com/Article/details/gmfmahvpq.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.fehbvm.com/Article/details/gzrraokjl.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://mobile.zdbjq.cn/Article/details/gbhcwovei.sHtML

Go:   err.Error()
来源：http://3g.fehbvm.com/Article/details/gjujgrriu.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.fehbvm.com/Article/details/glryutmbw.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.zdbjq.cn/Article/details/gnwuxpwzw.sHtML

[H09] 带错误码的异常
来源：http://mobile.fehbvm.com/Article/details/ggmkbtivc.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.hesvh.cn/Article/details/gjadhogji.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://baike.zdbjq.cn/Article/details/gscghfcpz.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.hesvh.cn/Article/details/gyxqgehzr.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://wap.zdbjq.cn/Article/details/gpprwawpu.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://read.share.hesvh.cn/Article/details/gszsvkcpa.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://www.m.share.hesvh.cn/Article/details/gxibueast.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.zdbjq.cn/Article/details/gfyomklda.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://3g.zdbjq.cn/Article/details/gnfkxxpdi.sHtML

[H10] 资源自动释放
来源：http://www.share.fehbvm.com/Article/details/gqpqzvuqi.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://blog.hesvh.cn/Article/details/gqozzaadb.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.share.hesvh.cn/Article/details/gfchktxzl.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://www.m.share.hesvh.cn/Article/details/gmlfvxmih.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://3g.hesvh.cn/Article/details/gtlhrkztm.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://baike.zdbjq.cn/Article/details/gwuhhpgpt.sHtML

Go:   defer f.Close()
来源：http://www.share.zdbjq.cn/Article/details/gbeghrubp.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.zdbjq.cn/Article/details/gioxuuxvy.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gnztanjrs.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghefvdiwe.sHtML

I. 正则表达式
来源：http://www.share.fehbvm.com/Article/details/gyurgkrtz.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/glbkinadk.sHtML

[I01] 判断是否匹配
来源：http://www.share.zdbjq.cn/Article/details/gymkceiyp.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://m.share.hesvh.cn/Article/details/ghfygluap.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://read.share.zdbjq.cn/Article/details/ghrnrtdjd.sHtML

JS:   /\d+/.test(s)
来源：http://www.blog.hesvh.cn/Article/details/gweyqtmxm.sHtML

TS:   /\d+/.test(s)
来源：http://wap.fehbvm.com/Article/details/gykevilnk.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://wap.zdbjq.cn/Article/details/gzmvhjetf.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://m.share.zdbjq.cn/Article/details/gfgmsivag.sHtML

Ruby: s.match?(/\d+/)
来源：http://mobile.hesvh.cn/Article/details/gjqneqtvn.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gvskjsaec.sHtML

[I02] 提取所有匹配
来源：http://baike.hesvh.cn/Article/details/gdoqobvjw.sHtML

Py:   re.findall(r"\d+", s)
来源：http://read.share.fehbvm.com/Article/details/gihcghdjy.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://www.blog.fehbvm.com/Article/details/gqjpkhmeb.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://www.m.share.hesvh.cn/Article/details/gdisdgwxd.sHtML

TS:   s.match(/\d+/g)
来源：http://m.share.zdbjq.cn/Article/details/gjroieqyz.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.hesvh.cn/Article/details/gyhmzakqo.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://www.share.fehbvm.com/Article/details/gztpiumkz.sHtML

Ruby: s.scan(/\d+/)
来源：http://www.m.share.fehbvm.com/Article/details/gdqfdidph.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/grcxzmfhk.sHtML

[I03] 提取捕获分组
来源：http://www.m.share.hesvh.cn/Article/details/gkvyelinl.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://www.share.zdbjq.cn/Article/details/galcqlzan.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://blog.fehbvm.com/Article/details/gkunwnurh.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.hesvh.cn/Article/details/gramunzow.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://mobile.hesvh.cn/Article/details/gabkjpelk.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://www.blog.fehbvm.com/Article/details/giszvmztc.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.m.share.zdbjq.cn/Article/details/gfdkqvmmz.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://m.share.zdbjq.cn/Article/details/ggxflqlxw.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://baike.zdbjq.cn/Article/details/gcswxqype.sHtML

[I04] 正则替换
来源：http://m.share.zdbjq.cn/Article/details/gfqkihnzh.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://m.share.hesvh.cn/Article/details/gpusyiula.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wap.fehbvm.com/Article/details/gqdipejef.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://baike.hesvh.cn/Article/details/gnutgtmgf.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://blog.zdbjq.cn/Article/details/gvngljelb.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://baike.zdbjq.cn/Article/details/gxphrizwn.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://3g.zdbjq.cn/Article/details/grsnerith.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://m.share.hesvh.cn/Article/details/guascrxzs.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://www.share.hesvh.cn/Article/details/gzlnzuzbn.sHtML

[I05] 按正则拆分
来源：http://m.share.zdbjq.cn/Article/details/gurzvpvcr.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://www.share.hesvh.cn/Article/details/gianhsdly.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://3g.fehbvm.com/Article/details/gkfulesgi.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://www.blog.fehbvm.com/Article/details/gkloxwbbq.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.zdbjq.cn/Article/details/ggkmdrfxv.sHtML


<!-- 参考信息 -->