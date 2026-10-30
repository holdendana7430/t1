代发 wailian999

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.hesvh.cn/Article/details/gbqcgiant.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/glgweobjr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gkahlmgsm.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.zdbjq.cn/Article/details/gjsisaqoy.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.hesvh.cn/Article/details/ggaqbknai.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gkmpojggw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fehbvm.com/Article/details/gxtvuhwej.sHtML

[F12] CSV 读写
来源：http://wap.hesvh.cn/Article/details/gmqvqutta.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.hesvh.cn/Article/details/gxpgnbywk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.zdbjq.cn/Article/details/gcgixarup.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.hesvh.cn/Article/details/gzxamfyfq.sHtML

TS:   // 同上
来源：http://read.share.hesvh.cn/Article/details/gajimnocf.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.zdbjq.cn/Article/details/gdkrdsgky.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.hesvh.cn/Article/details/gogodmfgs.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fehbvm.com/Article/details/gqojcfpat.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.zdbjq.cn/Article/details/grxzevfea.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gaxcrqrga.sHtML

G. 面向对象
来源：http://www.share.fehbvm.com/Article/details/gjyrncgux.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gqndgqlxc.sHtML

[G01] 定义类
来源：http://baike.hesvh.cn/Article/details/gkhkdjltf.sHtML

Py:   class User: pass
来源：http://m.share.hesvh.cn/Article/details/gwmpealfk.sHtML

PHP:  class User {}
来源：http://read.share.hesvh.cn/Article/details/gxznqienf.sHtML

JS:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gdpycuugr.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.zdbjq.cn/Article/details/gglxyzcfg.sHtML

Java: class User {}
来源：http://read.share.zdbjq.cn/Article/details/gsjfevvth.sHtML

Go:   type User struct { Name string }
来源：http://www.share.fehbvm.com/Article/details/gpfzjqoyk.sHtML

Ruby: class User; end
来源：http://blog.zdbjq.cn/Article/details/gpzqwzkrq.sHtML

C#:   class User {}
来源：http://wap.hesvh.cn/Article/details/gcnrqybyt.sHtML

[G02] 构造函数
来源：http://m.share.zdbjq.cn/Article/details/gjnbkzhsf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.zdbjq.cn/Article/details/godrhilka.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.hesvh.cn/Article/details/gyqtmekex.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gfdsapfye.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.hesvh.cn/Article/details/gsmuljfea.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gjbskuilr.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.hesvh.cn/Article/details/grjdwcviz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.hesvh.cn/Article/details/gehzjszji.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/giaicysnw.sHtML

[G03] 实例属性
来源：http://3g.hesvh.cn/Article/details/gjrjubtym.sHtML

Py:   self.name = "x"
来源：http://m.share.hesvh.cn/Article/details/gljcbxfwq.sHtML

PHP:  public string $name = "x";
来源：http://mobile.hesvh.cn/Article/details/gapnrmgcx.sHtML

JS:   this.name = "x";
来源：http://blog.zdbjq.cn/Article/details/gofpbvfcw.sHtML

TS:   name: string = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gkajnvmxs.sHtML

Java: private String name;
来源：http://www.m.share.hesvh.cn/Article/details/glhvtwfss.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fehbvm.com/Article/details/gjskdybau.sHtML

Ruby: @name = "x"
来源：http://blog.hesvh.cn/Article/details/gkkvivkpj.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gghvpesuy.sHtML

[G04] 定义方法
来源：http://wap.fehbvm.com/Article/details/gqzkdmgbi.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fehbvm.com/Article/details/gvvroxqdq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gsscilqlz.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gpljzopwf.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gnhtzbwyi.sHtML

Java: String greet() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gtwhdrhte.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gucpsamah.sHtML

Ruby: def greet; @name; end
来源：http://www.share.fehbvm.com/Article/details/gjjudpgbt.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/guaiffarw.sHtML

[G05] 继承
来源：http://wap.fehbvm.com/Article/details/gmbsojipo.sHtML

Py:   class Admin(User): pass
来源：http://baike.hesvh.cn/Article/details/gdsdtlonk.sHtML

PHP:  class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gsvkmdkmo.sHtML

JS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gzeeeqhtf.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxncnmldn.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gguqgetcq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fehbvm.com/Article/details/gmlcbeguc.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.fehbvm.com/Article/details/gmqecobrj.sHtML

C#:   class Admin : User {}
来源：http://blog.hesvh.cn/Article/details/gkcwesvas.sHtML

[G06] 重写方法
来源：http://www.m.share.fehbvm.com/Article/details/gcnbesnle.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.hesvh.cn/Article/details/gqvgvhrjh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gpldquxyw.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gkrgyxxor.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gtbieflat.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/ginyvxarw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.fehbvm.com/Article/details/gibpfnvio.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.fehbvm.com/Article/details/gcqatbgat.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.zdbjq.cn/Article/details/gphjnrqym.sHtML

[G07] 调用父类方法
来源：http://mobile.hesvh.cn/Article/details/gtoiheqqk.sHtML

Py:   super().greet()
来源：http://wap.fehbvm.com/Article/details/gswfjnlcc.sHtML

PHP:  parent::greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gsivoiktv.sHtML

JS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gvlgqqkkp.sHtML

TS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gxfyatpmu.sHtML

Java: super.greet();
来源：http://read.share.hesvh.cn/Article/details/gnancoiqx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.zdbjq.cn/Article/details/glabdlghg.sHtML

Ruby: super
来源：http://wap.fehbvm.com/Article/details/gnbharmzi.sHtML

C#:   base.Greet();
来源：http://blog.hesvh.cn/Article/details/guegtddxd.sHtML

[G08] 静态方法与属性
来源：http://baike.fehbvm.com/Article/details/gdqynigjg.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.hesvh.cn/Article/details/gxksngdbm.sHtML

PHP:  public static function f() {}
来源：http://www.share.fehbvm.com/Article/details/gwzwylodo.sHtML

JS:   static f() {}
来源：http://read.share.fehbvm.com/Article/details/glkmzsmrp.sHtML

TS:   static f(): void {}
来源：http://m.share.hesvh.cn/Article/details/gzrabnpog.sHtML

Java: static void f() {}
来源：http://read.share.hesvh.cn/Article/details/ggcmvijeg.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.hesvh.cn/Article/details/gzbjxhjil.sHtML

Ruby: def self.f; end
来源：http://blog.fehbvm.com/Article/details/gpzdnnbay.sHtML

C#:   public static void F() {}
来源：http://3g.hesvh.cn/Article/details/gajuahfbp.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.zdbjq.cn/Article/details/gvrzipqia.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.zdbjq.cn/Article/details/golbhkbbg.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.zdbjq.cn/Article/details/gjadnlzsb.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fehbvm.com/Article/details/gvenmdbrj.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fehbvm.com/Article/details/gexaekeab.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.zdbjq.cn/Article/details/ghphdwcyl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.hesvh.cn/Article/details/glslroreo.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.zdbjq.cn/Article/details/gckqchbgi.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.fehbvm.com/Article/details/grunlrhxo.sHtML

[G10] 访问控制
来源：http://baike.hesvh.cn/Article/details/gyfpsisfk.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fehbvm.com/Article/details/gdrvcepjp.sHtML

PHP:  public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gyhryedzd.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.zdbjq.cn/Article/details/goqkxnaaz.sHtML

TS:   public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gaicxqwvk.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.fehbvm.com/Article/details/gjswuemwu.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fehbvm.com/Article/details/gyxditfxd.sHtML

Ruby: public / protected / private
来源：http://wap.fehbvm.com/Article/details/gbinmduoh.sHtML

C#:   public / protected / private / internal
来源：http://3g.zdbjq.cn/Article/details/gbgeismlr.sHtML

[G11] getter / setter
来源：http://m.share.hesvh.cn/Article/details/gazvngaqv.sHtML

Py:   @property 与 @x.setter
来源：http://3g.fehbvm.com/Article/details/ghzklcrlm.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gwilfyspe.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fehbvm.com/Article/details/ggrcxhqqd.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.fehbvm.com/Article/details/gqmhzergw.sHtML

Java: public String getName() { return name; }
来源：http://baike.fehbvm.com/Article/details/gvisrxcji.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/glnggapol.sHtML

Ruby: attr_accessor :name
来源：http://baike.zdbjq.cn/Article/details/gqhwjmhlu.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.fehbvm.com/Article/details/gslmwnfch.sHtML

[G12] 对象转字符串
来源：http://baike.fehbvm.com/Article/details/gkfxyxmzz.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/glmqxbxil.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gdklqtsdc.sHtML

JS:   toString() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gahonnvck.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/goppbdeos.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gwrwtktqn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/glhdicrdh.sHtML

Ruby: def to_s; @name; end
来源：http://3g.fehbvm.com/Article/details/gzyxwsbde.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.fehbvm.com/Article/details/gzigqjvws.sHtML

[G13] 判断对象类型
来源：http://www.blog.zdbjq.cn/Article/details/gxykjpqdg.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.hesvh.cn/Article/details/gnsjmdoyp.sHtML

PHP:  $u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gwujgzhou.sHtML

JS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/ghjeoudpj.sHtML

TS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gkhunxrme.sHtML

Java: u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gofsrscvq.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.zdbjq.cn/Article/details/gwndcrjkv.sHtML

Ruby: u.is_a?(User)
来源：http://blog.zdbjq.cn/Article/details/gfrrtlbux.sHtML

C#:   u is User
来源：http://mobile.hesvh.cn/Article/details/gsmsyluwb.sHtML

[G14] 数据类 / record
来源：http://3g.zdbjq.cn/Article/details/gqapdgbib.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.zdbjq.cn/Article/details/gykywwmhg.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.fehbvm.com/Article/details/ghmjrnbzb.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.hesvh.cn/Article/details/gllnrjbwe.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.zdbjq.cn/Article/details/gdalyyrlb.sHtML

Java: record User(String name, int age) {}
来源：http://3g.fehbvm.com/Article/details/gwofblnul.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.hesvh.cn/Article/details/gwzkuqjba.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.fehbvm.com/Article/details/grevbniji.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.zdbjq.cn/Article/details/gxvooxvwk.sHtML

[G15] 枚举
来源：http://3g.hesvh.cn/Article/details/geupahhoz.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.hesvh.cn/Article/details/gbuelpeiq.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.zdbjq.cn/Article/details/gwgthejig.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.fehbvm.com/Article/details/gwfafnpve.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gpoxijudh.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.hesvh.cn/Article/details/guvebqfek.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.zdbjq.cn/Article/details/gxgdpeutj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.zdbjq.cn/Article/details/gidhfvpfx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/glxuomfbe.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.fehbvm.com/Article/details/gyztthbfm.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.zdbjq.cn/Article/details/guxrddstd.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.fehbvm.com/Article/details/gsrzsvqwn.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.fehbvm.com/Article/details/ggesbeuui.sHtML

TS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/gtozqckdo.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.fehbvm.com/Article/details/gzsxlnocm.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.zdbjq.cn/Article/details/gzncvvcsj.sHtML

Ruby: obj.instance_variables
来源：http://3g.fehbvm.com/Article/details/gkemeemay.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/gyxublxqv.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gcjbfzmtd.sHtML

H. 异常与错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gcmybzhrc.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghqjajuuo.sHtML

[H01] try / catch 基础
来源：http://3g.fehbvm.com/Article/details/gxmomijxi.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.zdbjq.cn/Article/details/gmsbmeenn.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.fehbvm.com/Article/details/gzokjxqen.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gmyjwfuwv.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.zdbjq.cn/Article/details/grwftxeku.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://read.share.hesvh.cn/Article/details/gebcgrhcq.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.zdbjq.cn/Article/details/gnegapwou.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.zdbjq.cn/Article/details/gtpmskgjj.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.hesvh.cn/Article/details/gqvyafhfk.sHtML

[H02] finally / ensure 收尾
来源：http://baike.hesvh.cn/Article/details/gzsljwlhm.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.hesvh.cn/Article/details/gtxnyhnfk.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/ggxtqjadz.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/ggrgzvbpr.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gqatovdki.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/gmnnfamtb.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.fehbvm.com/Article/details/gbllgoymj.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.hesvh.cn/Article/details/gbjkkdfdx.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gvyupiwkh.sHtML

[H03] 主动抛出异常
来源：http://blog.fehbvm.com/Article/details/gttvwsaur.sHtML

Py:   raise ValueError("错误信息")
来源：http://wap.fehbvm.com/Article/details/gswmulzcd.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gqqscuaxz.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/gkowvgxaa.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gwhqgtrab.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gignrirnj.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.fehbvm.com/Article/details/gvfnurbvb.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.fehbvm.com/Article/details/gbxwqwtxx.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gaxmoelqu.sHtML

[H04] 自定义异常类型
来源：http://blog.fehbvm.com/Article/details/gnhpmxtdp.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.zdbjq.cn/Article/details/gculyupci.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/gcvhscjjy.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.zdbjq.cn/Article/details/gmpzadbjs.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.zdbjq.cn/Article/details/gjpmazuur.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/gdlbsevbk.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.fehbvm.com/Article/details/gwglnskyr.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.fehbvm.com/Article/details/gxpyigztx.sHtML

C#:   class MyException : Exception {}
来源：http://3g.hesvh.cn/Article/details/grqrzohkt.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.fehbvm.com/Article/details/gxkpnhtfz.sHtML

Py:   except ValueError as e:
来源：http://www.share.zdbjq.cn/Article/details/guzsbivwe.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.hesvh.cn/Article/details/gonljuepg.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.fehbvm.com/Article/details/gcrxrapzs.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.hesvh.cn/Article/details/gvtsluzax.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.hesvh.cn/Article/details/ggipoivfi.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.zdbjq.cn/Article/details/gyuoimgyg.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.hesvh.cn/Article/details/gspmcbprt.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.hesvh.cn/Article/details/goqueaeul.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.fehbvm.com/Article/details/gaejuazge.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.hesvh.cn/Article/details/gwqrqetjq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.share.zdbjq.cn/Article/details/gvuphgkrs.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.hesvh.cn/Article/details/gpphqgtdq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.hesvh.cn/Article/details/gpoewcmjh.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.zdbjq.cn/Article/details/gpolyxyfc.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.hesvh.cn/Article/details/gynbtuwoe.sHtML

Ruby: d&.dig(:a, :b)
来源：http://wap.fehbvm.com/Article/details/gnjzjdnil.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.zdbjq.cn/Article/details/gdxgsywqi.sHtML

[H07] 断言
来源：http://baike.fehbvm.com/Article/details/gntjlbnwn.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.fehbvm.com/Article/details/gefddmfwz.sHtML

PHP:  assert($x > 0);
来源：http://m.share.zdbjq.cn/Article/details/grjoorvrb.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/glgqaohtf.sHtML

TS:   console.assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gqmurxlwf.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.hesvh.cn/Article/details/glqjebvwz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.fehbvm.com/Article/details/gilouqaac.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.zdbjq.cn/Article/details/gsqwixmdj.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gvwfhsydh.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.hesvh.cn/Article/details/gvrvxhltm.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://blog.fehbvm.com/Article/details/gdcziriyy.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.fehbvm.com/Article/details/gqetotpyu.sHtML

JS:   e.message;  e.stack
来源：http://baike.hesvh.cn/Article/details/gjjedhxgu.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.zdbjq.cn/Article/details/gpaczgqbx.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://baike.zdbjq.cn/Article/details/gspjcvujj.sHtML

Go:   err.Error()
来源：http://m.share.hesvh.cn/Article/details/gqzysupsq.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.share.hesvh.cn/Article/details/ghxnysfgf.sHtML

C#:   e.Message;  e.StackTrace
来源：http://wap.zdbjq.cn/Article/details/gcdbzmspc.sHtML

[H09] 带错误码的异常
来源：http://read.share.hesvh.cn/Article/details/gajxlqmoo.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://mobile.fehbvm.com/Article/details/gffuuknwh.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://wap.zdbjq.cn/Article/details/gdjherxho.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://3g.hesvh.cn/Article/details/gxyjgadtj.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://blog.fehbvm.com/Article/details/ghyzivhrn.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.zdbjq.cn/Article/details/gidsnorxy.sHtML

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://wap.fehbvm.com/Article/details/gvimcgavy.sHtML

Ruby: raise MyError.new("fail", 500)
来源：http://wap.zdbjq.cn/Article/details/grxpnynyh.sHtML

C#:   // 自定义异常类中加 Code 属性
来源：http://www.m.share.zdbjq.cn/Article/details/gexckuewp.sHtML

[H10] 资源自动释放
来源：http://www.blog.fehbvm.com/Article/details/gzlhxyjoh.sHtML

Py:   with open("a.txt") as f: data = f.read()
来源：http://www.share.hesvh.cn/Article/details/giwgdcjjg.sHtML

PHP:  // 无 with：在 finally 里 fclose()
来源：http://www.blog.fehbvm.com/Article/details/giuohqpsf.sHtML

JS:   // 无 with：在 finally 里关闭句柄
来源：http://mobile.hesvh.cn/Article/details/gnldjjnup.sHtML

TS:   // 无 with：在 finally 里关闭句柄
来源：http://blog.hesvh.cn/Article/details/gbfaqabwr.sHtML

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://www.share.fehbvm.com/Article/details/gnkccgyab.sHtML

Go:   defer f.Close()
来源：http://mobile.zdbjq.cn/Article/details/ghkuyvhem.sHtML

Ruby: File.open("a.txt") { |f| f.read }
来源：http://baike.fehbvm.com/Article/details/gzxltbsyw.sHtML

C#:   using var stream = File.OpenRead("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gnwermugw.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gozggvoix.sHtML

I. 正则表达式
来源：http://wap.zdbjq.cn/Article/details/gbnfhztqx.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghmluysrg.sHtML

[I01] 判断是否匹配
来源：http://wap.zdbjq.cn/Article/details/glwkgtuwr.sHtML

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://3g.fehbvm.com/Article/details/gvconkccj.sHtML

PHP:  preg_match('/\d+/', $s);
来源：http://m.share.hesvh.cn/Article/details/glmunkuth.sHtML

JS:   /\d+/.test(s)
来源：http://3g.zdbjq.cn/Article/details/gnkzycqsj.sHtML

TS:   /\d+/.test(s)
来源：http://www.blog.zdbjq.cn/Article/details/giijdhnzv.sHtML

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://3g.fehbvm.com/Article/details/gxfuoazie.sHtML

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://www.blog.fehbvm.com/Article/details/gkzwxjcgq.sHtML

Ruby: s.match?(/\d+/)
来源：http://3g.zdbjq.cn/Article/details/gehvmhyhg.sHtML

C#:   Regex.IsMatch(s, @"\d+")
来源：http://www.m.share.hesvh.cn/Article/details/gcoubdcwt.sHtML

[I02] 提取所有匹配
来源：http://wap.zdbjq.cn/Article/details/gdznauyvv.sHtML

Py:   re.findall(r"\d+", s)
来源：http://www.blog.hesvh.cn/Article/details/gqxvhaexy.sHtML

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://read.share.hesvh.cn/Article/details/gevefzhqc.sHtML

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://read.share.hesvh.cn/Article/details/gqeoxapiy.sHtML

TS:   s.match(/\d+/g)
来源：http://www.blog.fehbvm.com/Article/details/gpeyhnlud.sHtML

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://read.share.fehbvm.com/Article/details/gyutqmvdj.sHtML

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://baike.fehbvm.com/Article/details/gueutxraz.sHtML

Ruby: s.scan(/\d+/)
来源：http://baike.zdbjq.cn/Article/details/gwedimxoq.sHtML

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://3g.fehbvm.com/Article/details/ghirbvxwi.sHtML

[I03] 提取捕获分组
来源：http://m.share.zdbjq.cn/Article/details/gshxzuggj.sHtML

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://3g.hesvh.cn/Article/details/geovmpjek.sHtML

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://www.share.zdbjq.cn/Article/details/gijsliavx.sHtML

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://www.share.fehbvm.com/Article/details/gjgagyojt.sHtML

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://www.m.share.fehbvm.com/Article/details/gaeejykpd.sHtML

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://mobile.fehbvm.com/Article/details/gepeisvfu.sHtML

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://www.blog.zdbjq.cn/Article/details/gfuggtesp.sHtML

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://3g.hesvh.cn/Article/details/gloagtfnb.sHtML

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://www.share.zdbjq.cn/Article/details/gskumfbob.sHtML

[I04] 正则替换
来源：http://www.share.fehbvm.com/Article/details/gjriabnio.sHtML

Py:   re.sub(r"\d+", "#", s)
来源：http://www.share.fehbvm.com/Article/details/gpzwgwfkk.sHtML

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://baike.zdbjq.cn/Article/details/gphblysfu.sHtML

JS:   s.replace(/\d+/g, "#")
来源：http://www.share.zdbjq.cn/Article/details/gaxgoqisf.sHtML

TS:   s.replace(/\d+/g, "#")
来源：http://mobile.fehbvm.com/Article/details/ghttbpbtd.sHtML

Java: s.replaceAll("\\d+", "#")
来源：http://www.m.share.hesvh.cn/Article/details/gsbvgtndu.sHtML

Go:   re.ReplaceAllString(s, "#")
来源：http://www.blog.zdbjq.cn/Article/details/gjlaoekoy.sHtML

Ruby: s.gsub(/\d+/, "#")
来源：http://www.m.share.hesvh.cn/Article/details/gicvnkoun.sHtML

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://m.share.hesvh.cn/Article/details/gpagbtvcl.sHtML

[I05] 按正则拆分
来源：http://www.share.fehbvm.com/Article/details/gwpoguigk.sHtML

Py:   re.split(r"\s*,\s*", s)
来源：http://m.share.zdbjq.cn/Article/details/glaijhkov.sHtML

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gkkwzbpfh.sHtML

JS:   s.split(/\s*,\s*/)
来源：http://mobile.fehbvm.com/Article/details/gjbcqlxcx.sHtML

TS:   s.split(/\s*,\s*/)
来源：http://3g.hesvh.cn/Article/details/geaqoyeur.sHtML


<!-- 参考信息 -->